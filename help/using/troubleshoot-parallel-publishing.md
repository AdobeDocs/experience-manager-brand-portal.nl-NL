---
title: Problemen met parallelle publicatie naar Brand Portal oplossen
seo-title: Problemen met parallelle publicatie naar Brand Portal oplossen
description: Los parallel publiceren problemen op.
seo-description: Los parallel publiceren problemen op.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---


# Problemen met parallelle publicatie naar Brand Portal oplossen {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Het Portaal van het merk wordt gevormd met AEM Assets om goedgekeurde merkactiva te hebben foutloos ingebed (of gepubliceerd) van de schrijverinstantie van AEM Assets. Zodra [gevormd](../using/configure-aem-assets-with-brand-portal.md), gebruikt AEM Author een replicatieagent om de geselecteerde activa aan de dienst van de Poortwolk van het Merk te herhalen voor goedgekeurd gebruik door Poortgebruikers van het Merk. De veelvoudige replicatieagenten worden gebruikt AEM 6.2 SP1-GFP5, AEM GFP 6.3.0.2, en verder om hoge snelheid parallelle publicatie toe te staan.

>[!NOTE]
>
>Adobe raadt u aan een upgrade naar AEM 6.4.1.0 uit te voeren om ervoor te zorgen dat AEM Assets Brand Portal correct is geconfigureerd met AEM Assets. Een beperking in AEM 6.4 geeft een fout terwijl het vormen van AEM Assets met het Portaal van het Merk en de replicatie ontbreekt.

Bij het configureren van de cloudservice voor merkportal onder **[!UICONTROL /etc/cloudservice]**, worden alle benodigde gebruikers en token automatisch gegenereerd en opgeslagen in de opslagplaats. De de dienstconfiguratie van de wolk wordt gecreeerd, worden de de dienstgebruikers die voor replicatie en replicatieagenten worden vereist om inhoud te herhalen ook gecreeerd. Dit leidt tot vier replicatieagenten. Dus wanneer u een groot aantal middelen van AEM naar Brand Portal publiceert, worden deze in de wachtrij geplaatst en verdeeld onder deze replicatieagents via Round Robin.

Nochtans, kan het publiceren met tussenpozen als gevolg van grote sling banen, verhoogd Netwerk en **[!UICONTROL Disk I/O]** op instantie van AEM Author ontbreken, of vertraagde prestaties van instantie AEM Author. Daarom wordt aangeraden de verbinding met de replicatieagent(en) te testen voordat met publiceren wordt begonnen.

![](assets/test-connection.png)

## Problemen met eerste publicatie oplossen: valideren, uw publicatieconfiguratie {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

Uw publicatieconfiguraties valideren:

1. De foutenlogboeken controleren
1. Controleren of de replicatieagent is gemaakt
1. Verbinding testen

**Logboeken bijhouden tijdens het maken van Cloud Service**

Logboeken van staarten controleren. Controleer of de replicatieagent is gemaakt of niet. Als het maken van de replicatieagent mislukt, bewerkt u de cloudservice door kleine wijzigingen aan te brengen in de cloudservice. Valideer en controleer opnieuw of de replicatieagent wordt gecreeerd of niet. Als dat niet het geval is, bewerkt u de service opnieuw.

Als bij herhaaldelijk het uitgeven van de wolkendienst het niet behoorlijk wordt gevormd, rapporteer een dagzorgkaartje.

**Verbinding met replicatieagents testen**

Logboek van de mening, als de fouten in replicatielogboek worden gevonden:

1. Neem contact op met de Technische Ondersteuning van Adobe.

1. Opnieuw [opschonen](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) en opnieuw publicatieconfiguratie maken.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### Bestaande Brand Portal-publicatieconfiguraties opschonen {#clean-up-existing-config}

