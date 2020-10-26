---
title: Release-opmerkingen
seo-title: Release-opmerkingen
description: Bekijk de functies, verbeteringen, belangrijke problemen die zijn opgelost en bekende problemen in de Adobe Experience Manager Assets Brand Portal versie 2020.10.0.
seo-description: Bekijk de verbeteringen, kritieke problemen die zijn opgelost en bekende problemen in de Adobe Experience Manager Assets Brand Portal versie 2020.10.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: df378757f901a92de7003790651f623dcb92a4e3
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 5%

---


# Releaseopmerkingen {#release-notes}

Bekijk de nieuwe functies, verbeteringen, belangrijke problemen die zijn opgelost en bekende problemen in de Adobe Experience Manager Assets Brand Portal versie 2020.10.0.

## Geen informatie {#release-information}

| Product | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versie | 2020.10.0 |
| Date | Oktober 2020 |

## Overzicht {#overview}

Met Adobe Experience Manager (AEM) Assets Brand Portal kunt u eenvoudig goedgekeurde creatieve middelen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten. Het draagt bij tot een efficiëntere verdeling van activa, versnelt de marktintroductie van activa en vermindert het risico van niet-naleving en ongeoorloofde toegang. Merkportal biedt gebruikers de mogelijkheid om in door het bedrijf goedgekeurde indelingen te zoeken, te bekijken, voor te vertonen, te downloaden en te exporteren, altijd en overal.

## Nieuwe functies in 2020.10.0 {#whats-new-in-2020.10.0}

### Nieuwe functies {#new-features}

Deze release bevat de volgende nieuwe functies:

* Het **[!UICONTROL Download]** dialoogvenster wordt vernieuwd in een lijstweergave met aanvullende opties om de uitvoeringen uit te sluiten die niet vereist zijn, dezelfde set regels toe te passen voor vergelijkbare elementtypen en de geselecteerde elementuitvoeringen te downloaden.

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

* Navigatie naar de pagina&#39;s **[!UICONTROL Files]**, **[!UICONTROL Collections]** en **[!UICONTROL Shared Links]** is nu mogelijk vanaf alle pagina&#39;s van het Brand Portal met één klik.

* Met het **[!UICONTROL Renditions]** deelvenster op de pagina met elementdetails kunnen de gebruikers van het Brand Portal het oorspronkelijke element en (of) specifieke elementen selecteren en deze rechtstreeks downloaden vanuit het **[!UICONTROL Renditions]** deelvenster zonder dat ze het **[!UICONTROL Download]** dialoogvenster hoeven te openen.

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

* Naast de bestaande **[!UICONTROL Download]** configuraties, kunnen de beheerders van het Portaal van het Merk toestemmingen voor verschillende groep gebruikers ook vormen om het originele activa en zijn vertoningen van de pagina van de activadetails te bekijken en (of) te downloaden. Deze configuraties bepalen wie toegang heeft tot de elementuitvoeringen en (of deze kan downloaden).

### Verbeteringen {#enhancements}

Deze release bevat de volgende verbeteringen:

* De drempel van sessietime-out voor de gastgebruikers is verlaagd van 2 uur naar 15 minuten.
* De extra **[!UICONTROL View pages]** optie is verwijderd voor PDF&#39;s die uit meerdere pagina&#39;s bestaan, omdat de gebruiker de PDF-pagina&#39;s nu kan weergeven vanuit de Adobe Document Cloud Viewer.


<!--
### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issue:

* The users are not able to view the PDF pages if the PDF contains sub assets.
-->

### Bekende problemen {#known-issues}

Deze release bevat de volgende bekende uitgave:

* In de zoekopdracht op de **[!UICONTROL Asset Reports]** werkbalk ziet u de verwerking in de productinterface zonder zoekresultaat.
* De video-DM-codes zijn niet zichtbaar voor gebruikers die geen beheerder zijn, op de pagina met elementdetails.
* De uitlijning van de grootte van afzonderlijke elementuitvoeringen en de totale downloadgrootte wordt vervormd in het dialoogvenster Downloaden.



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

Als u wilt weten welke platforms zijn gecertificeerd voor uitvoering met deze versie van Brand Portal, raadpleegt u de kolom **Ondersteuning voor voor voor touch geoptimaliseerde interface** in de tabel in het gedeelte **Ondersteunde browsers voor ontwerpen van gebruikersinterface** van [Technische vereisten](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

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
