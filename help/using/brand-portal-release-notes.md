---
title: Release-opmerkingen
description: Lees meer over de functies, verbeteringen, kritieke problemen die zijn opgelost en bekende problemen in de Adobe Experience Manager Assets Brand Portal 2024.10.0-release.
content-type: reference
contentOwner: Kirandeep Kour
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: 3f3065de994f5c38e604b52848b0a538c9efd7d1
workflow-type: tm+mt
source-wordcount: '1508'
ht-degree: 0%

---

# Release-opmerkingen {#release-notes}

Bekijk de nieuwe functies, verbeteringen, belangrijke problemen die zijn opgelost en bekende problemen in de Adobe Experience Manager Assets Brand Portal 2024.10.0-release.

## Gegevens vrijgeven {#release-information}

| Product | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versie | 2024 10,0 |
| Datum | Oktober 2024 |

## Overzicht {#overview}

Met Adobe Experience Manager (AEM) Assets Brand Portal kunt u eenvoudig goedgekeurde creatieve middelen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten. Het draagt bij tot een efficiëntere verdeling van activa, versnelt de marktperiode voor activa en vermindert het risico van niet-naleving en ongeoorloofde toegang. Met Brand Portal kunnen gebruikers op elk gewenst moment in door het bedrijf goedgekeurde indelingen door elementen bladeren, zoeken, voorvertonen, downloaden en exporteren.

## Nieuwe functies in 2024.10.0 {#whats-new-in-2024.10.0}

### Kritieke problemen opgelost {#critical-issues-fixed}

#### Bugfixes {#bug-fixes}

Deze release bevat de volgende opgeloste problemen:

* De e-mailmeldingen voor het aanschaffen van importgebeurtenissen worden niet verzonden.
* Wanneer u het zoekfilter gebruikt, worden in [!DNL Brand Portal] dubbele mappen weergegeven in het venster Filter.
* Het downloaden van verzamelingen met elementen zonder licentie met speciale tekens in de naam werkt niet.
* Wanneer u naar [!UICONTROL Search Form Editor] navigeert, worden labels niet gelokaliseerd.
* Labels worden niet gelokaliseerd in het venster voor het delen van koppelingen.
* Kan video met speciale tekens in de naam niet downloaden.
* Het publiceren en verwijderen van de publicatie van de elementen van [!DNL Adobe Experience Manager Assets] naar Brand Portal werkt niet correct.
* Kan geen video&#39;s afspelen die zijn gedownload van de Brand Portal.

## Eerdere versies

### Release van februari 2024 {#feb-2024}

**fixes en verhogingen van de insect**

Deze release bevat de volgende opgeloste problemen:

* Kan door DRM beveiligde digitale middelen niet downloaden naar de Turkse landinstelling.
* Kan de bestaande rapporten met elementen met een titel van meerdere regels niet openen en downloaden.
* Wanneer u elementen downloadt met de knop [!UICONTROL Download] op de actiebalk, worden maximaal 1000 elementen gedownload.
* Onjuiste naam van PSD-type-elementen, wanneer u deze weergeeft in de inhoudsstructuur.
* [!UICONTROL Delete Rendition] op de pagina met elementdetails werkt niet.
* Verkeerd uitgelijnde titel en grootte van elementen in het pop-upvenster Downloaden.
* Tijdens het maken van een rapport worden labels niet gelokaliseerd.
* Ondersteuningsbeheerders worden in Brand Portal aangeduid als beheerders.

### Release oktober 2023 {#oct-2023}

**fixes en verhogingen van de insect**
Deze release bevat de volgende verbeteringen:

* Prestatieverbeteringen tijdens het bladeren door [!UICONTROL Collections] .

* Verbeteringen in onderzoeksresultaten terwijl het uitvoeren van een gedeeltelijk onderzoek gebruikend het gebied OmniSearch.

Deze release bevat de volgende opgeloste problemen:

* Kan [!UICONTROL Date] niet opslaan en [!UICONTROL Options] loopt vooruit op [!UICONTROL Smart Collection] .

* De [!UICONTROL Date and Time] -indeling is inconsistent wanneer u werkt in een andere landinstelling dan Engels.

* Bij het uitvoeren van een zoekopdracht naar elementen ontbreekt de knop [!UICONTROL Delete] .