De meeste keren dat publiceren niet werkt, kan de reden zijn dat de gebruiker die publiceert (bijvoorbeeld: `mac-<tenantid>-replication` heeft niet de recentste privé sleutel, en vandaar publiceert ontbreekt met &quot;401 onbevoegde&quot;fout en geen andere fout wordt gemeld in de logboeken van de replicatieagent. U zou het oplossen van problemen kunnen willen vermijden en een nieuwe configuratie in plaats daarvan tot stand brengen. Voor de nieuwe configuratie werkt behoorlijk, schrap omhoog het volgende van auteur AEM opstelling:

1. Ga naar `localhost:4502/crx/de/` (als u de auteurinstantie op localhost wilt uitvoeren:4502:\
   i. schrapping `/etc/replication/agents.author/mp_replication`ii. delete 
`/etc/cloudservices/mediaportal/<config_name>`

1. Ga naar localhost:4502/useradmin:\
   i. zoeken naar gebruiker `mac-<tenantid>replication`ii. deze gebruiker verwijderen

Nu is het systeem helemaal opgeruimd. Nu kunt u proberen tot een nieuwe cloudservice config te leiden en nog steeds de reeds bestaande JWT toepassing in [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/)gebruiken. Er is geen behoefte om een nieuwe toepassing tot stand te brengen, eerder enkel moet de openbare sleutel van de pas gecreëerde wolkenconfig worden bijgewerkt.

## Zichtbaarheid ontwikkelaarsleider JWT-toepassing {#developer-connection-jwt-application-tenant-visibility-issue}

Als op [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/), alle organen (huurders) waarvoor de huidige gebruikers systeembeheerder houden zijn vermeld. Als u hier de naam van de org niet vindt of u kunt geen toepassing voor een vereiste huurder hier tot stand brengen, gelieve te controleren of hebt u voldoende (systeembeheerder) rechten om dit te doen.

Er is één bekende kwestie op dit gebruikersinterface dat voor om het even welke huurder slechts top 10 toepassingen zichtbaar zijn. Wanneer u de toepassing maakt, blijft u op die pagina en bladwijzer de URL. U hoeft niet naar de pagina met lijsten van de toepassing te gaan en de toepassing te zoeken die u hebt gemaakt. U kunt rechtstreeks op deze URL met bladwijzer drukken en de toepassing zo nodig bijwerken of verwijderen.

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

Als een replicatieagent (die aan merkportaal enkel fijn) publiceert ophoudt verwerkend publicatietaken, controleer replicatielogboeken. AEM heeft ingebouwde auto-retry ingebouwde, zodat als een bepaald middel publiceren ontbreekt, wordt het opnieuw geprobeerd automatisch. Als er een probleem is dat soms voorkomt, zoals een netwerkfout, kan dit probleem tijdens het opnieuw proberen optreden.

Als er ononderbroken publicatiemislukkingen zijn en de rij wordt geblokkeerd, dan zou u moeten controleren **[!UICONTROL test connection]** en proberen om de fouten op te lossen die worden gemeld.

Gebaseerd op de fouten, wordt u geadviseerd om een steunkaartje te registreren, zodat het de technische team van het Portaal van het Merk u kan helpen kwesties oplossen.


## Replicatieagents configureren om een time-outfout voor de verbinding te voorkomen {#connection-timeout}

**Probleem**: Ik kan geen middelen van AEM Assets publiceren naar Brand Portal. Het replicatielogboek verklaart dat de verbinding uit timed.

**Resolutie**: Meestal mislukt het publiceren met een time-out-fout als er meerdere aanvragen in behandeling zijn in de replicatiewachtrij. Om de kwestie op te lossen, zorg ervoor dat de replicatieagenten worden gevormd om onderbreking te vermijden.

Voer de volgende stappen uit om de replicatieagent te vormen:
1. Meld u aan bij de auteur-instantie van uw AEM Assets.
1. From the **Tools** panel, navigate to **[!UICONTROL Deployment]** > **[!UICONTROL Replication]**.
1. Klik op de pagina Replicatie **[!UICONTROL Agents on author]**. U kunt de vier replicatieagenten voor uw Poorthuurder van het Merk zien.
1. Klik de replicatieagent URL om de agentendetails te openen.
1. Klik **[!UICONTROL Edit]** om de montages van de replicatieagent te wijzigen.
1. Klik in Agent-instellingen op het **[!UICONTROL Extended]** tabblad.
1. Schakel het **[!UICONTROL Close Connection]** selectievakje in.
1. Herhaal stap 4 door 7 om alle vier replicatieagenten te vormen.
1. Start de server opnieuw.