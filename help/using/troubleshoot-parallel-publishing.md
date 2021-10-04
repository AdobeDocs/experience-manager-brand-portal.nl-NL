---
title: Problemen met parallelle publicatie naar Brand Portal oplossen
seo-title: Troubleshoot issues in parallel publishing to Brand Portal
description: Los parallel publiceren problemen op.
seo-description: Troubleshoot parallel publishing.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
role: Admin
exl-id: 631beabc-b145-49ba-a8e4-f301497be6da
source-git-commit: e95dbff93ec4d207fe32a1752f9ccf59ee7c4e90
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 0%

---

# Problemen met parallelle publicatie naar Brand Portal oplossen {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal is geconfigureerd met Experience Manager Assets, zodat goedgekeurde merkelementen naadloos worden opgenomen (of gepubliceerd) in de authoringinstantie van Experience Manager Assets. Eenmaal [geconfigureerd](../using/configure-aem-assets-with-brand-portal.md), gebruikt de auteur van de Experience Manager een replicatieagent om de geselecteerde middelen aan de wolkendienst van Brand Portal voor goedgekeurd gebruik door de gebruikers van Brand Portal te herhalen. De veelvoudige replicatieagenten worden gebruikt Experience Manager 6.2 SP1-GFP5, Experience Manager GFP 6.3.0.2, en verder om hoge snelheidsparallelle publicatie toe te staan.

>[!NOTE]
>
>Adobe raadt aan een upgrade naar Experience Manager 6.4.1.0 uit te voeren om ervoor te zorgen dat Experience Manager Assets Brand Portal correct is geconfigureerd met Experience Manager Assets. Een beperking in Experience Manager 6.4 geeft een fout terwijl het vormen van de Middelen van de Experience Manager met Brand Portal en de replicatie ontbreekt.

Bij het configureren van de cloudservice voor Brand Portal onder **[!UICONTROL /etc/cloudservice]** worden alle benodigde gebruikers en token automatisch gegenereerd en opgeslagen in de opslagplaats. De de dienstconfiguratie van de wolk wordt gecreeerd, worden de de dienstgebruikers die voor replicatie en replicatieagenten worden vereist om inhoud te herhalen ook gecreeerd. Het leidt tot vier replicatieagenten. Dus wanneer u een groot aantal middelen publiceert van Experience Manager naar Brand Portal, worden de elementen in een wachtrij geplaatst en verdeeld onder de replicatieagents via Round Robin.

Nochtans, kan het publiceren met tussenpozen als gevolg van grote sling banen, verhoogd Netwerk en **[!UICONTROL Disk I/O]** op de instantie van de Auteur van de Experience Manager, of vertraagde prestaties van de instantie van de Auteur van de Experience Manager ontbreken. Het wordt daarom aangeraden de verbinding met de replicatieagent(en) te testen voordat u begint met publiceren.

![](assets/test-connection.png)

## Fouten bij eerste publicatie oplossen: valideren, uw publicatieconfiguratie {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

Uw publicatieconfiguraties valideren:

1. De foutenlogboeken controleren
1. Controleren of de replicatieagent is gemaakt
1. Verbinding testen

**Logboeken bijhouden tijdens het maken van Cloud Service**

Logboeken van staarten controleren. Controleer of de replicatieagent is gemaakt of niet. Als het maken van de replicatieagent mislukt, bewerkt u de cloudservice door kleine wijzigingen aan te brengen in de cloudservice. Valideer en controleer opnieuw of de replicatieagent wordt gecreeerd of niet. Als dat niet het geval is, bewerkt u de service opnieuw.

Als bij herhaaldelijk het uitgeven van de wolkendienst het niet behoorlijk wordt gevormd, rapporteer een dagzorgkaartje.

**Verbinding met replicatieagents testen**

Logboek van de mening, als de fouten in replicatielogboek worden gevonden:

1. Neem contact op met de Klantenondersteuning.

1. [opschonen](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) opnieuw proberen en opnieuw publicatieconfiguratie maken.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### Bestaande Brand Portal-publicatieconfiguraties opschonen {#clean-up-existing-config}