* Als het veld [!UICONTROL Title] multibyte-symbolen bevat in [!UICONTROL Link Share] , kan het rapport niet worden gedownload.

* Als u een document van het type PDF bekijkt, zijn de labels en knopinfo niet gelokaliseerd.

### Release van augustus 2023 {#aug-2023}

**fixes en verhogingen van de insect**
Deze release bevat de volgende verbeteringen:

* Prestatieverbeteringen tijdens het laden van elementen in het pop-upvenster [!UICONTROL Download] .
* Wanneer u een middel of een vertoning van een middel downloadt, wordt het nu gedownload in zijn originele dossiertype formaat in plaats van een zip dossier.

Deze release bevat de volgende opgeloste problemen:

* De lange labels of labels worden niet correct weergegeven voor zoekfilters.
* Kan namen van lange vertoningen niet weergeven in het dialoogvenster Downloaden.
* Kan geen voorvertoning van video-elementen weergeven in de kaartweergave.

### Release mei 2023 {#may-2023}

**Bugfixes**
Deze release bevat oplossingen voor de volgende kritieke problemen:

* Als een fout optreedt tijdens het downloaden van een element van een gedeelde koppeling, worden de labels `Notice` en `Close` van de foutmelding niet gelokaliseerd.
* De vertoningen van Brand Portal **de gebieden van de Kopbal van het Verzoek te Grote** fout terwijl de toegang tot van onderzoeksfilters gebruikend `Filter` ruit.

**Bekende kwesties**
Deze release bevat de volgende bekende problemen:

* Gedeeltelijke lokalisatie in de rapportinhoud van Asset sourcing.
* Enkele velden van het gebruikersprofiel kunnen niet worden bewerkt in het gebruikersprofiel.

### Release van februari 2023 {#feb-2023}

**Bugfixes**

Deze release bevat oplossingen voor de volgende kritieke problemen:

* Profielafbeelding kan niet worden bijgewerkt op de Brand Portal.
* De grootte van het deelvenster van de inhoudsstructuur kan niet worden gewijzigd. Als de bestandsnaam langer is dan de standaardbreedte van de inhoudsstructuur, kunt u de inhoudsstructuur niet zowel horizontaal als verticaal slepen. Hierdoor zijn langere bestandsnamen niet leesbaar.
* De zoekresultaten zijn inconsistent voor dezelfde eigenschap die tweemaal in de zoekformulieren wordt gebruikt.
* De tekst op de tussenliggende aanmeldingspagina&#39;s is niet voor alle talen gelokaliseerd.

**Verbeteringen**

Deze release bevat de volgende verbeteringen:

* Er is nu een nieuwe, moderne PDF-viewer beschikbaar voor een verbeterde voorvertoning van de PDF-elementen.
* U kunt er nu voor kiezen om berichten voor het aanschaffen van bedrijfsmiddelen in of uit te schakelen voor beheerders. Navigeer naar [!UICONTROL General Settings] en schakel [!UICONTROL `Notify Administrator of asset contribution`] in of uit.

  ![ breng Beheerder op de hoogte voor activabijdrage ](assets/notify-admin.png)

* Een niet-geautoriseerde gebruiker kan geen toegang tot de Brand Portal aanvragen als de toegang tot de aanvraag is uitgeschakeld.
* De organisaties die alleen provisioned zijn voor Brand Portal, zijn zichtbaar in de lijst met profielkiezers.

**Bekende problemen**

Deze release bevat de volgende bekende problemen:

* Gedeeltelijke lokalisatie in de rapportinhoud van Asset sourcing.
* Enkele velden van het gebruikersprofiel kunnen niet worden bewerkt in het gebruikersprofiel.

### Release oktober 2022 {#oct-2022}

**Kritieke Vaste Kwesties**

Deze release bevat oplossingen voor de volgende kritieke problemen:

* Langzame reactietijden terwijl het kopiëren van grote dossiers van Brand Portal aan een derdehulpmiddel.
* Als u het selectievakje voor het aantal vertoningen inschakelt, worden de selectievakjes voor het selecteren van afzonderlijke uitvoeringen uitgeschakeld.
* Langzame reactietijd voor zoeken.

