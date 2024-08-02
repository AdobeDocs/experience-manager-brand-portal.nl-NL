---
title: Algemeen huurconfiguraties beheren
description: Configureer downloadversnelling, maak van openbare slimme verzamelingen, maak van openbare verzamelingen en stel beheerders in staat elementen op huurders te verwijderen.
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 5607be8e-0a7f-4692-b71b-5f66eb9ac5ee
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---

# Algemene huurdersconfiguraties beheren {#administer-general-tenant-configurations}

Met Experience Manager Assets Brand Portal kunnen organisaties de volgende mogelijkheden configureren voor specifieke huurders:

* Verwijderen van bedrijfsmiddelen door beheerders
* Openbare collectie maken door gebruikers die geen beheerder zijn
* Creatie van slimme openbare verzamelingen door gebruikers zonder beheerdersrechten
* De bovenliggende hiërarchie van gedeelde mappen is zichtbaar voor niet-beheerders

Deze configuraties zijn opgegeven als **[!UICONTROL General Settings]** -configuraties in het deelvenster met beheergereedschappen.

![](assets/general-config.png)

**A** - Configuratie om beheerders te laten activa van Brand Portal schrappen. (Standaard is ingeschakeld)

**B** - Configuratie om gebruikers te laten niet-admin openbare inzamelingen tot stand brengen. (Standaard is ingeschakeld)

**C** - Configuratie om gebruikers te laten niet-admin tot openbare slimme inzamelingen leiden. (Standaard is ingeschakeld)

**D** - Configuratie om de omslaghiërarchie (van de wortel) van gedeelde omslagen aan niet-admingebruikers (Editors, Kijkers, de Gebruikers van de Gast) te tonen. (Standaard is uitgeschakeld)

## Algemene configuraties inschakelen of uitschakelen {#enable-disable-general-configurations}

Om elk van deze configuraties in of uit te schakelen:

1. Meld u aan met beheerdersrechten.
1. Selecteer het logo van de Experience Manager voor toegang tot de beheergereedschappen op de werkbalk boven in het scherm.
1. Selecteer in het deelvenster met beheergereedschappen de optie **[!UICONTROL General]** om de pagina **[!UICONTROL General Settings]** te openen.
1. Gebruik de respectieve knevelschakelaar om het even welke Algemene configuraties toe te laten of onbruikbaar te maken.
1. **[!UICONTROL Save]** de wijzigingen.
1. Log uit zodat de wijzigingen van kracht kunnen worden.

## Beheerders toestaan elementen uit Brand Portal te verwijderen {#allow-admin-users-to-delete-assets-from-brand-portal}

Met de configuratie van **[!UICONTROL Allow users to delete]** kunnen organisaties gebruikers met beheerdersrechten toestaan (of beperken) elementen en mappen uit Brand Portal te verwijderen.

## Openbare collecties maken door niet-beheerders toestaan {#allow-public-collections-creation-by-non-admins}

[[!UICONTROL Allow public collections creation]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) -configuratie bepaalt of niet-beheerders openbare verzamelingen kunnen maken op Brand Portal. De configuratie is standaard ingeschakeld. Door de configuratie onbruikbaar te maken, kunnen de organisaties het hebben van talrijke openbare inzamelingen op hun portaal verhinderen zodat de systeemruimte kan worden bewaard.

## Maken van openbare slimme verzamelingen door niet-beheerders toestaan {#allow-public-smart-collections-creation-by-non-admins}

[[!UICONTROL Allow public smart collections creation]](../using/brand-portal-searching.md#main-pars-header-500620467) configuratie controleert of niet-beheerders hun onderzoeken als slimme inzamelingen kunnen bewaren en hen openbaar voor die huurder maken. De configuratie is standaard ingeschakeld. Door de configuratie uit te schakelen, kunnen organisaties voorkomen dat een enorm aantal openbare slimme verzamelingen wordt gemaakt door gebruikers die geen beheerder zijn op de Brand Portal van de organisatie.

<!-- 
## Allow download acceleration {#allow-download-acceleration}

[[!UICONTROL Allow download acceleration]](../using/accelerated-download.md) configuration lets the organizations to allow accelerated downloads of assets from Brand Portal and shared links, by integrating with IBM Aspera Connect that is an install-on-demand application. The application uses proprietary technology to remove TCP overheads.
-->

## Maphiërarchie inschakelen {#enable-folder-hierarchy}

Met de configuratie [[!UICONTROL Enable Folder Hierarchy]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) kunnen beheerders bepalen hoe de gedeelde mappen worden weergegeven door gebruikers die geen beheerder zijn (Editors, Viewers en Gastgebruikers) nadat ze zich hebben aangemeld.
