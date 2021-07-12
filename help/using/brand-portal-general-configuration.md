---
title: Algemene huurdersconfiguraties beheren
seo-title: Algemene huurdersconfiguraties beheren
description: Configureer downloadversnelling, maak van openbare slimme verzamelingen, maak van openbare verzamelingen en stel beheerders in staat elementen op huurders te verwijderen.
seo-description: Configureer downloadversnelling, maak van openbare slimme verzamelingen, maak van openbare verzamelingen en stel beheerders in staat elementen op huurders te verwijderen.
uuid: 3c46cd7c-c38b-4bc7-b566-93f977bc8227
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f4c237bc-f6a4-4bc4-af56-3d9c3027daf4
role: Admin
exl-id: 5607be8e-0a7f-4692-b71b-5f66eb9ac5ee
source-git-commit: 26b009fec800d9b437bde5838009c71b1b3b7ac6
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Algemene huurdersconfiguraties beheren {#administer-general-tenant-configurations}

AEM Assets Brand Portal staat organisaties toe om de volgende mogelijkheden voor specifieke huurders te vormen:

* Verwijderen van bedrijfsmiddelen door beheerders
* Openbare collectie maken door gebruikers die geen beheerder zijn
* Creatie van slimme openbare verzamelingen door gebruikers zonder beheerdersrechten
* Bovenliggende hiërarchie van gedeelde mappen zichtbaar voor gebruikers zonder beheerdersrechten

Deze configuraties zijn opgegeven als **[!UICONTROL General Settings]** configuraties in het deelvenster met beheergereedschappen.

![](assets/general-config.png)

****   AConfiguration om beheerders toe te staan om activa van Brand Portal te schrappen. (Standaard is ingeschakeld)

****   BConfiguration om de gebruikers niet-admin toe te staan om openbare inzamelingen tot stand te brengen. (Standaard is ingeschakeld)

**Configuratie**   waarmee gebruikers die geen beheerder zijn, openbare slimme verzamelingen kunnen maken. (Standaard is ingeschakeld)

****  DConfiguration om maphiërarchie (van de wortel) van gedeelde omslagen aan niet-admingebruikers (Editors, Kijkers, de Gebruikers van de Gast) te tonen. (Standaard is uitgeschakeld)

## Algemene configuraties inschakelen/uitschakelen {#enable-disable-general-configurations}

Om elk van deze configuraties toe te laten/onbruikbaar te maken:

1. Meld u aan met beheerdersrechten.
1. Selecteer het AEM logo voor toegang tot de beheergereedschappen op de werkbalk boven in het scherm.
1. Selecteer **[!UICONTROL General]** in het deelvenster met beheergereedschappen om de pagina **[!UICONTROL General Settings]** te openen.
1. Gebruik de respectieve knevelschakelaar om het even welke Algemene configuraties toe te laten/onbruikbaar te maken.
1. **[!UICONTROL Save]** de wijzigingen.
1. Afmelden om de wijzigingen van kracht te laten worden.

## Beheerders toestaan elementen uit Brand Portal te verwijderen {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL Allow users to delete]** Met configuratie kunnen organisaties gebruikers met beheerdersrechten toestaan (of beperken) elementen en mappen uit Brand Portal te verwijderen.

## Openbare collecties maken door niet-beheerders toestaan {#allow-public-collections-creation-by-non-admins}

[[!UICONTROL Allow public collections creation]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) De configuratie controleert of niet-beheerders openbare inzamelingen op Brand Portal kunnen tot stand brengen. De configuratie is standaard ingeschakeld. Door de configuratieorganisaties onbruikbaar te maken kunnen het hebben van talrijke openbare inzamelingen op hun portaal verhinderen zodat de systeemruimte kan worden bewaard.

## Maken van openbare slimme verzamelingen door niet-beheerders toestaan {#allow-public-smart-collections-creation-by-non-admins}

[[!UICONTROL Allow public smart collections creation]](../using/brand-portal-searching.md#main-pars-header-500620467) de configuratie controleert of niet-beheerders hun onderzoeken als slimme inzamelingen kunnen bewaren en hen openbaar voor die huurder maken. De configuratie is standaard ingeschakeld. Door de configuratieorganisaties onbruikbaar te maken kan het hebben van een enorm aantal openbare slimme inzamelingen verhinderen die door gebruikers niet-admin op de Brand Portal van de organisatie worden gecreeerd.

<!-- 
## Allow download acceleration {#allow-download-acceleration}

[[!UICONTROL Allow download acceleration]](../using/accelerated-download.md) configuration lets the organizations to allow accelerated downloads of assets from Brand Portal and shared links, by integrating with IBM Aspera Connect that is an install-on-demand application. The application uses proprietary technology to remove TCP overheads.
-->

## Maphiërarchie inschakelen {#enable-folder-hierarchy}

[[!UICONTROL Enable Folder Hierarchy]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) De configuratie staat de beheerders toe om te controleren hoe de gebruikers niet-admin (Editors, Kijkers, en de Gebruikers van de Gast) de gedeelde omslagen na het programma openen zien.
