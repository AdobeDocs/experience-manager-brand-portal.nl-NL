---
title: Nieuw in AEM Assets Brand Portal
seo-title: Nieuw in AEM Assets Brand Portal
description: Bekijk de nieuwe functies en verbeteringen voor 6.4.7.
seo-description: Bekijk de nieuwe functies en verbeteringen voor 6.4.7.
uuid: 2c59d738-9b53-4f25-a205-13bf75c80b77
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: introduction
discoiquuid: fec32ca3-142b-4a11-9b92-5113fc27277a
translation-type: tm+mt
source-git-commit: d06381d84c70ab1566ac40c825233577de40af87
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Nieuw in AEM Assets Brand Portal {#what-s-new-in-aem-assets-brand-portal}

Met Adobe Experience Manager (AEM) Assets Brand Portal kunt u eenvoudig goedgekeurde creatieve middelen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten. Het draagt bij tot een efficiëntere verdeling van activa, versnelt de marktintroductie van activa en vermindert het risico van niet-naleving en ongeoorloofde toegang. Adobe werkt aan een verbetering van de algemene ervaring van het Brand Portal. Hier is een blik in de nieuwe eigenschappen en verhogingen.

## Wat veranderde in 6.4.7 {#what-changed-in-647}

De release van Brand Portal 6.4.7 introduceert de documentviewer, verbetert de ervaring voor het downloaden van middelen en bevat belangrijke correcties. Zie Opmerkingen bij de release van de nieuwste [Brand Portal](brand-portal-release-notes.md).

<!--
Brand Portal 6.4.7 release brings in the Document Viewer, leverages the Brand Portal administrators to configure asset download, and centers top customer requests. See latest [Brand Portal Release Notes](brand-portal-release-notes.md).
-->

### Documentviewer {#doc-viewer}

De documentviewer verbetert de weergave van PDF&#39;s. Deze app biedt een vergelijkbare ervaring als de Adobe Document Cloud bij het bekijken van de PDF-bestanden in Brand Portal.

Eerder waren er beperkte opties beschikbaar om de PDF-bestanden te bekijken.

Met Document Viewer hebben de gebruikers van de Brand Portal nu de opties om pagina&#39;s weer te geven, bladwijzers weer te geven, op pagina te zoeken, in te zoomen, uit te zoomen, naar vorige en volgende pagina&#39;s te navigeren, naar pagina te schakelen, aan venster te passen, op scherm te passen en de werkbalk te verbergen of te verbergen.

>[!NOTE]
>
>De ervaring met het weergeven van andere documentindelingen blijft ongewijzigd.



![](assets/doc-viewer.png)

### Downloadervaring {#download-configurations}

Het proces voor het downloaden van bedrijfsmiddelen is vernieuwd en biedt een eenvoudige gebruikerservaring bij het [downloaden van bedrijfsmiddelen van Brand Portal](brand-portal-download-assets.md).

De bestaande workflow voor het downloaden van middelen van het Brand Portal wordt onvermijdelijk gevolgd door het verschijnen van een **[!UICONTROL Download]** dialoogvenster met meerdere downloadopties waaruit u kunt kiezen.

In het Portaal van het Merk 6.4.7, kunnen de beheerders van het Portaal van het Merk de activa **[!UICONTROL Download]** montages vormen. De beschikbare configuraties zijn:
* **[!UICONTROL Fast Download]**
* **[!UICONTROL Custom Renditions]**
* **[!UICONTROL System Renditions]**

De beheerder van het Portaal van het Merk kan om het even welke combinatie toelaten om activadownload te vormen.

<!--In Brand Portal 6.4.7, fast download, custom renditions, and system renditions are the three configurations available.-->

* Als zowel **[!UICONTROL Custom Renditions]** als **[!UICONTROL System Renditions]** configuraties zijn uitgeschakeld, worden de oorspronkelijke uitvoeringen van de elementen gedownload zonder extra dialoogvenster dat het downloaden voor de gebruikers van de Brand Portal vereenvoudigt.

* Als een van de elementen **[!UICONTROL Custom Rendition]** of **[!UICONTROL System Rendition]** is ingeschakeld, wordt het **[!UICONTROL Download]** dialoogvenster weergegeven en worden het oorspronkelijke element en de elementvertoningen gedownload. Het inschakelen van **[!UICONTROL Fast Download]** configuratie versnelt het downloadproces.

Gebaseerd op de configuratie, blijft het downloadwerkschema constant voor stand-alone activa, veelvoudige activa, omslagen die activa, vergunning of unlicensed activa bevatten, en het downloaden van activa gebruikend aandeelverbinding.

![](assets/download-configuration.png)


## Wat veranderde in 6.4.6 {#what-changed-in-646}

In Brand Portal 6.4.6 wordt het machtigingskanaal tussen AEM Assets en Brand Portal gewijzigd. Brand Portal wordt nu ondersteund op AEM Assets als Cloud Service, AEM Assets 6.3 en hoger. In AEM Assets 6.3 en hoger werd het Brand Portal eerder geconfigureerd in de klassieke gebruikersinterface via Legacy OAuth Gateway, die de JWT-tokenuitwisseling gebruikt om een IMS Access-token voor verificatie te verkrijgen. AEM Assets is nu geconfigureerd met het Brand Portal via de Adobe Developer Console, die een IMS-token aanschaft voor toestemming van uw Poortmedewerker.

<!-- The steps to configure integration are different depending on your AEM version, and whether you are configuring for the first-time, or upgrading the existing integration:
-->

<!--
  
   | **AEM Version** |**New Integration** |**Upgrade Integration** |
|---|---|---|
| **AEM 6.5** |[Create new integration](../using/brand-portal-configure-integration-65.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4** |[Create new integration](../using/brand-portal-configure-integration-64.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3** |[Create new integration](../using/brand-portal-configure-integration-63.md) |[Upgrade existing integration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 

   -->

De stappen voor het configureren van AEM Assets met Brand Portal verschillen afhankelijk van uw AEM versie en of u voor het eerst configureert of de bestaande configuraties bijwerkt:

<!--| **AEM Version** |**New Configuration** |**Upgrade Configuration** |
|---|---|---|
| **AEM 6.5 (6.5.4.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-65.md) |[Upgrade configuration](../using/brand-portal-configure-integration-65.md#upgrade-integration-65) | 
| **AEM 6.4 (6.4.8.0 and above)** |[Create configuration](../using/brand-portal-configure-integration-64.md) |[Upgrade configuration](../using/brand-portal-configure-integration-64.md#upgrade-integration-64) | 
| **AEM 6.3 (6.3.3.8 and above)** |[Create configuration](../using/brand-portal-configure-integration-63.md) |[Upgrade configuration](../using/brand-portal-configure-integration-63.md#upgrade-integration-63) | 
| **AEM 6.2** |Contact Support |Contact Support | 
-->


<!-- AEM Assets configuration with Brand Portal on Adobe I/O is supported on:
* AEM 6.5.4.0 and above
* AEM 6.4.8.0 and above
* AEM 6.3.3.8 and above -->

| **AEM** | **Nieuwe configuratie** | **Upgradeconfiguratie** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 en hoger)** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgradeconfiguratie](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 en hoger)** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgradeconfiguratie](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 en hoger)** | [Configuratie maken](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Upgradeconfiguratie](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6,2** | Contact opnemen met ondersteuning | Contact opnemen met ondersteuning |

>[!NOTE]
>
>Het wordt aanbevolen uw AEM-exemplaar bij te werken naar het nieuwste servicepakket.

Zie Opmerkingen bij de release van de nieuwste [Brand Portal](brand-portal-release-notes.md).

Zie Veelgestelde vragen over [Brand Portal](brand-portal-faqs.md).

## Wat veranderde in 6.4.5 {#what-changed-in-645}


Brand Portal 6.4.5 is een functieversie die zich richt op het bieden van gebruikers van het Brand Portal (externe agentschappen/teams) de mogelijkheid om inhoud te uploaden naar het Brand Portal en deze te publiceren naar AEM Assets, zonder dat toegang nodig is tot de auteursomgeving. Deze functie wordt **[Asset Sourcing genoemd in Brand Portal](brand-portal-asset-sourcing.md)**, en zal klantenervaringen verbeteren door een mechanisme in twee richtingen voor gebruikers te verstrekken om activa zowel bij te dragen als te delen met andere wereldwijd verspreide gebruikers van het Portaal van het Merk.

### Asset Sourting in Brand Portal {#asset-sourcing-in-bp}

Met Asset Sourcing kunnen AEM gebruikers (beheerders/gebruikers die geen beheerder zijn) nieuwe mappen maken met een extra eigenschap voor **Asset Contribution** . Hierdoor wordt de nieuwe map opengesteld voor het verzenden van bedrijfsmiddelen door gebruikers van Brand Portal. Hierdoor wordt automatisch een workflow geactiveerd die twee extra submappen, NEW en SHARED, maakt in de nieuwe map **Contribution** .

De AEM gebruiker bepaalt dan het vereiste door een kort [overzicht van de soorten activa te](brand-portal-configure-contribution-folder-properties.md) uploaden die aan de bijdrageomslag moeten worden toegevoegd, evenals basislijnactiva [te](brand-portal-upload-baseline-assets.md)uploaden, aan de **GEDEELDE** omslag om BP gebruikers te verzekeren hebben de verwijzingsinformatie zij nodig hebben. De beheerder kan actieve gebruikers van het Brand Portal dan toegang tot de bijdrageomslag verlenen alvorens de pas gecreëerde omslag van de **Bijdrage** aan het Portaal van het Merk te publiceren.


Als de gebruiker klaar is met het toevoegen van inhoud in de map **NEW** , kan hij of zij de map met de bijdrage weer publiceren naar de AEM auteuromgeving. Het kan enkele minuten duren voordat de import is voltooid en de nieuw gepubliceerde inhoud in AEM Assets wordt weerspiegeld.

Bovendien blijft alle bestaande functionaliteit ongewijzigd. Gebruikers van het Brand Portal kunnen middelen weergeven, zoeken en downloaden vanuit de bijdragemap en vanuit de andere toegestane mappen. En beheerders kunnen de bijdragemap verder delen, eigenschappen wijzigen en elementen toevoegen aan verzamelingen.

>[!NOTE]
>
>Asset Sourcing in Brand Portal wordt ondersteund op AEM 6.5.2.0 en hoger.
>
>De functie wordt niet ondersteund in de eerdere versies - AEM 6.3 en AEM 6.4.

### Elementen uploaden naar de bijdragemap {#upload-assets-in-bp}

De gebruikers van het Portaal van het merk met aangewezen toestemmingen kunnen de activa [downloaden vereisten](brand-portal-download-asset-requirements.md) om de behoefte te begrijpen en veelvoudige activa of omslagen te uploaden die veelvoudige activa bevatten aan de bijdrageomslag. Merk Portal-gebruikers kunnen echter alleen elementen uploaden naar de submap **NEW** . De map **SHARED** is bedoeld voor de verdeling van vereisten en basislijnelementen. Zie, Elementen [uploaden naar de bijdragemap](brand-portal-upload-assets-to-contribution-folder.md)

![](assets/upload-asset6.png)

![](assets/upload-asset4.png)


### Bijdragemap publiceren naar AEM Assets {#publish-assets-to-aem}

Wanneer het uploaden is voltooid naar de map **NEW** , kunnen gebruikers van Brand Portal de map met bijdragen weer publiceren naar AEM. Het kan enkele minuten duren om de gepubliceerde inhoud/middelen in AEM Assets te importeren en weer te geven. Zie [Contribute-map publiceren naar AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)


![](assets/upload-asset5.png)

## Wat veranderde in 6.4.4 {#what-changed-in-644}

Merk Portal 6.4.4 versie concentreert zich op verhogingen aan tekstonderzoek en hoogste klantenverzoeken. Zie Opmerkingen bij de release van de nieuwste [Brand Portal](brand-portal-release-notes.md).

### Verbeteringen voor zoeken {#search-enhancements}

Brand Portal 6.4.4 en hoger ondersteunt gedeeltelijk zoeken naar voorspelling van tekst in filtervenster. Als u gedeeltelijk zoeken in tekst wilt toestaan, moet u **Gedeeltelijk zoeken** in Voorspelling eigenschap in het zoekformulier inschakelen.

Lees verder voor meer informatie over gedeeltelijk zoeken naar tekst en zoeken naar jokertekens.

#### Gedeeltelijke woordzoekopdracht {#partial-phrase-search}

U kunt nu naar elementen zoeken door alleen een deel (dat een woord of twee is) van de gezochte woordgroep op te geven in het filtervenster.

**Het zoeken naar hoofdletters/kleine letters** is handig wanneer u niet zeker weet welke combinatie van woorden in de gezochte uitdrukking voorkomt.

Bijvoorbeeld, als uw onderzoeksvorm in het Portaal van het Merk de Voorkeur van het Bezit voor gedeeltelijke onderzoek op activa titel gebruikt, dan specificerend de term **kamp** keert alle activa met het woordkamp in hun titeluitdrukking terug.

![](assets/partialphrasesearch.png)

#### Zoekopdracht met jokertekens {#wildcard-search}

Het Brand Portal staat toe gebruikend de asterisk (*) in onderzoeksvraag samen met een deel van het woord in uw gezochte uitdrukking.

**Gebruik hoofdletters/kleine letters** als u niet precies weet welke woorden in de gezochte uitdrukking voorkomen, kunt u een zoekopdracht met jokertekens gebruiken om de tussenruimten in de zoekopdracht op te vullen.

Als u bijvoorbeeld **klimmen*** opgeeft, worden alle elementen geretourneerd met woorden die beginnen met de tekens die in de titelzin **klimmen** als in het zoekformulier in het Brand Portal Eigenschapvoorspelling wordt gebruikt voor gedeeltelijk zoeken naar de titel van de elementen.

![](assets/wildcard-prop.png)

Op dezelfde manier specificeren:

* ***klib** retourneert alle elementen met woorden die eindigen met tekens die in hun titelzin **klimmen** .

* ***klib*** retourneert alle elementen met woorden die bestaan uit de tekens die in hun titelzin **klimmen** .

>[!NOTE]
>
>Als u het selectievakje **Gedeeltelijk zoeken** inschakelt, is Hoofdlettergebruik **** negeren standaard ingeschakeld.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-searching.md#facetedsearchbyapplyingfilterstosearch)

## Wat veranderde in 6.4.3 {#what-changed-in}

Merk Portal 6.4.3 release richt zich op — organisaties een alternatieve alias ter beschikking stellen naast hun huurder-id in de toegangs-URL van het Brand Portal, nieuwe configuratie van de mappenhiërarchie, verbeteringen op het gebied van videoondersteuning, gepland publiceren van de AEM-auteur naar het Brand Portal, operationele verbeteringen en gaat in op verzoeken van klanten.

### Navigatie in maphiërarchie voor niet-beheerders

Beheerders kunnen nu configureren hoe de mappen bij het aanmelden worden weergegeven aan gebruikers zonder beheer (Editors, Viewers en Gastgebruikers). [Configuratie van maphiërarchie](../using/brand-portal-general-configuration.md) inschakelen wordt toegevoegd aan **Algemene instellingen** in het deelvenster met beheergereedschappen. Als de configuratie:

* **Als deze optie is ingeschakeld**, is de mappenstructuur die begint in de hoofdmap zichtbaar voor gebruikers zonder beheerdersrechten. Aldus, die hen een navigatie ervaring gelijkend op beheerders verlenen.
* **uitgeschakeld**, worden alleen de gedeelde mappen weergegeven op de bestemmingspagina.

![](assets/enable-folder-hierarchy.png)

Met de functie Maphiërarchie [](../using/brand-portal-general-configuration.md) inschakelen (indien ingeschakeld) kunt u de mappen onderscheiden met dezelfde namen die worden gedeeld vanuit verschillende hiërarchieën. Bij het aanmelden zien niet-beheerders nu de virtuele bovenliggende mappen (en vooroudermappen) van de gedeelde mappen.

![](assets/disabled-folder-hierarchy1-2.png)

![](assets/enabled-hierarchy1-2.png)

De gedeelde mappen worden in de desbetreffende directory&#39;s in virtuele mappen ingedeeld. U kunt deze virtuele mappen herkennen met een vergrendelingspictogram.

De standaardminiatuur van de virtuele mappen is de miniatuurafbeelding van de eerste gedeelde map.

![](assets/hierarchy1-nonadmin-2.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-general-configuration.md)

### Zoeken in specifieke maphiërarchie of pad

**Voorspelfunctie voor padbrowser** wordt geïntroduceerd in Zoekformulier om te kunnen zoeken naar elementen in een specifieke map. Het standaardzoekpad van zoekvoorspelling voor padbrowser is `/content/dam/mac/<tenant-id>/`, dat kan worden geconfigureerd door het standaardzoekformulier te bewerken.

* Admin-gebruikers kunnen met Padbrowser naar een willekeurige map op het Brand Portal navigeren.
* Gebruikers die geen beheerder zijn, kunnen de padbrowser gebruiken om alleen naar de mappen (en terug te navigeren naar de bovenliggende mappen) te navigeren die met hen worden gedeeld.

   Wordt bijvoorbeeld `/content/dam/mac/<tenant-id>/folderA/folderB/folderC` gedeeld met een gebruiker die geen beheerder is. De gebruiker kan naar elementen binnen folderC zoeken gebruikend Browser van de Weg. Deze gebruiker kan ook naar folderB en folderA navigeren (aangezien zij voorouders van folderC zijn die met de gebruiker wordt gedeeld).

![](assets/edit-search-form.png)

**Het gebruiksgeval**

U kunt nu het zoeken naar middelen beperken in een specifieke map waarnaar u hebt gebladerd, in plaats van te beginnen bij de hoofdmap.

Het zoeken onder deze mappen resulteert alleen uit de elementen die met de gebruiker zijn gedeeld.

![](assets/filter-panel.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal-search-facets.md#listofsearchpredicates)

### Ondersteuning voor dynamische media-video-uitvoeringen

Gebruikers van wie de AEM-auteur-instantie zich in de hybride modus Dynamische media bevindt, kunnen naast de originele videobestanden ook een voorvertoning van de dynamische media-uitvoeringen weergeven en deze downloaden.

Om voorproef en download van dynamische media vertoningen op specifieke huurdersrekeningen toe te staan, moeten de beheerders **Dynamische Configuratie** van Media (videodienst URL (DM-Gateway URL) en registratie identiteitskaart specificeren om de dynamische video) in de configuratie van de **Video** van het admin hulpmiddelenpaneel te halen.

**U kunt een voorvertoning weergeven van video&#39;s over het gebruiksscenario** Dynamic Media:

* Pagina met elementgegevens
* Weergave van de kaart van het element
* Voorvertoningspagina voor delen koppelen

Dynamische videocodes voor media kunnen worden gedownload van:

* Brand Portal
* Gedeelde koppeling

![](assets/edit-dynamic-media-config.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Gepland publiceren naar Brand Portal

De middelen (en de omslagen) publiceren werkschema van [AEM (6.4.2.0)](https://helpx.adobe.com/experience-manager/6-4/release-notes/sp-release-notes.html#main-pars_header_9658011) de instantie van de Auteur aan het Portaal van het Merk kan voor een recentere datum en een tijd worden gepland.

Op dezelfde manier kunnen gepubliceerde elementen op een latere datum (tijd) uit de portal worden verwijderd door de workflow Publiceren via Brand Portal te plannen.

![](assets/schedule-publish.png)
![](assets/publishlater-workflow.png)

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Configureerbare alias van huurder in URL

Organisaties kunnen hun portaal-URL aanpassen door een alternatief voorvoegsel in de URL te hebben. Om een alias voor huurdersnaam in hun bestaande portaal URL te krijgen, moeten de organisaties Adobe steun contacteren.

Merk op dat alleen het voorvoegsel van de Brand Portal-URL kan worden aangepast en niet de volledige URL.\
Zo kan een organisatie met bestaande domeingeomettrix. **brand-portal.adobe.com** op verzoek **geomettrixinc.brand-portal.adobe.com** maken.

Nochtans, kan de instantie van de Auteur AEM slechts met huurder identiteitskaart URL en niet met huurder alias (afwisselende) URL worden [gevormd](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) .

**De gebruikscase** Organisaties kunnen aan hun brandingbehoeften voldoen door de portaal-URL aan te passen in plaats van zich aan de URL van Adobe te houden.

[![](https://helpx.adobe.com/content/dam/help/en/experience-manager/brand-portal/images/see-the-guide.png)](../using/brand-portal.md#tenantaliasforportalurl)

### Verbeteringen in downloadervaring

De release biedt een vereenvoudigde downloadervaring met een beperkt aantal klikken en waarschuwingen, op:

* ervoor kiezen alleen de uitvoeringen (en niet de originele elementen) te downloaden.
* de elementen downloaden wanneer de toegang tot de oorspronkelijke uitvoeringen beperkt is.

## Wat veranderde in 6.4.2 {#what-changed-in-1}

De introductie van Brand Portal 6.4.2 biedt een aantal mogelijkheden om te voldoen aan de behoeften van organisaties op het gebied van middelendistributie en helpt hen om een groot aantal gebruikers te bereiken die wereldwijd via gasttoegang en optimale ervaring met versnelde downloads worden gedistribueerd. Het Portaal van het merk verstrekt ook grotere controle aan organisaties door nieuwe configuraties voor beheerders, onlangs toegevoegd rapport, en caters aan klantenverzoeken.

### Toegang voor gasten

![](assets/bp-login-screen-1.png)

AEM Brand-portaal biedt gasten toegang tot het portaal. Een gastgebruiker vereist geen geloofsbrieven om het portaal in te gaan en kan tot alle openbare omslagen en inzamelingen toegang hebben en downloaden. Gastgebruikers kunnen elementen toevoegen aan hun lichtbak (privéverzameling) en deze downloaden. Ze kunnen ook zoeken naar slimme tags en voorspelden van zoekopdrachten weergeven die door beheerders zijn ingesteld. De gastzitting staat gebruikers niet toe om inzamelingen tot stand te brengen en bewaarde onderzoeken of hen verder te delen, tot omslag en inzamelingsmontages toegang te hebben, en activa als verbindingen te delen.

In een organisatie zijn meerdere gelijktijdige gastsessies toegestaan, wat beperkt is tot 10% van de totale gebruikersquota per organisatie.

Een gastsessie blijft twee uur actief. Daarom wordt de staat van de lichtbak ook bewaard tot twee uur vanaf de tijd van het zittingsbegin. Na twee uur, moet de gastzitting opnieuw beginnen, zodat wordt de lichtbakstaat verloren.

### Versnelde downloads

Gebruikers van het Brand Portal kunnen gebruikmaken van snelle downloads op basis van IBM Aspera Connect om snelheden tot 25x sneller te kunnen gebruiken en genieten van een naadloze downloadervaring, ongeacht hun locatie over de hele wereld. Als gebruikers de elementen sneller van Brand Portal of de gedeelde koppeling willen downloaden, moeten ze de optie Downloadversnelling **** inschakelen selecteren in het dialoogvenster Downloaden, mits downloadversnelling is ingeschakeld in hun organisatie.

![](assets/donload-assets-dialog-2.png)

Om versneld downloaden op basis van IBM Aspera voor de organisatie in te schakelen, **schakelen beheerders de optie Downloadversnelling** (die standaard is uitgeschakeld) in bij [Algemene instellingen](brand-portal-general-configuration.md#allow-download-acceleration) in het deelvenster met beheergereedschappen. Raadpleeg [Guide voor snellere downloads vanaf Brand Portal](../using/accelerated-download.md#main-pars-header)voor meer informatie over vereisten en stappen voor het oplossen van problemen waarmee elementbestanden sneller kunnen worden gedownload van Brand Portal en gedeelde koppelingen.

### Rapport voor gebruikersaanmelding

Er is een nieuw rapport geïntroduceerd om gebruikersaanmeldingen bij te houden. Het rapport **Gebruikersaanmelding** kan nuttig zijn om organisaties in staat te stellen een controle uit te voeren en te houden op de gedelegeerde beheerders en andere gebruikers van het Brand Portal.

De rapportlogboeken tonen namen, e-mail IDs, persona&#39;s (admin, kijker, redacteur, gast), groepen, laatste login, activiteitenstatus, en login telling van elke gebruiker van Poort 6.4.2 plaatsing van het Merk tot de tijd van rapportgeneratie. De beheerders kunnen het rapport als .csv uitvoeren. Samen met andere rapporten, laat het rapport van Logins van de Gebruiker organisaties toe om gebruikersinteractie met de goedgekeurde merkmiddelen beter te controleren, daardoor ervoor zorgend conformiteit aan collectieve nalevingsbureaus.

![](assets/user-logins-1.png)

### Toegang tot oorspronkelijke vertoningen

Beheerders kunnen de gebruikerstoegang tot originele afbeeldingsbestanden (.jpeg, .tiff, .png, .bmp, .gif, .pjpeg, x-portable-anymap, x-portable-bitmap, x-portable-graymap, x-portable-pixmap, x-rgb, x-xbitmap, x-xpixmap, x-icon, image/photoshop, image/x-photoshop, .psd, image/vnd.adobe.photoshop) en geeft toegang tot vertoningen met lage resolutie die zij van het Portaal van het Merk of gedeelde verbinding downloaden. Deze toegang kan op het niveau van de gebruikersgroep van het lusje van Groepen van de pagina van Rollen van de Gebruiker in het paneel van Admin hulpmiddelen worden gecontroleerd.

![](assets/access-original-rend-1.png)

* Standaard kunnen alle gebruikers de originele uitvoeringen downloaden, omdat de optie Toegang tot origineel voor iedereen is ingeschakeld.
* Beheerders moeten de selectie van de desbetreffende selectievakjes opheffen om te voorkomen dat een groep gebruikers toegang krijgt tot de oorspronkelijke uitvoeringen.
* Als een gebruiker lid is van meerdere groepen, maar slechts één van de groepen heeft beperkingen, gelden de beperkingen voor die gebruiker.
* De beperkingen zijn niet van toepassing op beheerders, ook al zijn zij lid van beperkte groepen.
* Rechten van de gebruiker die elementen deelt als koppeling zijn van toepassing op de gebruikers die elementen downloaden via gedeelde koppelingen.

### Pad met maphiërarchie op kaart- en lijstweergaven

In de Kaarten van mappen wordt in de Kaartweergave nu informatie over de maphiërarchie weergegeven voor gebruikers die geen beheerder zijn (Editor, Viewer en gastgebruiker). Deze functionaliteit laat de gebruikers de plaats van de omslagen kennen, die zij, met betrekking tot de ouderhiërarchie toegang hebben.

Informatie over de maphiërarchie is vooral handig om onderscheid te maken tussen de mappen waarvan de namen overeenkomen met andere mappen die vanuit een andere maphiërarchie worden gedeeld. Als de gebruikers die geen beheerder zijn niet op de hoogte zijn van de mapstructuur van de elementen die met hen worden gedeeld, lijken elementen/mappen met vergelijkbare namen verwarrend.

* De paden die op de betreffende kaarten worden weergegeven, worden afgekapt om in de kaartgrootten te passen. Gebruikers kunnen het volledige pad echter zien als knopinfo bij het aanwijzen over het afgebroken pad.

![](assets/folder-hierarchy1-1.png)

De Mening van de lijst toont omslagWeg van activa in een kolom aan alle gebruikers van het Portaal van het Merk.

![](assets/list-view-1.png)

### Overzicht, optie om de eigenschappen van elementen weer te geven

Brand Portal biedt een overzichtsoptie voor gebruikers die geen beheerder zijn (Editors, Viewers, Gastgebruikers) om de eigenschappen van bedrijfsmiddelen van geselecteerde elementen/mappen weer te geven. De optie Overzicht is zichtbaar:

1. Selecteer bovenaan op de werkbalk een middel/map.
2. In de vervolgkeuzelijst selecteert u de spoorkiezer.

Als u de optie Overzicht selecteert terwijl een middel/map is geselecteerd, kunnen gebruikers de titel, het pad en het tijdstip van het maken van de elementen zien. Terwijl de gebruiker met de optie Overzicht op de pagina met elementdetails de metagegevens van het element kan bekijken.

![](assets/overview-option-2.png)

![](assets/overview-rail-selector-2.png)

## Nieuwe configuraties

Er worden zes nieuwe configuraties toegevoegd voor beheerders om de volgende functies in of uit te schakelen voor specifieke huurders:

* Toegang voor gasten toestaan
* Gebruikers toegang tot Brand Portal laten aanvragen
* Beheerders toestaan elementen te verwijderen uit Brand Portal
* Openbare collecties maken
* Maken van openbare slimme verzamelingen toestaan
* Downloadversnelling toestaan

De bovenstaande configuraties zijn beschikbaar onder Toegang en Algemene instellingen in het deelvenster met beheergereedschappen.

![](assets/access-configs-1.png)
![](assets/general-configs-1.png)
![](assets/admin-tools-panel-13.png)

### Adobe I/O UI om de Integraties van de Auth te vormen

Brand Portal 6.4.2 en hoger gebruikt de Adobe.io- [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/) -interface om JWT-toepassing te maken. Hierdoor kunnen Auth-integraties worden geconfigureerd om AEM Assets-integratie met Brand Portal mogelijk te maken. Eerder werd de interface voor het configureren van OAuth-integratie gehost in `https://marketing.adobe.com/developer/`. Meer informatie over het integreren van AEM Assets met Brand Portal voor het publiceren van middelen en verzamelingen naar Brand Portal vindt u in AEM Assets-integratie [configureren met Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html).

## Verbeteringen zoeken

Beheerders kunnen de eigenschap instellen dat niet-hoofdlettergevoelig wordt voorspeld door de bijgewerkte eigenschap predikaat te gebruiken, die een controle op Hoofdlettergebruik negeren heeft. Deze optie is beschikbaar voor de voorspelling van eigenschappen en eigenschappen met meerdere waarden.\
Nochtans, is het niet-hoofdlettergevoelige onderzoek relatief langzamer dan standaardonderzoek naar bezitspredikaat. Als het zoekfilter te veel niet-hoofdlettergevoelige voorspellingen bevat, kan de zoekopdracht vertragen. Daarom wordt het aanbevolen de niet-hoofdgevoelige zoekopdracht op oordeelkundige wijze te gebruiken.

## Wat veranderde in 6.4.1 {#what-changed-in-2}

Brand Portal 6.4.1 is een platform upgraderelease die verschillende nieuwe functies en essentiële verbeteringen bevat, zoals bladeren, zoeken en prestatieverbeteringen om een bevredigende klantervaring te bieden.

### Verbeteringen voor bladeren

* Nieuwe contentstructuurrails om snel door de hiërarchie van elementen te navigeren.

![](assets/contenttree-2.png)

* Nieuwe sneltoetsen geïntroduceerd, bijvoorbeeld _(p)_ voor navigatie naar eigenschappenpagina, _(e)_ voor Bewerken en _(ctrl+c)_ voor kopieerbewerkingen.
* Verbeterde schuifervaring, luie laadervaring in kaart- en lijstweergave voor het bladeren door een groot aantal elementen.
* Uitgebreide kaartweergave met ondersteuning voor kaarten van verschillende grootte op basis van weergave-instelling.

![](assets/cardviewsettings-1.png)

* In de kaartweergave wordt nu datum-/tijdstempel weergegeven wanneer u de muis boven het datumlabel plaatst.

* Verbeterde kolomweergave met **Meer details** onder de elementmomentopname, waarmee u naar de detailpagina van een element kunt navigeren.

![](assets/columnmoredetail.png)

* In de lijstweergave worden nu standaard de bestandsnamen van elementen in de eerste kolom weergegeven, naast de landinstelling, het type element, de afmetingen, de grootte, de classificatie en de publicatiegegevens. De nieuwe Montages **van de** Mening kunnen worden gebruikt om de hoeveelheid detail te vormen in de mening van de Lijst te tonen.

* Betere ervaring met middelendetails, omdat u met nieuwe navigatieknoppen heen en weer kunt navigeren tussen elementen en elementen kunt weergeven.

![](assets/navbtn.png)

* Nieuwe mogelijkheid om audiobestanden, geüpload vanaf AEM, voor te vertonen op de detailpagina van het element.
* New Related Assets capabilities provided in Asset properties. Activa die verwant zijn aan andere bron/afgeleide middelen op AEM en op Brand Portal worden gepubliceerd, hebben hun relatie nu intact in Brand Portal, met koppelingen naar de gerelateerde elementen op de eigenschappenpagina.
* Er is een nieuwe configuratie geïntroduceerd om te voorkomen dat gebruikers zonder beheerdersrechten openbare verzamelingen maken. Organisaties kunnen met het team van de Steun van Adobe samenwerken om dit vermogen op specifieke rekeningen te vormen.

### Verbeteringen voor zoeken

* Mogelijkheid geïntroduceerd om terug te keren naar dezelfde positie in zoekresultaten, na navigatie naar een zoekopdracht, zonder de zoekquery opnieuw uit te voeren.
* Er is een aantal nieuwe zoekresultaten opgegeven waarmee het aantal zoekresultaten wordt weergegeven.
* Het verbeterde filter van het Onderzoek van het Type van Dossier met de capaciteit om onderzoeksresultaten te filtreren die op verfijnde types MIME zoals .jpg, .png, en .psd worden gebaseerd in vergelijking met vroegere Beelden, Documenten, Multimedia opties.
* Verbeterde zoekfilters voor verzamelingen, met nauwkeurige tijdstempels in plaats van de vorige tijdschuifregelaar.
* De nieuwe het type van Toegang filters zijn geïntroduceerd om naar de inzamelingen te zoeken die openbaar of niet-Openbaar zijn.

![](assets/accesstypefilter.png)

### Optimalisaties downloaden

* Eén groot bestand wordt rechtstreeks gedownload, zonder dat er een ZIP-bestand wordt gemaakt. Hierdoor wordt de snelheid en de doorvoer verhoogd.
* De Zip-downloadlimiet voor de functie voor het delen van koppelingen is gestegen naar 5 GB, van 1 GB.

* Gebruikers kunnen nu alleen de aangepaste en originele bestanden downloaden en uitvoeringen buiten de box voorkomen tijdens het downloaden van elementen van het Brand Portal of via de functie voor gedeelde koppelingen.

![](assets/excludeautorendition.png)

### Prestatieverbeteringen

* Tot 100% betere downloadsnelheid voor middelen.
* Tot 40% verbetering in zoekactie voor middelen.
* Tot 40% betere bladerprestaties.

**Opmerking**: Bewegde verbeteringen zijn volgens de tests die in het laboratorium worden uitgevoerd.

### Verbeterde rapporteringsmogelijkheden

**Het geïntroduceerde Rapport van het Aandeel van de Verbinding** Een nieuw rapport, om informatie over gedeelde verbindingen te verstrekken, is geïntroduceerd. Het rapport van het Aandeel van de Verbinding maakt een lijst van alle URLs, aan de activa, die met interne en externe gebruikers over organisatie in het gespecificeerde tijdkader worden gedeeld. Het deelt ook wanneer de verbinding werd gedeeld, door wie, en wanneer het verlopen.

![](assets/navigatereport.png)

**Gewijzigd het ingangspunt voor toegang tot het rapport** van het Gebruik wordt nu geconsolideerd met andere rapporten en kan nu van de console van de Rapporten van Activa worden bekeken. Navigeer naar Rapporten **** maken/beheren vanuit het deelvenster met beheergereedschappen om de console voor Asset Reports te bereiken.

![](assets/accessassetreport.png)

**De verbeterde gebruikerservaring met het rapporteren** van de interface van de Rapportering op het Portaal van het Merk is intuïtiever geworden en geeft organisaties meer controle. Naast het maken van verschillende rapporten kunnen beheerders nu terugkeren naar de gegenereerde rapporten en deze downloaden of verwijderen, aangezien deze rapporten worden opgeslagen in Brand Portal.

Elk van de rapporten die kunnen worden gecreeerd worden aangepast door standaardkolommen toe te voegen of te verwijderen. Bovendien kunnen aangepaste kolommen worden toegevoegd aan de rapporten Downloaden, Verlopen en Publiceren om de mate van granulariteit van de kolommen te bepalen.

### Verbeterde beheerfuncties

Verbeterde eigenschappenkiezer in de beheerfuncties voor metagegevens, zoeken en rapporten met Type-ahead- en bladermogelijkheden om de beheerervaring te vereenvoudigen.

### Andere verbeteringen

* Middelen die vanuit AEM 6.3.2.1 en 6.4 naar Brand Portal zijn gepubliceerd, kunnen nu openbaar worden gemaakt voor algemene gebruikers van het Merkortaal door het selectievakje Openbare map publiceren in te schakelen in het dialoogvenster AEM Assets Merkorportreplicatie.

![](assets/public-folder-publish.png)

* Beheerders worden via e-mails met een verzoek om toegang op de hoogte gesteld, behalve de meldingen in het aanmeldingsgebied van het Brand Portal, als iemand toegang tot het Brand Portal heeft aangevraagd.

## Wat veranderde in 6.3.2 {#what-changed-in-3}

Brand Portal 6.3.2 bevat nieuwe en verbeterde functionaliteit die gericht is op de belangrijkste verzoeken van klanten en algemene prestatieverbeteringen.

### Toegang aanvragen tot Brand Portal {#request-access-to-brand-portal}

Gebruikers kunnen nu toegang tot het Brand Portal aanvragen met behulp van de nieuwe **vereiste toegangsmogelijkheden** die beschikbaar zijn op het aanmeldingsscherm van het Brand Portal.

![](assets/bplogin_request_access.png)

Afhankelijk van of gebruikers een Adobe ID hebben of een Adobe ID moeten maken, kunnen gebruikers de juiste workflow volgen om een aanvraag in te dienen. Merk Portal-productbeheerders ontvangen dergelijke verzoeken in hun aanmeldingsgebied en verlenen toegang via Adobe Admin Console.

Zie Toegang [aanvragen tot Brand Portal](../using/brand-portal.md#requestaccesstobrandportal)voor meer informatie.

### Verbetering in het rapport over gedownloade elementen {#enhancement-in-the-assets-downloaded-report}

Het gedownloade rapport voor elementen bevat nu het aantal gedownloade elementen per gebruiker binnen het opgegeven datum- en tijdbereik. Gebruikers kunnen dit rapport downloaden in de .csv-indeling en gegevens compileren, zoals het totale aantal downloads voor een onder licentie geplaatst element.

![](assets/reports_download_downloaded_by.png)

Voor meer informatie, zie Stap 3 en 6 in [creëren en leiden extra rapporten](../using/brand-portal-reports.md#createandmanageadditionalreports).

### Meldingen over onderhoud aan Brand Portal {#brand-portal-maintenance-notification}

Brand Portal geeft nu een meldingsbanner weer enkele dagen voor een aanstaande onderhoudsactiviteit. Een voorbeeldmelding:

![](assets/bp_maintenance_notification-1.png)

Voor meer informatie, zie [het onderhoudsbericht](https://helpx.adobe.com/experience-manager/brand-portal/using/brand-portal.html#BrandPortalmaintenancenotification)van het Portaal van het Merk.

### Verbetering voor gelicentieerde elementen die worden gedeeld met de functie voor het delen van koppelingen {#enhancement-for-licensed-assets-shared-using-the-link-share-feature}

Tijdens het downloaden van gelicentieerde middelen met de functie voor het delen van koppelingen, wordt u nu gevraagd akkoord te gaan met de licentieovereenkomst voor deze elementen.

![](assets/copyright_management.png)

Voor meer informatie, zie Stap 12 in de activa van het [Aandeel als verbinding](../using/brand-portal-link-share.md#shareassetsasalink).

### Verbetering van gebruikerenkiezer {#user-picker-enhancement}

De prestaties van de kiezer van de gebruiker worden nu verbeterd om tegemoet te komen aan de behoeften van klanten met een grote gebruikersbasis.

### Ervaar wijzigingen in cloud-branding {#experience-cloud-branding-changes}

Brand Portal voldoet nu aan de nieuwe Adobe Experience Cloud-merknaam.

![](assets/bp_solution_switcher.png)

## Wat veranderde in 6.3.1 {#what-changed-in-4}

Brand Portal 6.3.1 bevat nieuwe en verbeterde functionaliteit die gericht is op het uitlijnen van Brand Portal op AEM.

### Bijgewerkte gebruikersinterface {#upgraded-user-interface}

Als u de gebruikerservaring van Brand Portal wilt uitlijnen op AEM, gaat Adobe over naar de gebruikersinterface van Coral 3. Deze wijziging verbetert de algemene bruikbaarheid, waaronder navigatie en vormgeving.

#### Verbeterde navigatie-ervaring {#enhanced-navigational-experience}

* Snelle toegang tot administratieve hulpmiddelen door het nieuwe embleem van de Adobe:

![](assets/aemlogo-3.png)

* Productnavigatie door een overlay:

![](assets/overlay_navigation.png)

* Snelle navigatie naar bovenliggende mappen:

![](assets/navigationparentfolders.png)

* Snel zoeken en navigeren naar de vereiste inhoud en gereedschappen:

![](assets/omnisearchicon.png)

### Verbeterde bladerervaring {#enhanced-browsing-experience}

* Nieuwe kolomweergave om door geneste mappen te bladeren:

![](assets/millercolumnnavigation.png) ![](assets/multi-columnview.png)

* In de lijst met elementen in een map wordt bovenaan het laatst geüploade element weergegeven.

### Verbeterde zoekervaring {#enhanced-search-experience}

* Met de nieuwe zoekfunctie Universeel hebt u snel toegang tot relevante inhoud, mogelijkheden of tags via automatische suggesties wanneer u zoektrefwoorden typt. Universeel onderzoek is beschikbaar over alle onderzoekseigenschappen.

![](assets/omnisearch_whatsnew.png)

* U kunt ook zoekfilters toevoegen aan de zoekopdracht in Universeel om de zoekopdracht verder te verfijnen en sneller te laten verlopen.

![](assets/omnisearch_withfilters.png)

* Met de nieuwe zoekopdracht op basis van assetbeoordeling kunt u zoeken naar elementen met waarderingen, indien gepubliceerd vanuit AEM Assets.
* De nieuwe zoekfunctie met meerdere waarden accepteert meerdere trefwoorden met de operator AND om elementen sneller te detecteren.
* Met de nieuwe zoekfunctie kunt u de zoekrelevantie verbeteren, zodat specifieke elementen boven aan de zoekresultaten worden weergegeven.
* Met de nieuwe zoekfunctie op basis van paden kunt u het pad naar een geneste map opgeven om te kunnen zoeken naar elementen in die map.

#### Nieuwe op slimme tags gebaseerde zoekopdracht {#new-smart-tags-based-search}

Als afbeeldingen met slimme tags van AEM Assets naar Brand Portal worden gepubliceerd, kunt u deze afbeeldingen zoeken in Brand Portal met de slimme-tagnamen als zoektrefwoorden. Deze functie is alleen beschikbaar voor bestanden.

### Verbeterde downloadervaring {#enhanced-downloading-experience}

Nadat u een geneste map hebt gedownload, kunt u de oorspronkelijke maphiërarchie behouden. Elementen in een geneste map kunnen in één map worden gedownload, in tegenstelling tot afzonderlijke mappen.

### Verbeterde prestaties {#improved-performance}

Verbeteringen in de mogelijkheden voor bladeren, zoeken en downloaden verbeteren de prestaties van Brand Portal aanzienlijk.

### New digital rights management for assets {#new-digital-rights-management-for-assets}

Beheerders kunnen de vervaldatum en -tijd voor elementen instellen voordat ze deze delen. Nadat een element is verlopen, is het zichtbaar voor viewers en editors, maar kan het niet worden gedownload. Wanneer een element vervalt, ontvangen beheerders een melding.

### Verbeterde middelensortering {#enhanced-asset-sorting}

Het sorteren van middelen in een omslag in lijstmening is niet meer beperkt tot het aantal activa die op de eerste pagina worden getoond. Alle elementen in een map worden gesorteerd, ongeacht of alle elementen op de eerste pagina worden weergegeven.

### Verbeterde rapportage {#reporting-capabilities}

Beheerders kunnen drie typen rapporten maken en beheren: gedownloade, verlopen en gepubliceerde elementen. De capaciteit om de kolommen in een rapport te vormen, en de rapporten naar formaat uit te voeren CSV is ook beschikbaar.

![](assets/newreport.png)

### Aanvullende metagegevens {#additional-metadata}

Merkortaal 6.3.1 introduceert aanvullende metagegevens, die overeenkomen met AEM Assets 6.3. U kunt het formulier Schema-editor gebruiken om de metagegevens te beheren die zichtbaar moeten zijn op de pagina Eigenschappen van elementen. Metagegevens van elementen zijn niet zichtbaar voor gebruikers die gebruikmaken van een externe koppeling en die alleen elementen kunnen voorvertonen en downloaden via de gedeelde URL van de koppeling.

![](assets/additionsinmetadata.png)

### Extra functies voor beheerders {#additional-capabilities-for-administrators}

* Voordat u aanpassingen in de achtergrond voor het aanmeldingsscherm voltooit, kunnen beheerders een voorvertoning van de wijzigingen bekijken.

![](assets/wallpaperpreview.png)

* Nadat een beheerder nieuwe gebruikers toevoegt, moeten zij geen uitnodigingen goedkeuren om aan het Portaal van het Merk worden toegevoegd, worden zij automatisch toegevoegd.

### Nieuwe publicatiemogelijkheden in AEM Assets 6.3 {#new-publishing-capabilities-in-aem-assets}

* AEM beheerders kunnen het schema van meta-gegevens van AEM Assets aan het Portaal van het Merk publiceren gebruikend AEM 6.3 SP1-GFP 1 (6.3.1.1), die in Q4 2017 beschikbaar zal zijn.

![](assets/publish_metadataschemaaemassets.png)

* AEM beheerders kunnen alle tags van AEM Assets naar Brand Portal publiceren met behulp van AEM 6.2 SP1-GVB7 en AEM 6.3 SP1-GVB 1 (6.3.1.1).

![](assets/publish_tags_aemassets.png)

* Vanuit AEM Assets kunt u elementen en verzamelingen publiceren die tags, waaronder slimme tags, bevatten. U kunt vervolgens naar deze elementen of verzamelingen zoeken met deze tags als zoektrefwoorden in Brand Portal.