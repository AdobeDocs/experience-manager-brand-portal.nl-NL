---
title: Elementen downloaden
seo-title: Elementen downloaden
description: Alle gebruikers kunnen tegelijkertijd meerdere middelen en mappen downloaden die voor hen toegankelijk zijn. Op deze manier kunnen goedgekeurde merkmiddelen veilig worden gedistribueerd voor offline gebruik.
seo-description: Alle gebruikers kunnen tegelijkertijd meerdere middelen en mappen downloaden die voor hen toegankelijk zijn. Op deze manier kunnen goedgekeurde merkmiddelen veilig worden gedistribueerd voor offline gebruik.
uuid: 4b57118e-a76e-4d8a-992a-cb3c3097bc03
content-type: reference
contentOwner: Vishabh Gupta
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: download-install
discoiquuid: f90c2214-beea-4695-9102-8b952bc9fd17
translation-type: tm+mt
source-git-commit: 46e6bf2865aa90953791fdee9f24673e92cb19b7
workflow-type: tm+mt
source-wordcount: '1854'
ht-degree: 0%

---


# Elementen downloaden van Brand Portal {#download-assets-from-bp}

<!-- Before update in Download experience - 26th Aug 2020 comment by Vishabh.
 All users can simultaneously download multiple assets and folders accessible to them from Brand Portal. This way, approved brand assets can be securely distributed for offline use. Read on to know how to download approved assets from Brand Portal, and what to expect from the [download performance](../using/brand-portal-download-assets.md#main-pars-header).
-->

Adobe Experience Manager Assets Brand Portal verbetert de downloadervaring doordat gebruikers tegelijkertijd meerdere middelen en mappen kunnen downloaden die voor hen toegankelijk zijn via Brand Portal. Op deze manier kunnen goedgekeurde merkmiddelen veilig worden gedistribueerd voor offline gebruik. Lees verder om te weten hoe u goedgekeurde middelen kunt downloaden van Brand Portal en wat u kunt verwachten van de [downloadprestaties](../using/brand-portal-download-assets.md#expected-download-performance).


>[!NOTE]
>
>In Brand Portal 2020.10.0 (en hoger) is de instelling **[!UICONTROL Fast Download]** standaard ingeschakeld, waarbij IBM Aspera Connect wordt gebruikt voor het versnelde downloaden van de middelen. [Installeer IBM Aspera Connect 3.9.9](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html) in de browserextensie voordat u de middelen downloadt van Brand Portal. Voor meer details, zie [gids om downloads van het Portaal van het Merk te versnellen](../using/accelerated-download.md).
>
>Als u IBM Aspera Connect niet wilt gebruiken en verder wilt gaan met het normale downloadproces, neemt u contact op met de beheerder van het Brand Portal om de instelling **[!UICONTROL Fast Download]** uit te schakelen.

## Elementdownload {#configure-download} configureren

De beheerders van het Portaal van het merk kunnen de activa downloaden en de montages van de gebruikersgroep voor de gebruikers van het Portaal van het Merk vormen hen om tot activa van de interface van het Portaal van het Merk toegang te hebben en te downloaden.

>[!NOTE]
>
>De downloadmontages die op het gebruikersinterface worden toegepast vergemakkelijken een zelfbedieningservaring aan de gebruikers van het Portaal van het Merk om de activa gemakkelijk te vormen en te downloaden. Het beperkt niet het downloaden van elementen op de toepassingslaag, bijvoorbeeld, kunnen de gebruikers tot de activa nog toegang hebben en downloaden vertoningen met de volledige weg URL.

De toegang tot en het downloaden van de activa van de interface van het Portaal van het Merk wordt bepaald door de volgende configuraties:

* Downloadinstellingen inschakelen
* Gebruikersgroepinstellingen configureren

### Downloadinstellingen {#enable-download-settings} inschakelen

De beheerders kunnen de activa **[!UICONTROL Download Settings]** toelaten om de reeks vertoningen te bepalen die voor de gebruikers van het Portaal van het Merk voor download toegankelijk zijn.

De beschikbare instellingen zijn:

* **[!UICONTROL Fast Download]**

   Hiermee kunt u de middelen sneller downloaden met IBM Aspera Connect. Standaard is de instelling **[!UICONTROL Fast Download]** ingeschakeld in **[!UICONTROL Download Settings]**.

* **[!UICONTROL Custom Renditions]**

   Hiermee kunt u aangepaste en (of) dynamische uitvoeringen van de elementen downloaden.

   Alle andere elementuitvoeringen dan het oorspronkelijke element en door het systeem gegenereerde uitvoeringen worden aangepaste uitvoeringen genoemd. Dit omvat statische en dynamische uitvoeringen die beschikbaar zijn voor het element. Elke gebruiker kan een aangepaste statische uitvoering maken in AEM Assets, terwijl alleen de AEM beheerder aangepaste dynamische uitvoeringen kan maken. Zie [hoe u voorinstellingen voor afbeeldingen of dynamische vertoningen kunt toepassen](../using/brand-portal-image-presets.md) voor meer informatie.

* **[!UICONTROL System Renditions]**

   Hiermee kunt u door het systeem gegenereerde uitvoeringen van de elementen downloaden.

   Dit zijn de miniaturen die automatisch worden gegenereerd in AEM Assets op basis van de workflow voor &quot;DAM-updatebestanden&quot;.

Meld u als beheerder aan bij uw Brand Portal-gebruiker en navigeer naar **[!UICONTROL Tools]** > **[!UICONTROL Download]**.

De beheerders kunnen om het even welke combinatie montages voor de gebruikers van het Portaal van het Merk aan toegang en downloadvertoningen toelaten.

![](assets/download-configuration.png)


>[!NOTE]
>
>Alleen de beheerders kunnen de verlopen elementen downloaden. Zie [Digitale rechten van elementen beheren](../using/manage-digital-rights-of-assets.md) voor meer informatie over verlopen elementen.

### Gebruikersgroepinstellingen {#configure-user-group-settings} configureren

Naast **[!UICONTROL Download Settings]** kunnen de beheerders van het Poortportaal van het Merk montages voor verschillende groep gebruikers verder vormen om de originele activa en hun vertoningen te bekijken en (of) te downloaden.

Meld u als beheerder aan bij uw Brand Portal-gebruiker en navigeer naar **[!UICONTROL Tools]** > **[!UICONTROL Users]**. Navigeer op de pagina **[!UICONTROL User Roles]** naar het tabblad **[!UICONTROL Groups]** om de weergave- en (of) downloadinstellingen voor de gebruikersgroepen te configureren.

![view-download-permission](assets/download-permissions.png)

>[!NOTE]
>
>Als een gebruiker wordt toegevoegd aan meerdere groepen en als een van deze groepen beperkingen heeft, gelden de beperkingen voor de gebruiker.

Gebaseerd op de configuratie, blijft het downloadwerkschema constant voor stand-alone activa, veelvoudige activa, omslagen die activa, vergunning of unlicensed activa bevatten, en het downloaden van activa gebruikend aandeelverbinding.

De volgende matrix definieert of een gebruiker toegang heeft tot de uitvoeringen, afhankelijk van de [downloadconfiguraties](#configure-download):

| **Downloadinstellingen: Aangepaste uitvoeringen** | **Downloadinstellingen: Systeemuitvoeringen** | **Instellingen gebruikersgroep: Origineel downloaden** | **Instellingen gebruikersgroep: Uitvoeringen downloaden** | **Resultaat** |
|---|---|---|---|---|
| ON | ON | ON | ON | Alle uitvoeringen weergeven en downloaden |
| ON | ON | UIT | UIT | Origineel element weergeven |
| UIT | UIT | ON | ON | Oorspronkelijk middel weergeven en downloaden |
| ON | UIT | ON | ON | Oorspronkelijk middel en aangepaste uitvoeringen weergeven en downloaden |
| UIT | ON | ON | ON | Oorspronkelijke middel- en systeemuitvoeringen weergeven en downloaden |
| ON | UIT | UIT | UIT | Origineel element weergeven |
| UIT | ON | UIT | UIT | Origineel element weergeven |
| UIT | UIT | UIT | ON | Origineel element weergeven |
| UIT | UIT | ON | UIT | Oorspronkelijk middel weergeven en downloaden |
| UIT | UIT | UIT | UIT | Origineel element weergeven |



## Elementen {#download-assets} downloaden

De gebruikers van het Portaal van het merk kunnen veelvoudige activa, omslagen die activa, en inzamelingen van de interface van het Portaal van het Merk downloaden.

>[!NOTE]
>
>Neem contact op met de beheerder van het Brand Portal als u geen machtiging hebt om de elementuitvoeringen te openen of te downloaden.

Als de gebruiker toegang tot vertoningen heeft, wordt de gebruiker voorzien van het verbeterde **[!UICONTROL Download]** dialoog met de volgende mogelijkheden:
* Alle beschikbare uitvoeringen van elementen in de downloadlijst weergeven.
* Sluit uitvoeringen van de elementen uit die niet vereist zijn voor downloaden.
* Pas met één klik dezelfde set uitvoeringen toe op alle vergelijkbare elementtypen.
* Pas een andere set uitvoeringen toe voor verschillende elementtypen.
* Maak een aparte map voor elke elementuitvoering.
* Geselecteerde elementen en de bijbehorende uitvoeringen downloaden.

![download-dialog](assets/download-dialog-box.png)

>[!NOTE]
>
>Het dialoogvenster **[!UICONTROL Download]** wordt alleen weergegeven als de elementen zijn geselecteerd om te worden gedownload en **[!UICONTROL Custom Renditions]** of **[!UICONTROL System Renditions]** is ingeschakeld in **[!UICONTROL Download Settings]**.


### Stappen om elementen te downloaden {#bulk-download}

Hier volgen de stappen voor het downloaden van elementen of mappen met elementen van de interface Brand Portal:

1. Meld u aan bij uw Brand Portal-huurder. Standaard wordt de weergave **[!UICONTROL Files]** geopend, die alle gepubliceerde elementen en mappen bevat.

   Voer een van de volgende handelingen uit:

   * Selecteer de elementen of mappen die u wilt downloaden. Klik op het pictogram **[!UICONTROL Download]** op de werkbalk boven in het scherm.

      ![select-multiple-assets](assets/select-assets-new.png)

   * Als u specifieke elementuitvoeringen van een element wilt downloaden, plaatst u de aanwijzer boven het element en klikt u op het pictogram **[!UICONTROL Download]** in de miniaturen van de snelle handeling.

      ![select-element](assets/select-asset.png)


      >[!NOTE]
      >
      >Als u de middelen voor het eerst downloadt en IBM Aspera Connect niet in uw browser hebt geïnstalleerd, wordt u gevraagd om de Aspera-downloadaccelerator te installeren.


      >[!NOTE]
      >
      >Als de elementen die u downloadt ook gelicentieerde elementen bevatten, wordt u doorgestuurd naar de pagina **[!UICONTROL Copyright Management]**. Selecteer op deze pagina de elementen, klik op **[!UICONTROL Agree]** en klik op **[!UICONTROL Download]**. Als u het niet eens bent, worden de gelicentieerde middelen niet gedownload.
      > 
      >Voor met licentie beveiligde elementen is [licentieovereenkomst gekoppeld](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets). Dit gebeurt door de [metagegevenseigenschap](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) van het element in Experience Manager Assets in te stellen.


      ![in licentie gegeven](assets/licensed-asset-new.png)

1. Het dialoogvenster **[!UICONTROL Download]** met alle geselecteerde elementen wordt geopend.

   Klik op een element om de beschikbare uitvoeringen weer te geven en selecteer de selectievakjes die overeenkomen met de uitvoeringen die u wilt downloaden.

   U kunt de uitvoeringen voor afzonderlijke elementen handmatig selecteren of uitsluiten, of op het pictogram **Toepassen** klikken om dezelfde set uitvoeringen te selecteren die u voor vergelijkbare elementtypen wilt downloaden (alle afbeeldingsbestanden in dit voorbeeld). Klik in het dialoogvenster **[!UICONTROL Apply All]** op **[!UICONTROL Done]** om de regel toe te passen op alle vergelijkbare elementen.

   ![toepassen](assets/apply.png)

   U kunt ook een element uit de downloadlijst verwijderen (indien vereist) door op het pictogram **Verwijderen** te klikken.

   ![remove](assets/remove.png)

   Selecteer het selectievakje **[!UICONTROL Create separate folder for each asset]** om de maphiërarchie van het Brand Portal te behouden tijdens het downloaden van elementen. Standaard wordt de maphiërarchie Brand Portal genegeerd en worden alle elementen gedownload in een ZIP-map.

   De downloadknop geeft het aantal geselecteerde items weer. Als u klaar bent met het toepassen van de regels, klikt u op **[!UICONTROL Download items]**.

   ![download-dialog](assets/download-dialog-new.png)

1. Standaard is de instelling **[!UICONTROL Fast Download]** ingeschakeld in **[!UICONTROL Download Settings]**. Daarom wordt een bevestigingsvenster weergegeven waarin versnelde download met IBM Aspera Connect is toegestaan.

   Als u **[!UICONTROL Fast Download]** wilt blijven gebruiken, klikt u op **[!UICONTROL Allow]**. Alle geselecteerde vertoningen worden gedownload in een ZIP-map met behulp van IBM Aspera Connect.

   Als u IBM Aspera Connect niet wilt gebruiken, klikt u op **[!UICONTROL Deny]**. Als **[!UICONTROL Fast Download]** wordt ontkend of ontbreekt, bevolkt het systeem een Bericht van de Fout. Klik op de knop **[!UICONTROL Normal Download]** om door te gaan met het downloaden van de elementen. De geselecteerde vertoningen worden gedownload in een ZIP-map zonder gebruik te maken van IBM Aspera Connect.

>[!NOTE]
>
>Als de instelling **[!UICONTROL Fast Download]** door de beheerder is uitgeschakeld, worden de geselecteerde uitvoeringen rechtstreeks gedownload in een ZIP-map zonder gebruik te maken van IBM Aspera Connect.


>[!NOTE]
>
>Als een map, verzameling of meer dan 20 elementen zijn geselecteerd om te worden gedownload, wordt het dialoogvenster **[!UICONTROL Download]** overgeslagen en worden alle elementenuitvoeringen die voor de gebruiker toegankelijk zijn, met uitzondering van de dynamische uitvoeringen, gedownload in een ZIP-map. De elementuitvoeringen worden gedownload in een aparte map voor elk element in de ZIP-map.


>[!NOTE]
>
>Het Portaal van het merk steunt het vormen Dynamic Media op zowel Hybride als wijze Scene 7.
>
>(*Als AEM auteurinstantie op **Dynamic Media Hybride wijze*** loopt)
>
>Als u dynamische uitvoeringen van een element wilt voorvertonen of downloaden, zorgt u ervoor dat de dynamische media is ingeschakeld en de Pyramid-TIFF-uitvoering van het element bestaat in de AEM Assets-auteur-instantie vanwaar de elementen zijn gepubliceerd. Wanneer een middel van AEM aan het Portaal van het Merk wordt gepubliceerd, wordt zijn piramide tiff vertoning ook gepubliceerd.



Als de beheerder u niet [heeft gemachtigd om toegang te hebben tot de oorspronkelijke vertoningen](../using/brand-portal-adding-users.md#main-pars-procedure-202029708), worden de oorspronkelijke vertoningen van de geselecteerde elementen niet gedownload.

![no-access-message](assets/no-access-message.png)

<!-- This issue has been resolved, check with engineering.
>[!NOTE]
>
>Once you have downloaded the asset renditions, the **[!UICONTROL Download]** button is disabled to avoid creating duplicate copies of the renditions. To download more (missing or another copy of renditions), refresh the browser to re-enable the download button.
-->

### Elementen downloaden van de pagina met elementdetails {#download-assets-from-asset-details-page}

Naast de downloadworkflow is er een andere methode om de uitvoeringen voor afzonderlijke elementen rechtstreeks te downloaden vanaf de pagina met elementdetails.

Gebruikers kunnen een voorvertoning van verschillende uitvoeringen bekijken, specifieke uitvoeringen selecteren en deze rechtstreeks downloaden vanuit het deelvenster **[!UICONTROL Renditions]** op de pagina met elementdetails zonder het dialoogvenster **[!UICONTROL Download]** te hoeven openen.


Hier volgen de stappen voor het downloaden van elementuitvoeringen van de pagina met elementdetails:

1. Meld u aan bij uw Poortmedewerker voor merken en klik op het element om de pagina met elementdetails te openen.
1. Klik op het bedekkingspictogram aan de linkerkant en klik op **[!UICONTROL Renditions]**.

   ![rendition-navigation](assets/rendition-navigation.png)

1. In het **[!UICONTROL Renditions]**-deelvenster worden alle toegankelijke elementuitvoeringen weergegeven op basis van het element [downloadconfiguraties](#configure-download).

   Selecteer de specifieke vertoningen die u wilt downloaden en klik op **[!UICONTROL Download items]**.

   ![renditions-panel](assets/renditions-panel.png)

1. Standaard is de instelling **[!UICONTROL Fast Download]** ingeschakeld in **[!UICONTROL Download Settings]**. Daarom wordt een bevestigingsvenster weergegeven waarin versnelde download met IBM Aspera Connect is toegestaan.

   Als u **[!UICONTROL Fast Download]** wilt blijven gebruiken, klikt u op **[!UICONTROL Allow]**. Alle geselecteerde vertoningen worden gedownload in een ZIP-map met behulp van IBM Aspera Connect.

   Als u het gebruik van **[!UICONTROL Fast Download]** weigert, vult het systeem een foutbericht in. Klik op de knop **[!UICONTROL Normal Download]** om door te gaan met downloaden. De geselecteerde vertoningen worden gedownload in een ZIP-map zonder gebruik te maken van IBM Aspera Connect.

>[!NOTE]
>
>Als de instelling **[!UICONTROL Fast Download]** door de beheerder is uitgeschakeld, worden de geselecteerde uitvoeringen rechtstreeks gedownload in een ZIP-map zonder gebruik te maken van IBM Aspera Connect.


>[!NOTE]
>
>Elementen die afzonderlijk worden gedownload, worden weergegeven in het rapport voor het downloaden van elementen. Als er echter een map met elementen wordt gedownload, worden de map en de middelen niet weergegeven in het rapport voor het downloaden van middelen.

<!--
>[!NOTE]
>
>Assets that are individually downloaded are visible in the assets download report. However, if a folder containing assets is downloaded, the folder and assets are not displayed in the assets download report.
-->

<!-- Backup of content before updating the new feature docs.
## Configure asset download {#configure-download}

The download configuration allows the Brand Portal administrators to define the set of renditions available to the Brand Portal users for downloading the assets. The administrator can configure the asset **[!UICONTROL Download]** settings from the Brand Portal interface. 

The available configurations are:

* **[!UICONTROL Fast Download]** 

  Enables high-speed download of the assets. To know more, see [guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).

* **[!UICONTROL Custom Renditions]** 
  
  Download custom and (or) dynamic renditions of the assets. 
  All the asset renditions other than the original asset and system-generated renditions are called as custom renditions. It includes static as well as dynamic renditions available for the asset. Any user can create a custom static rendition in AEM Assets, whereas, only the AEM administrator can create custom dynamic renditions. To know more, see [how to apply image presets or dynamic renditions](../using/brand-portal-image-presets.md)

* **[!UICONTROL System Renditions]** 

  Download system-generated renditions of the assets. These are the thumbnails which are automatically generated in AEM Assets based on the "DAM update asset" workflow. 

Log in to your Brand Portal tenant as an administrator and navigate to **[!UICONTROL Tools]** > **[!UICONTROL Download]**. By default, the **[!UICONTROL Fast Download]** configuration is enabled in the **[!UICONTROL Download Settings]**. 

The administrators can enable any combination to configure the asset download process.

![](assets/download-configuration.png)


Based on the configuration, the download workflow remains constant for stand-alone assets, multiple assets, folders containing assets, licensed or unlicensed assets, and downloading assets using share link. 


* If both **[!UICONTROL Custom Renditions]** and **[!UICONTROL System Renditions]** configurations are turned-off, the original renditions of the assets are downloaded without any additional dialog being presented to the users.    


* If any of the **[!UICONTROL Custom Renditions]** or **[!UICONTROL System Renditions]** configuration is enabled, an additional **[!UICONTROL Download]** dialog box appears wherein you can choose whether to download the original asset along with its renditions, or download only specific renditions. 

>[!NOTE]
>
>Only the administrators can download the expired assets. For more information about expired assets, see [manage digital rights of assets](../using/manage-digital-rights-of-assets.md).

## Steps to download assets {#steps-to-download-assets}

Following are the steps to download assets or folders containing assets from Brand Portal:

1. From the Brand Portal interface, do one of the following:

   * Select the folders or assets you want to download. From the toolbar at the top, click the **[!UICONTROL Download]** icon.

     ![](assets/downloadassets-1.png)

   * To download a specific asset or folder, hover the pointer over the asset or folder and click the **[!UICONTROL Download]** icon available in the quick action thumbnails.

     ![](assets/downloadsingleasset-1.png)


     >[!NOTE]
     >
     >If you are downloading the assets for the first time and do not have IBM Aspera Connect installed in your browser, it will prompt you to install the Aspera download accelerator. 


     >[!NOTE]
     >
     >If the assets you are downloading also include licensed assets, you are redirected to the **[!UICONTROL Copyright Management]** page. In this page, select the assets, click **[!UICONTROL Agree]**, and then click **[!UICONTROL Download]**. If you choose to disagree, licensed assets are not downloaded. 
     > 
     >License-protected assets have [license agreement attached](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) to them, which is done by setting asset's [metadata property](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) in Experience Manager Assets.


     ![](assets/licensed-asset-download-1.png)

     
     >[!NOTE]
     >
     >Ensure to select all the required asset renditions while downloading them from the asset details page, and click **[!UICONTROL Download]**. The selected renditions are downloaded to your local machine.
     > 
     >Once you download, the **[!UICONTROL Download]** button is disabled to avoid creating duplicate copies of the downloaded renditions. To download more (missing or another copy of renditions), refresh the browser to re-enable the download button.

     If any of the **[!UICONTROL Custom Renditions]** or **[!UICONTROL System Renditions]** configuration is enabled in the **[!UICONTROL Download Settings]**, the **[!UICONTROL Download]** dialog appears with the **[!UICONTROL Asset(s)]** check box selected by default. If the **[!UICONTROL Fast Download]** configuration is enabled, the **[!UICONTROL Enable download acceleration]** check box is selected by default.

     ![](assets/download-dialog.png)

     >[!NOTE]
     >
     >If the downloading assets are image files, and you select only the **[!UICONTROL Asset(s)]** check box in the **[!UICONTROL Download]** dialog but are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) then no image files are downloaded and a notification appears, stating that you have been restricted by the administrator to access original renditions.

     ![](assets/restrictaccess-note.png)

1. To download the renditions in addition to the original assets, select the **[!UICONTROL Rendition(s)]** check box. However, if you want to download the system-generated renditions along with the custom renditions, clear the **[!UICONTROL Exclude System Renditions]** check box.

   ![](assets/download-system-rendition.png)

   * To download only the renditions, clear the **[!UICONTROL Asset(s)]** check box.

     >[!NOTE]
     >
     >By default, only the assets are downloaded. However, original renditions of image files are not downloaded if you are not [authorized by the administrator to have access to the original renditions of image files](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

    * To share the selected assets with other users through a link, select the **[!UICONTROL Email]** check box. An email notification is sent to the users with the download link. To know how to download assets from shared links, see [downloading assets from shared links](../using/brand-portal-link-share.md#main-pars-header-1703469193).  

      ![](assets/download-link.png)

      >[!NOTE]
      >
      >The download link on email notification expires after 45 days.
      >
      >The administrators can customize email messages, that is, logo, description, and footer, using the [Branding](../using/brand-portal-branding.md) feature.


    * You can select a predefined image preset or create a custom dynamic rendition from the **[!UICONTROL Download]** dialog box. 

      To apply a [custom image preset to the asset and its renditions](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages), select the **[!UICONTROL Dynamic Rendition(s)]** check box. Specify the image preset properties (such as size, format, color space, resolution, and image modifier) to apply the custom image preset while downloading the asset and its renditions. To download only the dynamic renditions, clear the **[!UICONTROL Asset(s)]** check box.

      ![](assets/dynamic-rendition.png)

      >[!NOTE]
      >
      >Brand Portal supports configuring Dynamic Media in both - Hybird and Scene 7 mode. 
      >
      >(*If AEM author instance is running on **Dynamic Media Hybrid mode***)
      >
      >To preview or download dynamic renditions of an asset, ensure that the dynamic media is enabled and the asset's Pyramid tiff rendition exists at the AEM Assets author instance from where the assets have been published. When an asset is published to Brand Portal, its Pyramid tiff rendition is also published.
      
  
    * To preserve the Brand Portal folder hierarchy while downloading assets, select the **[!UICONTROL Create separate folder for each asset]** check box. By default, the Brand Portal folder hierarchy is ignored and all the assets are downloaded in one folder in your local system.

1. Click **[!UICONTROL Download]**.

   The assets (and renditions if selected) are downloaded as a zip file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions. 

   If you are not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#main-pars-procedure-202029708), the original renditions of the selected assets are not downloaded. 

   >[!NOTE]
   >
   >Assets that are individually downloaded are visible in the assets download report. However, if a folder containing assets is downloaded, the folder and assets are not displayed in the assets download report.
-->

## Downloadprestaties {#expected-download-performance} verwacht

Het downloaden van bestanden kan per clientlocatie verschillen, afhankelijk van factoren zoals lokale internetverbinding en serverwachttijd. De verwachte downloadprestaties voor 2-GB dossier dat bij verschillende cliëntplaatsen wordt waargenomen zijn als volgt, met de server van het Portaal van het Merk bij Oregon in Verenigde Staten:

| Clientlocatie | Latentie tussen client en server | Downloadsnelheid verwacht | Tijd die nodig is om een bestand van 2 GB te downloaden |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| US West (N. Californië) | 18 milliseconden | 7,68 MB/s | 4 minuten |
| US West (Oregon) | 42 milliseconden | 3,84 MB/s | 9 minuten |
| US East (N. Virginia) | 85 milliseconden | 1,61 MB/s | 21 minuten |
| APAC (Tokio) | 124 milliseconden | 1,13 MB/s | 30 minuten |
| Noida | 275 milliseconden | 0,5 MB/s | 68 minuten |
| Sydney | 175 milliseconden | 0,49 MB/s | 69 minuten |
| Londen | 179 milliseconden | 0,32 MB/s | 106 minuten |
| Singapore | 196 milliseconden | 0,5 MB/s | 68 minuten |


>[!NOTE]
>
>Er worden gegevens met betrekking tot de kationen waargenomen onder testomstandigheden, die kunnen variëren voor gebruikers op verschillende locaties met een gevarieerde latentie en bandbreedte.

