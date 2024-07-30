---
title: Problemen met parallelle publicatie naar Brand Portal oplossen
description: Los parallel publiceren problemen op.
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
role: Admin
exl-id: 631beabc-b145-49ba-a8e4-f301497be6da
source-git-commit: ce3a7a5232f32c86b4930f9079bed5f04d001d8f
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 0%

---

# Problemen met parallelle publicatie naar Brand Portal oplossen {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal is geconfigureerd met Experience Manager Assets om goedgekeurde merkmiddelen naadloos in te nemen (of te publiceren) vanuit de Experience Manager Assets-auteur-instantie. Zodra [ gevormd ](../using/configure-aem-assets-with-brand-portal.md), gebruikt de Auteur van de Experience Manager een replicatieagent om één of meerdere geselecteerde activa aan de wolkendienst van Brand Portal voor goedgekeurd gebruik door de gebruikers van Brand Portal te herhalen. De veelvoudige replicatieagenten worden gebruikt Experience Manager 6.2 SP1-GFP5, Experience Manager GFP 6.3.0.2, en verder om hoge snelheidsparallelle publicatie toe te staan.

>[!NOTE]
>
>Adobe raadt aan een upgrade naar Experience Manager 6.4.1.0 uit te voeren om de configuratie van Experience Manager Assets Brand Portal met Experience Manager Assets te voltooien. Een beperking in Experience Manager 6.4 geeft een fout terwijl het vormen van Experience Manager Assets met Brand Portal en replicatie ontbreekt.

Als u een cloudservice voor Brand Portal configureert onder **[!UICONTROL /etc/cloudservice]** , worden alle benodigde gebruikers en token automatisch gegenereerd en opgeslagen in de opslagplaats. De de dienstconfiguratie van de wolk wordt gecreeerd, worden de de dienstgebruikers die voor replicatie en replicatieagenten worden vereist om inhoud te herhalen ook gecreeerd. Het leidt tot vier replicatieagenten. Dus wanneer u een groot aantal middelen publiceert van Experience Manager naar Brand Portal, worden de elementen in een wachtrij geplaatst en verdeeld onder de replicatieagents via Round Robin.

Publiceren kan echter soms mislukken als gevolg van grote slingertaken, een verhoogd netwerk en **[!UICONTROL Disk I/O]** op een Experience Manager Author-instantie of trage prestaties van de Experience Manager Author-instantie. De Adobe adviseert testend de verbinding met één of meerdere replicatieagenten alvorens u begint te publiceren.

![](assets/test-connection.png)

## Problemen oplossen bij eerste publicatie: uw publicatieconfiguratie valideren {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

Uw publicatieconfiguraties valideren:

1. De foutenlogboeken controleren
1. Controleren of de replicatieagent is gemaakt
1. Verbinding testen

**Logboeken van het Lusje terwijl het creëren van Cloud Service**

Logboeken van staarten controleren. Controleer of de replicatieagent is gemaakt of niet. Als het maken van de replicatieagent mislukt, bewerkt u de Cloud-service door kleine wijzigingen aan te brengen in de Cloud-service. Valideer en controleer opnieuw of de replicatieagent wordt gecreeerd of niet. Als dat niet het geval is, bewerkt u de service opnieuw.

Als bij herhaaldelijk het uitgeven van de wolkendienst het niet behoorlijk wordt gevormd, rapporteer een kaartje van de Daycare.

**Verbinding van de Test met replicatieagenten**

Logboek van de mening, als de fouten in het replicatielogboek worden gevonden:

1. Neem contact op met de Klantenondersteuning.

1. Opnieuw [ schoonmaakbeurt ](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) en creeer opnieuw publiceer configuratie.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

## Bestaande Brand Portal-publicatieconfiguraties opschonen {#clean-up-existing-config}

Het publiceren ontbreekt vaak met een &quot;401 onbevoegde&quot;fout omdat de gebruiker (bijvoorbeeld, `mac-<tenantid>-replication`) de recentste privé sleutel mist, en geen andere fout wordt gemeld in de logboeken van de replicatieagent. U zou het oplossen van problemen kunnen willen vermijden en een configuratie in plaats daarvan tot stand brengen. Voor de nieuwe configuratie om behoorlijk te werken, schoonmaak het volgende van de opstelling van de auteur van de Experience Manager:

1. Ga naar `localhost:4502/crx/de/` (aangezien u de auteurinstantie uitvoert op `localhost:4502:`)
i. Verwijderen `/etc/replication/agents.author/mp_replication`
ii. Verwijderen `/etc/cloudservices/mediaportal/<config_name>`