De meeste keren dat publiceren niet werkt, kan de reden zijn dat de gebruiker die publiceert (bijvoorbeeld: `mac-<tenantid>-replication` heeft niet de recentste privé sleutel, en daarom publiceert ontbreekt met &quot;401 onbevoegde&quot;fout en geen andere fout wordt gemeld in de logboeken van de replicatieagent. U zou het oplossen van problemen kunnen willen vermijden en een configuratie in plaats daarvan tot stand brengen. Voor de nieuwe configuratie om behoorlijk te werken, schoonmaak het volgende van de opstelling van de auteur van de Experience Manager:

1. Ga naar `localhost:4502/crx/de/` (aangezien u auteursinstantie op localhost:4502: in werking stelt\
   i. verwijderen `/etc/replication/agents.author/mp_replication`
ii. delete 
`/etc/cloudservices/mediaportal/<config_name>`

1. Ga naar localhost:4502/useradmin:\
   i. zoeken naar gebruiker `mac-<tenantid>replication`
ii. deze gebruiker verwijderen

Nu wordt het systeem helemaal schoongemaakt. Nu kunt u proberen om een config van de wolkendienst tot stand te brengen en nog de bestaande toepassing JWT te gebruiken. U hoeft geen toepassing te maken, u hoeft de openbare sleutel niet bij te werken vanuit de nieuwe cloudconfiguratie.

>[!NOTE]
>
>Wijzig geen automatisch gegenereerde instellingen.


## Zichtbaarheid ontwikkelaarsleider JWT-toepassing {#developer-connection-jwt-application-tenant-visibility-issue}

Als op `https://legacy-oauth.cloud.adobe.io/`, alle organen (huurders) waarvoor de huidige gebruikers systeembeheerder houden zijn vermeld. Als u hier de naam van de org niet vindt of u kunt geen toepassing voor een vereiste huurder hier tot stand brengen, gelieve te controleren of hebt u voldoende (systeembeheerder) rechten.

Er is één bekende kwestie op dit gebruikersinterface die voor om het even welke huurder slechts tien toepassingen zichtbaar zijn. Wanneer u de toepassing maakt, blijft u op die pagina en bladwijzer de URL. U hoeft niet naar de pagina met lijsten van de toepassing te gaan en de toepassing te zoeken die u hebt gemaakt. U kunt rechtstreeks op deze URL met bladwijzer drukken en de toepassing zo nodig bijwerken of verwijderen.

De JWT-toepassing wordt mogelijk niet correct vermeld. Daarom wordt aangeraden de URL bij het maken van een JWT-toepassing te noteren of een bladwijzer te maken.

## Het runnen van Configuratie houdt het werken op {#running-configuration-stops-working}

<!--
Comment Type: draft

<p>If the running configuration stops working, either of the following two possibilities
<g class="gr_ gr_15 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar multiReplace" data-gr-id="15" id="15" style="font-size: 12px;">
are
</g> there:</p>
<p>1.
<g class="gr_ gr_14 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="14" id="14">
Connection
</g> has failed, or</p>
<p>2. Publish has failed with permission to dam-replication-service denied, while connection has passed </p>
<p>If the connection has failed [1], the
<g class="gr_ gr_10 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling ins-del multiReplace" data-gr-id="10" id="10">
fail safe
</g> way to fix it is to <a href="../using/troubleshoot-parallel-publishing.md#main-pars-header-1664955658">clean up</a> the existing Brand Portal publish configuration and recreate a publish configuration. </p>
<p>However, if the
<g class="gr_ gr_18 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling" data-gr-id="18" id="18">
publish
</g> has failed with
<g class="gr_ gr_16 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="16" id="16">
permission
</g> denied to dam-replication-service, raise a support ticket.</p>
-->

Als een replicatieagent (die aan Brand Portal enkel fijn) publiceerde ophoudt verwerkend publiceert banen, controleer replicatielogboeken. Experience Manager heeft ingebouwde functie voor het automatisch opnieuw proberen van bestanden. Als de publicatie van een bepaald element mislukt, wordt dit automatisch opnieuw geprobeerd. Als er een probleem is dat soms voorkomt, zoals een netwerkfout, kan dit probleem tijdens het opnieuw proberen optreden.

Als er ononderbroken publicatiemislukkingen zijn en de rij wordt geblokkeerd, dan zou u **[!UICONTROL test connection]** moeten controleren en proberen om de fouten op te lossen die worden gemeld.

Op basis van de fouten wordt u aangeraden een ondersteuningsticket te registreren, zodat het technische team van Brand Portal u kan helpen problemen op te lossen.


## Replicatieagents configureren om een time-outfout voor de verbinding te voorkomen {#connection-timeout}

Doorgaans mislukt de publicatietaak met een time-outfout als er meerdere aanvragen in behandeling zijn in de replicatiestoets. Om deze kwestie op te lossen, zorg ervoor dat de replicatieagenten worden gevormd om onderbreking te vermijden.

Om de replicatieagenten te vormen:

1. Meld u aan bij de AEM Assets-auteur.
1. Navigeer in het deelvenster **Gereedschappen** naar **[!UICONTROL Deployment]** > **[!UICONTROL Replication]**.
1. Klik op **[!UICONTROL Agents on author]** op de pagina Replicatie. U kunt de vier replicatieagenten van uw huurder van Brand Portal zien.
1. Klik de replicatieagent URL en klik **[!UICONTROL Edit]**.
1. Klik in Agent-instellingen op het tabblad **[!UICONTROL Extended]**.
1. Schakel het selectievakje **[!UICONTROL Close Connection]** in.
1. Herhaal stap 4 door 7 om alle vier replicatieagenten te vormen.
1. Start de server opnieuw.