>[!IMPORTANT]
>
>De pulsmeldingen in de AEM Assets Brand Portal zullen vanaf 1 december 2022 worden stopgezet. In plaats van Pulse-berichten ontvangt u nog steeds e-mailmeldingen voor de volgende gebeurtenissen:
>
>* Elementen delen via koppeling
>* Toegang aanvragen
>* Mappen met bijdragen delen
>* Exporteren naar AEM starten
>* Exporteren naar AEM voltooid
>

### Release van augustus 2022 {#aug-2022}

**Kritieke Vaste Kwesties**

Deze release bevat oplossingen voor de volgende kritieke problemen:

* Als NUI een element niet verwerkt in Experience Manager, geeft Brand Portal een onjuiste status voor het importeren van elementen weer.
* Wanneer de voorvertoningsactie mislukt, is er geen melding om de fout te melden.
* De onjuiste waarde voor de eigenschap `totalUploadedSize` voor elk element is vast.
* Wanneer u **klikt Download alle punten** en er een groot aantal vertoningen beschikbaar voor activa zijn, downloadt Brand Portal een ongeldig .ZIP dossier.
* De vertaling van sommige tekenreeksen wordt afgebroken in de Brand Portal-gebruikersinterface.

### Release mei 2022 {#may-2022}

**Nieuwe eigenschappen**

Brand Portal voert nu om de twaalf uur automatische taken uit om alle Brand Portal-middelen te verwijderen die naar AEM worden gepubliceerd. U hoeft daarom de middelen in de map Contribution niet handmatig te verwijderen om de mapgrootte onder de drempelwaarde te houden.

**Kritieke Vaste Kwesties**

Deze release bevat oplossingen voor de volgende kritieke problemen:

* Wanneer u een map of een verzameling downloadt die elementen met kleurtags bevat, wordt ook een XML-bestand gedownload.
* Wanneer u een video downloadt die uitvoeringen bevat, maakt Brand Portal een ongeldig ZIP-bestand.
* Wanneer u voorinstellingen en elementen maakt op AEM auteur en deze vervolgens publiceert naar Brand Portal, kunt u dynamische uitvoeringen selecteren tijdens het downloaden van de elementen. U kunt het gedownloade .ZIP-bestand echter niet extraheren. Dit probleem voorkomt toegang tot de gedownloade inhoud.
* Problemen tijdens het downloaden van video-elementen uit bepaalde mappen op Brand Portal.
* Wanneer u de URL van de map Contribution deelt via een e-mail, kunnen de rollen Viewer en Editor problemen ondervinden bij het openen van de bovenliggende map via de breadcrumb.
* Het bron gepubliceerde rapport toont een onjuiste tijd van het baanbegin.

### Release van februari 2022 {#feb-2022}

**Nieuwe eigenschappen**

* De drempel van sessietime-out voor de gastgebruikers is verlaagd van 2 uur naar 15 minuten.
* De extra optie **[!UICONTROL View pages]** is verwijderd voor PDF met meerdere pagina&#39;s omdat de gebruiker de pagina&#39;s PDF nu kan bekijken in de Adobe Document Cloud Viewer.
* De gebruikers kunnen niet naar mappen zoeken, navigeren of deze openen. De gebruikersinterface geeft het foutbericht weer: `Failed to load data` .
* In het deelvenster **[!UICONTROL Renditions]** worden niet alle statische uitvoeringen weergegeven van de elementen die naar Brand Portal zijn gepubliceerd.
* In het deelvenster **[!UICONTROL Renditions]** worden de slimme uitsnijduitvoeringen van het element weergegeven, maar de gebruiker kan de slimme uitsnijduitvoeringen niet voorvertonen of downloaden.
* In het dialoogvenster Downloaden worden de slimme uitsnijduitvoeringen van het geselecteerde element weergegeven, maar de gebruiker kan de slimme uitsnijduitvoeringen niet downloaden.
* Een gebruiker die geen beheerder is, krijgt alleen de oorspronkelijke uitvoering van het element wanneer een element wordt gedownload. Het systeem en de aangepaste uitvoeringen worden niet gedownload.
* Wanneer u een zoekfilter toepast om een element te downloaden, wordt de knop `Download` uitgeschakeld in het dialoogvenster voor downloaden en kan de gebruiker het element niet downloaden.
* Als `Smart Tags` en (of) `Color Tags` zijn ingeschakeld, worden de `json` -bestanden weergegeven als uitvoeringen en worden deze `json` -bestanden gedownload in de gearchiveerde ZIP-map.
* De anonieme gebruikers kunnen geen elementen downloaden via een gedeelde koppeling omdat de koppeling wordt omgeleid naar de Brand Portal-aanmeldingspagina.
* Het systeem geeft niet de juiste waarde weer voor het aantal actieve gelijktijdige gebruikers.

