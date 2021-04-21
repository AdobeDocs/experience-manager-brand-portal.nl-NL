---
title: Asset Sourting in Brand Portal
seo-title: Asset Sourting in Brand Portal
description: Bekijk de functie voor het aanschaffen van bedrijfsmiddelen die beschikbaar is in de Adobe Experience Manager Assets Brand Portal.
seo-description: Bekijk de functie voor het aanschaffen van bedrijfsmiddelen die beschikbaar is in de Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
sub-product: elementen
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
exl-id: 2c132a7a-ed10-4856-8378-67939167ea60
translation-type: tm+mt
source-git-commit: e8bb1149582329f5304bda7e5e67e8dcc27cfc7b
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# Overzicht van Asset Souring {#overview-asset-sourcing-in-bp}

**Met Asset** Sourcingkunnen de AEM (beheerders/gebruikers zonder beheer) nieuwe mappen maken met een extra eigenschap  **Asset** Contribution, zodat de nieuwe map die is gemaakt, kan worden verzonden door de gebruikers van de Brand Portal. Dit leidt automatisch tot een werkschema dat tot twee extra subomslagen, genoemd **SHARED** en **NEW**, binnen de pas gecreëerde **Bijdrage** omslag leidt. De AEM beheerder bepaalt dan het vereiste door een kort over de types van activa te uploaden die aan de bijdrageomslag, evenals een reeks basislijnactiva, aan **SHARED** omslag moeten worden toegevoegd om ervoor te zorgen de gebruikers van BP de verwijzingsinformatie hebben zij nodig. De beheerder kan de actieve gebruikers van het Portaal van het Merk dan toegang tot de bijdrageomslag verlenen alvorens de pas gecreëerde **omslag** aan het Portaal van het Merk te publiceren. Zodra de gebruiker klaar is met het toevoegen van inhoud in de map **NEW**, kunnen zij de bijdragemap weer publiceren naar de AEM auteursomgeving. Het kan enkele minuten duren voordat de import is voltooid en de nieuw gepubliceerde inhoud in AEM Assets wordt weerspiegeld.

Bovendien blijft alle bestaande functionaliteit ongewijzigd. Gebruikers van het Brand Portal kunnen middelen weergeven, zoeken en downloaden vanuit de bijdragemap en vanuit de andere toegestane mappen. En beheerders kunnen de bijdragemap verder delen, eigenschappen wijzigen en elementen toevoegen aan verzamelingen.

## Vereisten {#prerequisites}

