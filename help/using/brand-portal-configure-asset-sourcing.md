---
title: Asset Souring configureren
seo-title: Asset Souring configureren
description: Krijg inzicht in het vormen van activa het bronbepalend eigenschap in AEM Assets.
seo-description: Krijg inzicht in het vormen van activa het bronbepalend eigenschap in AEM Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 21ead6dac38429a5b427f4c92150c4bee47efc76
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 1%

---


# Asset Souring configureren {#configure-asset-sourcing}

AEM-beheerders kunnen **Asset Sourcing** configureren vanuit de AEM-auteur. De beheerder laat de configuratie van de de eigenschapmarkering van de Levering van Activa van de Configuratie **van de Console van** AEM toe Web en uploadt de actieve lijst van gebruikers van het Portaal van het Merk in **AEM Assets**.

>[!NOTE]
>
>Alvorens u met de configuratie begint, zorg ervoor dat uw instantie van AEM Assets met het Portaal van het Merk wordt gevormd. See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md).


In de volgende video ziet u hoe u Asset Sourcing kunt configureren op uw AEM-auteurinstantie:

>[!VIDEO](https://video.tv.adobe.com/v/29771)

## Asset Souring inschakelen {#enable-asset-sourcing}

AEM-beheerders kunnen Asset Sourcing inschakelen vanuit de configuratie van de AEM-webconsole (ook bekend als Configuration Manager).

**Asset Sourcing inschakelen:**
1. Meld u aan bij de AEM-auteur-instantie en open Configuration ManagerDefault URL: http:// localhost:4502/system/console/configMgr
1. Zoeken met het trefwoord **Asset Sourcing** om te zoeken **[!UICONTROL Asset Sourcing Feature Flag Config]**
1. Klik **[!UICONTROL Asset Sourcing Feature Flag Config]** om het configuratievenster te openen
1. Selectievakje inschakelen **[!UICONTROL feature.flag.active.status]**
1. Klik op **[!UICONTROL Save]**.

![](assets/enable-asset-sourcing.png)

## Lijst met gebruikers van Brand Portal uploaden {#upload-bp-user-list}

AEM-beheerders kunnen het CSV-bestand (Brand Portal-gebruikersconfiguratiebestand) uploaden dat een actieve gebruikerslijst voor het Merkortaal bevat in AEM Assets. Een bijdragemap kan alleen worden gedeeld met de actieve gebruikers van het Brand Portal die zijn gedefinieerd in de gebruikerslijst. Beheerders kunnen ook nieuwe gebruikers toevoegen aan het configuratiebestand en de gewijzigde gebruikerslijst uploaden.

>[!NOTE]
>
>De indeling van het CSV-bestand is gelijk aan de indeling die door de Admin Console wordt ondersteund bij het importeren van bulkgebruikers. E-mail, voornaam en achternaam zijn verplicht.

Beheerders kunnen nieuwe gebruikers toevoegen in AEM Admin Console. Raadpleeg Gebruikers [](brand-portal-adding-users.md) beheren voor meer informatie. Na het toevoegen van gebruikers in Admin Console, kunnen deze gebruikers aan het dossier van de de gebruikersconfiguratie van het Portaal van het Merk worden toegevoegd en dan toestemming toegewezen om tot de bijdrageomslag toegang te hebben.

**Ga als volgt te werk om de gebruikerslijst van Brand Portal te uploaden:**
1. Meld u aan bij de instantie van uw AEM-auteurStandaard-URL: http:// localhost:4502/aem/start.html
1. Ga vanuit het deelvenster **** ![](assets/tools.png)Tools naar **[!UICONTROL Assets > Brand Portal Users]**
   ![](assets/upload-user-list1.png)
1. Het venster Contribuanten uploaden naar Brand Portal wordt geopend.
Blader vanaf uw lokale computer en upload het **configuratiebestand** (.csv) met de actieve gebruikerslijst van het Brand Portal.
1. Klik op **[!UICONTROL Save]**.
   ![](assets/upload-user-list2.png)


Beheerders kunnen toegang tot specifieke gebruikers/groepen bieden vanuit deze gebruikerslijst tijdens het configureren van de bijdragemap.

Zie Contribute-map [](brand-portal-contribution-folder.md)configureren voor meer informatie.
