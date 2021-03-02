---
title: Release-opmerkingen
seo-title: Release-opmerkingen
description: Bekijk de functies, verbeteringen, belangrijke problemen die zijn opgelost en bekende problemen in de Adobe Experience Manager Assets Brand Portal versie 2021.02.0.
seo-description: Bekijk de verbeteringen, kritieke problemen die zijn opgelost en bekende problemen in de Adobe Experience Manager Assets Brand Portal versie 2021.02.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 302bbf441453a760fe53d981a61b2eb014ebd1f0
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 4%

---


# Releaseopmerkingen {#release-notes}

Bekijk de nieuwe functies, verbeteringen, belangrijke problemen die zijn opgelost en bekende problemen in de Adobe Experience Manager Assets Brand Portal versie 2021.02.0.

## Informatie opheffen {#release-information}

| Product | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versie | 2021 02,0 |
| Date | februari 2021 |

## Overzicht {#overview}

Met Adobe Experience Manager (AEM) Assets Brand Portal kunt u eenvoudig goedgekeurde creatieve middelen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten. Het draagt bij tot een efficiëntere verdeling van activa, versnelt de marktintroductie van activa en vermindert het risico van niet-naleving en ongeoorloofde toegang. Merkportal biedt gebruikers de mogelijkheid om in door het bedrijf goedgekeurde indelingen te zoeken, te bekijken, voor te vertonen, te downloaden en te exporteren, altijd en overal.

## Nieuwe functies in 2021.02.0 {#whats-new-in-2021.02.0}

### Nieuwe functies {#new-features}

Deze release bevat de volgende nieuwe functies:

* De functie Asset Sourcing is nu als Cloud Service beschikbaar op AEM Assets. Hiermee kunnen gebruikers van het Brand Portal elementen uploaden naar de mappen met toegestane bijdragen en de map met bijdragen publiceren van Brand Portal naar AEM Assets als instantie van Cloud Service.

* Er is een extra **[!UICONTROL Asset Download]**-instelling toegevoegd onder **[!UICONTROL Download Settings]**. Er wordt een aparte map voor elk element gemaakt tijdens het downloaden van de mappen, verzamelingen of het bulkdownloaden van elementen. Zie [downloadinstellingen](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download).

<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions. See [steps to download assets from Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog. See [download assets from asset details page](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page).
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

### Verbeteringen {#enhancements}

Deze release bevat de volgende verbeteringen:

* Voor het downloaden van mappen wordt voor elk element een aparte map gemaakt met behulp van een gedeelde koppeling, ongeacht **[!UICONTROL Download Settings]**.
* Het Brand Portal **[!UICONTROL Usage Report]** is gewijzigd om alleen de actieve gebruikers van het Brand Portal weer te geven.

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Kritieke problemen opgelost {#critical-issues-fixed}

Deze release bevat oplossingen voor de volgende kritieke problemen:

* Als alleen de originele elementen worden gedownload, weerspiegelt het element de eigen extensie en wordt het pas geopend als de extensie handmatig wordt gewijzigd in zip.
* De gebruikersinterface van de verzamelingsmap reageert niet wanneer u op de navigatiepijl klikt.
* **[!UICONTROL Create]** Deze knop is zichtbaar in de  **[!UICONTROL Column]** weergave, zelfs als de mappen leeg zijn.
* **[!UICONTROL Omni search]** ontbreekt met een 414 foutenmelding (verzoek-URI Te lang) als de verzender terwijl het toegang tot van de instantie van het Portaal van het Merk wordt overgeslagen.
* Er wordt een lege ZIP-map gedownload als het element een komma (`,`) in de bestandsnaam bevat.
* Gebruikers van viewers kunnen gebruikers toevoegen aan de verzameling die ze hebben gemaakt.
* Er is sprake van inconsistent gedrag wanneer een element (miniatuur of webuitvoering) wordt gedownload via een koppeling voor delen.

Zie [nieuwe functies in Brand Portal 2021.02.0](whats-new.md).

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

De gebruikersinterface van het Merk Portal is beschikbaar in de volgende talen:

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

Als u wilt controleren welke platforms zijn gecertificeerd voor uitvoering met deze versie van Brand Portal, raadpleegt u de kolom **Ondersteuning voor voor voor touch geoptimaliseerde interface** in de tabel in de sectie **Ondersteunde browsers voor ontwerpgebruikersinterface** van [Technische vereisten](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Koppelingen {#links}

* [Adobe Experience Manager-productpagina op adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Merknaam van bedrijfsmiddelen — Documentatie](https://helpx.adobe.com/nl/experience-manager/brand-portal/user-guide.html)

## Toegang tot en ondersteuning voor producten (beperkt aantal sites) {#product-access-and-support-restricted-sites}

Deze sites zijn alleen beschikbaar voor klanten. Neem contact op met uw Adobe-accountmanager als u een klant bent en toegang nodig hebt.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [Producttoegang](https://login.marketing.adobe.com)

* [Adobe Klantenservice](https://helpx.adobe.com/contact.html)