* AEM Assets als Cloud Service-instantie, AEM Assets 6.5.2 of hoger.
* Zorg ervoor dat uw AEM Assets-exemplaar is geconfigureerd met Brand Portal. Zie [AEM Assets configureren met Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
* Zorg ervoor dat uw Poorthuurder van het Merk met één de auteursinstantie van AEM Assets wordt gevormd.

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![Brand Portal Asset Sourting](assets/asset-sourcing.png)


>[!NOTE]
>
>Er is een bekend probleem in AEM Assets 6.5.4. Gebruikers van het Brand Portal kunnen de middelen van de map met bijdragen niet naar AEM Assets publiceren bij de upgrade naar de Adobe Developer Console.
>
>De kwestie is vastgelegd in AEM 6.5.5. U kunt uw AEM Assets-instantie upgraden naar het nieuwste servicepack AEM 6.5.5 en [uw configuraties upgraden](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) op de Adobe Developer Console.
>
>Voor directe oplossing op AEM 6.5.4, wordt het geadviseerd [hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) te downloaden en op uw auteursinstantie te installeren.

## Asset Sourting {#configure-asset-sourcing} configureren

**Asset** Sourcingis geconfigureerd vanuit de AEM Assets-auteurinstantie. De beheerders kunnen de configuratie van de de eigenschapmarkering van de Levering van Activa van **AEM de Configuratie van de Console van het Web** toelaten en de actieve lijst van gebruikers van het Portaal van het Merk in **AEM Assets** uploaden.

>[!NOTE]
>
>Asset Sourcing is standaard ingeschakeld op AEM Assets als Cloud Service. De AEM beheerder kan de actieve gebruikers van het Portaal van het Merk direct uploaden om hen toegang tot de eigenschap van de Activa te verlenen die.

>[!NOTE]
>
>Voordat u met de configuratie begint, moet u ervoor zorgen dat uw AEM Assets-instantie is geconfigureerd met Brand Portal. Zie [AEM Assets configureren met Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

In de volgende video ziet u hoe u Asset Sourcing configureert op uw AEM Assets-auteurinstantie:

>[!VIDEO](https://video.tv.adobe.com/v/29771)

### Asset Souring {#enable-asset-sourcing} inschakelen

AEM beheerders kunnen de de eigenschapmarkering van de Levering van Activa van binnen de Configuratie van de Console van het AEM Web (a.k.a de Manager van de Configuratie) toelaten.

>[!NOTE]
>
>Deze stap is niet van toepassing voor AEM Assets als Cloud Service.


**Asset Sourcing inschakelen:**
1. Meld u aan bij de AEM Assets-auteur en open Configuration Manager.
Standaard-URL: http:// localhost:4502/system/console/configMgr.
1. Zoek met het trefwoord **Asset Sourcing** naar **[!UICONTROL Asset Sourcing Feature Flag Config]**.
1. Klik **[!UICONTROL Asset Sourcing Feature Flag Config]** om het configuratievenster te openen.
1. Schakel het selectievakje **[!UICONTROL feature.flag.active.status]** in.
1. Klik op **[!UICONTROL Save]**.

![](assets/enable-asset-sourcing.png)

### Lijst met gebruikers van Brand Portal {#upload-bp-user-list} uploaden

AEM beheerders kunnen het CSV-bestand (Brand Portal-gebruikersconfiguratiebestand) uploaden dat een actieve gebruikerslijst voor Brand Portal in AEM Assets bevat. Een bijdragemap kan alleen worden gedeeld met de actieve gebruikers van het Brand Portal die zijn gedefinieerd in de gebruikerslijst. De beheerder kan ook nieuwe gebruikers toevoegen aan het configuratiebestand en de gewijzigde gebruikerslijst uploaden.

>[!NOTE]
>
>De indeling van het CSV-bestand is gelijk aan de indeling die wordt ondersteund in Admin Console voor het importeren van bulkgebruikers. E-mail, voornaam en achternaam zijn verplicht.

De beheerders kunnen nieuwe gebruikers in AEM Admin Console toevoegen, zie [Gebruikers beheren](brand-portal-adding-users.md) voor gedetailleerde informatie. Na het toevoegen van gebruikers in Admin Console, kunnen deze gebruikers aan het dossier van de de gebruikersconfiguratie van het Portaal van het Merk worden toegevoegd en dan toestemming toegewezen om tot de bijdrageomslag toegang te hebben.

**Ga als volgt te werk om de gebruikerslijst van Brand Portal te uploaden:**
1. Meld u aan bij uw AEM Assets-exemplaar.
1. Navigeer in het deelvenster **Gereedschappen** naar **[!UICONTROL Assets]** > **[!UICONTROL Brand Portal Users]**.

1. Het venster Contribuanten uploaden naar Brand Portal wordt geopend.
Blader van uw lokale computer en upload **configuratiebestand (.csv)** met de actieve gebruikerslijst van het Merkortaal.
1. Klik op **[!UICONTROL Save]**.

   ![](assets/upload-user-list2.png)


Beheerders kunnen toegang tot specifieke gebruikers bieden vanuit deze gebruikerslijst terwijl ze een bijdragemap configureren. Alleen de gebruikers die zijn toegewezen aan een map met bijdragen hebben toegang tot de map met bijdragen en publiceren middelen van Brand Portal naar AEM Assets.

## Zie ook {#reference-articles}

* [Contribute-map voor Brand Portal configureren en publiceren](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [Bijdragemap publiceren naar AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