<!--
### New Features {#new-features}

This release includes the following new features:

* AEM Assets as a Cloud Service is now entitled to have a pre-configured Brand Portal instance. The Cloud Manager user can activate Brand Portal on the AEM Assets as a Cloud Service instance.

* Asset Sourcing feature is now available on AEM Assets as a Cloud Service. It allows the Brand Portal users to upload assets to the permitted contribution folders and publish the contribution folder from Brand Portal to AEM Assets as a Cloud Service instance. 

* An additional **[!UICONTROL Asset Download]** setting has been introduced under the **[!UICONTROL Download Settings]**. It creates a separate folder for each asset while downloading the folders, collections, or bulk download of assets. 
-->
<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions.
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog.
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users]() to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

<!--
### Enhancements {#enhancements}

Brand Portal 2021.08.0 is an internal release that introduces Business profiles for enterprise and teams customers to give organizations better control over their assets. 

This release includes the following enhancements:

* The users now have organization-specific entitlement on the new and migrated organizations. If a user is entitled to multiple organizations, the user has to select the organization at the time of login.

* The new users that are added in Admin Console must **Join Team** to get entitled to the organization. 

>[!NOTE]
>
>Business profiles are currently applicable for the new organizations that are created after August 16, 2021. 
>
>Until your organization is migrated, you can continue to use Adobe ID, Enterprise ID, or Federated ID types to access the organization.   
-->

<!-- 
* For folder download, a separate folder is created for each asset using share link irrespective of the **[!UICONTROL Download Settings]**. 
* The Brand Portal **[!UICONTROL Usage Report]** has been modified to reflect only the active Brand Portal users.
-->

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.

* The users are unable to search, navigate, or open folders. The user interface reflects the error message: `Failed to load data`. 
* The **[!UICONTROL Renditions]** panel does not list all the static renditions of the assets that are published to Brand Portal.
* The **[!UICONTROL Renditions]** panel lists the smart crop renditions of the asset, however, the user cannot preview or download the smart crop renditions.
* The download dialog lists the smart crop renditions of the selected asset, however, the user cannot download the smart crop renditions. 
* A non-admin user is getting only the original asset rendition when downloading an asset. The system and custom renditions are not downloaded.  
* When applying search filter to download an asset, the `Download` button is disabled in the download dialog and does not allows the user to download the asset.
* If `Smart Tags` and (or) `Color Tags` are enabled, the download dialog lists the `json` files as renditions and downloads these `json` files in the archived zip folder.
* The anonymous users are unable to download assets using a shared link because the link redirects to the Brand Portal login page. 
* The system is not reflecting the correct value for the number of active concurrent users.
-->

<!--
### New features {#new-features}