1. Ga naar localhost:4502/useradmin:\
   i. Zoeken naar gebruiker `mac-<tenantid>replication`
ii. Deze gebruiker verwijderen

Nu is het systeem helemaal opgeruimd. Nu, kunt u proberen om een de dienstconfig van de wolk tot stand te brengen en nog de bestaande toepassing van JWT te gebruiken. U hoeft geen toepassing te maken, u hoeft de openbare sleutel niet bij te werken vanuit de nieuwe cloudconfiguratie.

>[!NOTE]
>
>Wijzig geen automatisch gegenereerde instellingen.


## Zichtbaarheid ontwikkelaarsleider JWT-toepassing {#developer-connection-jwt-application-tenant-visibility-issue}

Indien ingeschakeld `https://legacy-oauth.cloud.adobe.io/` , worden alle organen (huurders) vermeld waarvoor de huidige gebruikers de systeembeheerder aanhouden. Als u de naam van de org hier niet vindt of u kunt geen toepassing voor een vereiste huurder hier tot stand brengen, gelieve te controleren of hebt u voldoende (systeembeheerder) rechten.

Er is één bekende kwestie op dit gebruikersinterface dat voor om het even welke huurder, slechts de top tien toepassingen zichtbaar zijn. Wanneer u de toepassing maakt, blijft u op die pagina en bladwijzer de URL. Ga niet naar de pagina met lijsten van de toepassing en zoek de toepassing die u hebt gemaakt. U kunt rechtstreeks op deze URL met bladwijzer drukken en de toepassing bijwerken of verwijderen wanneer dat nodig is.

De JWT-toepassing wordt mogelijk niet correct vermeld. Daarom wordt u aangeraden een URL op te nemen of een bladwijzer te maken wanneer u een JWT-toepassing maakt.

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

Als een replicatieagent (die aan Brand Portal enkel fijn) publiceerde ophoudt verwerkend publiceert banen, controleer replicatielogboeken. Experience Manager heeft ingebouwde functie voor het automatisch opnieuw proberen van bestanden. Als de publicatie van een bepaald element mislukt, wordt dit automatisch opnieuw geprobeerd. Als er een probleem is dat soms voorkomt, zoals een netwerkfout, kan het probleem tijdens een nieuwe poging optreden.

Als er voortdurend publicatiefouten optreden en de wachtrij wordt geblokkeerd, controleert u **[!UICONTROL test connection]** . Probeer de fouten op te lossen die worden gerapporteerd.

Op basis van de fouten wordt u aangeraden een ondersteuningsticket te registreren, zodat het technische team van Brand Portal u kan helpen de problemen op te lossen.

## Brand Portal IMS-configuratietoken verlopen {#token-expired}

Als uw Brand Portal-omgeving abrupt stopt, is het mogelijk dat de IMS-configuraties niet goed werken. Het systeem toont een ongezonde configuratie IMS en wijst op een foutenmelding (gelijkend op het volgende) dat uw toegangstoken is verlopen.

`com.adobe.granite.auth.oauth.AccessTokenProvider failed to get access token from authorization server status: 400 response: Unknown macro: {"error"}`

Om dit probleem op te lossen, raadt de Adobe u aan de IMS-configuratie handmatig op te slaan en te sluiten en de status van de computer opnieuw te controleren. Als de configuraties niet werken, verwijdert u de bestaande configuraties en maakt u een nieuwe.


## Replicatieagents configureren om een time-outfout voor de verbinding te voorkomen {#connection-timeout}

Doorgaans mislukt de publicatietaak met een time-outfout als er meerdere aanvragen in behandeling zijn in de replicatiestoets. Om deze kwestie op te lossen, zorg ervoor dat de replicatieagenten worden gevormd om onderbreking te vermijden.

Om de replicatieagenten te vormen:

1. Meld u aan bij de AEM Assets-auteur.
1. Van het **paneel van Hulpmiddelen**, navigeer aan **[!UICONTROL Deployment]** > **[!UICONTROL Replication]**.
1. Klik op **[!UICONTROL `Agents on author`]** op de pagina Replicatie. U kunt de vier replicatieagenten van uw huurder van Brand Portal zien.
1. Klik op de URL van de replicatieagent en klik op **[!UICONTROL Edit]** .
1. Klik in Agent-instellingen op de tab **[!UICONTROL Extended]** .
1. Schakel het selectievakje **[!UICONTROL Close Connection]** in.
1. Herhaal stap 4 door 7 om alle vier replicatieagenten te vormen.
1. Start de server opnieuw.
