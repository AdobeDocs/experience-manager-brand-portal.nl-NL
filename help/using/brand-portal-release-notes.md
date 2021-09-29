---
title: Release-opmerkingen
seo-title: Release Notes
description: Lees meer over de functies, verbeteringen, belangrijke problemen die zijn opgelost en bekende problemen in de Adobe Experience Manager Assets Brand Portal 2021.08.0-release.
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 2021.08.0 release.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: 67a745fed6a13cfdb30e26062eecc3c8d1775e36
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 3%

---

# Release-opmerkingen {#release-notes}

Bekijk de nieuwe functies, verbeteringen, belangrijke problemen die zijn opgelost en bekende problemen in de Adobe Experience Manager Assets Brand Portal 2021.08.0-release.

## Geen informatie {#release-information}

| Product | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versie | 2021,08,0 |
| Date | augustus 2021 |

## Overzicht {#overview}

Met Adobe Experience Manager (AEM) Assets Brand Portal kunt u eenvoudig goedgekeurde creatieve middelen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten. Het draagt bij tot een efficiëntere verdeling van activa, versnelt de marktintroductie van activa en vermindert het risico van niet-naleving en ongeoorloofde toegang. Met Brand Portal kunnen gebruikers bestanden in door het bedrijf goedgekeurde indelingen doorbladeren, zoeken, voorvertonen, downloaden en exporteren, altijd en overal.

## Nieuwe functies in 2021.08.0 {#whats-new-in-2021.08.0}

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


### Verbeteringen {#enhancements}

Brand Portal 2021.08.0 is een interne release die bedrijfsprofielen introduceert voor ondernemingen en teams klanten om organisaties betere controle te geven over hun middelen.

Deze release bevat de volgende verbeteringen:

* De gebruikers hebben nu organisatiespecifieke rechten voor de nieuwe en gemigreerde organisaties. Als een gebruiker recht heeft op meerdere organisaties, moet de gebruiker de organisatie selecteren op het moment van aanmelding.

* De nieuwe gebruikers die in Admin Console worden toegevoegd moeten **zich aansluiten bij Team** om recht op de organisatie te krijgen.

>[!NOTE]
>
>De bedrijfsprofielen zijn momenteel van toepassing op de nieuwe organisaties die na 16 augustus 2021 worden gecreeerd.
>
>Totdat uw organisatie is gemigreerd, kunt u Adobe ID, Enterprise ID, of de types van Federated ID blijven gebruiken om tot de organisatie toegang te hebben.

<!-- 
* For folder download, a separate folder is created for each asset using share link irrespective of the **[!UICONTROL Download Settings]**. 
* The Brand Portal **[!UICONTROL Usage Report]** has been modified to reflect only the active Brand Portal users.
-->

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Kritieke problemen opgelost {#critical-issues-fixed}

Deze release bevat oplossingen voor de volgende kritieke problemen:

* E-mailmeldingen voor middelenbronnen worden niet voor sommige organisaties geleverd.

* Videobestanden met extensie `.mov` worden niet uitgevoerd op Brand Portal.

* In de vervolgkeuzelijst **[!UICONTROL Smart Collections]** zijn slechts tien opgeslagen verzamelingen zichtbaar.

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


### Bekende problemen {#known-issues}

Deze release bevat de volgende bekende problemen:

* De gebruikers kunnen zich niet aanmelden bij Brand Portal tijdens de migratie van hun bestaande organisatie.

   De actieve gebruikers die zijn aangemeld bij Brand Portal, kunnen echter blijven werken tot hun huidige sessie verloopt.

* Bij het navigeren van Brand Portal naar Admin Console zien de beheerders mogelijk een extra scherm om de organisatie te selecteren.

* Gebruikers kunnen het toegepaste schema voor metagegevens niet uit een map verwijderen.


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

## Gecertificeerde Platforms {#certified-platforms}

Als u wilt controleren welke platforms zijn gecertificeerd voor uitvoering met deze versie van Brand Portal, raadpleegt u de kolom **Ondersteuning voor voor voor touch geoptimaliseerde interface** in de tabel in de sectie **Ondersteunde browsers voor ontwerpgebruikersinterface** van [Technische vereisten](https://experienceleague.adobe.com/docs/experience-manager-65/deploying/introduction/technical-requirements.html).

## Koppelingen {#links}

* [Adobe Experience Manager-productpagina op adobe.com](https://business.adobe.com/in/products/experience-manager/adobe-experience-manager.html)
* [Assets Brand Portal-documentatie](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/home.html)

## Toegang tot en ondersteuning voor producten (beperkt aantal sites) {#product-access-and-support-restricted-sites}

Deze sites zijn alleen beschikbaar voor klanten. Neem contact op met uw Adobe-accountmanager als u een klant bent en toegang nodig hebt.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support](https://helpx.adobe.com/contact.html)
-->