Brand Portal now executes automatic jobs every twelve hours to delete all Brand Portal assets that are published to AEM. As a result, you do not need to delete the assets in the Contribution folder manually to keep the folder size below the threshold limit. See [What's new in Experience Manager Assets Brand Portal](whats-new.md).
-->

<!--
This release includes fixes to the following critical issues:

* When you download a folder or a collection that includes assets with color tags, an XML file gets downloaded as well.

* When you download a video that includes renditions, Brand Portal creates an invalid .ZIP file.

* When you create presets and assets on AEM author and publish them to Brand Portal and then select dynamic renditions while downloading the assets, you cannot extract the downloaded .ZIP file.

* Issues while downloading video assets from certain folders available on Brand Portal.

* When you share the Contribution folder's URL using an email, Viewer and Editor roles face issues while accessing its parent folder using the breadcrumb.

* Sourcing published report displays an incorrect job start time.
>
 
<!--
* Asset Sourcing email notifications are not delivered for some organizations. 

* Video files with extension `.mov` are not running on Brand Portal. 

* In the **[!UICONTROL Smart Collections]** dropdown list, only ten saved collections are visible. 
-->
<!--
* *_deleted tenants are listed as valid tenant which fails during the execution of TenantCustomizers/TenantUpdates where tenant id is returned as /etc/tenants/`<nodename>`.
-->

<!--
In case only the original assets are downloaded, the asset reflects its own extension and does not open until the extension is manually changed to zip. 
* The user interface of the collection folder does not respond on clicking the navigation arrow. 
* **[!UICONTROL Create]** button is visible in the **[!UICONTROL Column]** view even when the folders are empty.
* **[!UICONTROL Omni search]** fails with a 414 error message (Request-URI Too Long) if the dispatcher is bypassed while accessing the Brand Portal instance.
* An empty zip folder is downloaded if the asset contains a comma (`,`) in the file name.
* The viewer users get the option to add users to the collection they have created. 
* Inconsistent behavior is experienced when an asset (thumbnail or web rendition) is downloaded using share link.

See [what's new in Brand Portal 2021.02.0](whats-new.md).
-->

<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* Search on the **[!UICONTROL Asset Reports]** shows processing on the product interface with no search result.
* The video DM encodes are not visible to the non-admin users on the asset details page.
* The alignment of the size of individual asset renditions and total download size is distorted in the Download dialog.
-->


<!--
* Download Settings configuration to configure asset download from Brand Portal. Fast download, custom renditions, and system renditions are the available configurations. 
-->

<!--
* Document Viewer has been introduced to enhance the PDF viewing experience. New options are available for viewing the PDF files in Brand Portal.

* Advances in the asset download process which improves the Brand Portal user experience while [downloading assets from Brand Portal](brand-portal-download-assets.md). Brand Portal administrators can configure **[!UICONTROL Fast Download]**, **[!UICONTROL Custom Renditions]**, and **[!UICONTROL System Renditions]** from the **[!UICONTROL Download]** settings. 

For details, see [what's new in Brand Portal 6.4.7](whats-new.md). 

### Critical Issues Fixed {#critical-issues-fixed-647}

This release includes fixes to the following critical issues:

* The viewer users are not permitted to share link for collections but the option to share is visible to them on the product interface.

* The **[!UICONTROL Download]** button on the options bar does not list all the licensed assets of the selected folder.

* The search takes longer to show the results for certain keywords.

* The **[!UICONTROL Agree]** and **[!UICONTROL Disagree]** check boxes does not appear on bulk selection of licensed and unlicensed assets during download.

* Filter-based search shows processing on the product interface with no search result. 

* The assets do not download from share link if the shared folder contains numerous and large assets.


### Known Issues {#known-issues-647}

This release includes the following known issues:

* If multiple assets are selected, license text does not appear on clicking Terms and Conditions on the license agreement page during download using share link.   

-->

## Talen {#languages}

De Brand Portal-gebruikersinterface is beschikbaar in de volgende talen:

* Engels
* Duits
* Frans
* Spaans
* Italiaans
* Braziliaans Portugees
* Japans
* Vereenvoudigd Chinees
* Koreaans

## Gecertificeerde platforms {#certified-platforms}

Om te zien welke platforms voor deze versie van Brand Portal worden verklaard, controleer de **Steun voor aanraking-geoptimaliseerde UI** kolom in **Ondersteunde Browsers voor Authoring sectie van het Gebruikersinterface** van [ Technische Vereisten ](https://experienceleague.adobe.com/nl/docs/experience-manager-65/content/implementing/deploying/introduction/technical-requirements).

## Koppelingen {#links}

* [ de Pagina van het Product van Adobe Experience Manager op adobe.com ](https://business.adobe.com/in/products/experience-manager/adobe-experience-manager.html)
* [ Documentatie van Assets Brand Portal ](https://experienceleague.adobe.com/nl/docs/experience-manager-brand-portal/using/home)

## Toegang tot en ondersteuning voor producten (beperkt aantal sites) {#product-access-and-support-restricted-sites}

Deze sites zijn alleen beschikbaar voor klanten. Als u een klant bent en toegang nodig hebt, neemt u contact op met de accountmanager van de Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support]()
-->
