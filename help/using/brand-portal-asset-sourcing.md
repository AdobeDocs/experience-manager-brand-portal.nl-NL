---
title: Asset Sourting in Brand Portal
seo-title: Asset Sourting in Brand Portal
description: Bekijk de functie voor het aanschaffen van bedrijfsmiddelen die in de Adobe Experience Manager Assets Brand Portal wordt uitgebracht.
seo-description: Bekijk de functie voor het aanschaffen van bedrijfsmiddelen die in de Adobe Experience Manager Assets Brand Portal wordt uitgebracht.
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
source-git-commit: bfbc90e3cdc9e3fc72a6e54f6730922753585471
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# Overzicht van Asset Souring {#overview-asset-sourcing-in-bp}

**Met Asset** Sourcingkunnen de AEM (beheerders/gebruikers zonder beheer) nieuwe mappen maken met een extra  **Asset** Contribution-eigenschap, zodat de nieuwe map die is gemaakt, kan worden verzonden door de Brand Portal-gebruikers. Dit leidt automatisch tot een werkschema dat tot twee extra subomslagen, genoemd **SHARED** en **NEW**, binnen de pas gecreëerde **Bijdrage** omslag leidt. De AEM beheerder bepaalt dan het vereiste door een kort over de types van activa te uploaden die aan de bijdrageomslag, evenals een reeks basislijnactiva, aan **SHARED** omslag moeten worden toegevoegd om ervoor te zorgen de gebruikers van BP de verwijzingsinformatie hebben zij nodig. De beheerder kan actieve Brand Portal-gebruikers dan toegang tot de bijdragemap geven voordat ze de nieuwe map **Contribution** publiceren naar Brand Portal. Zodra de gebruiker klaar is met het toevoegen van inhoud in de map **NEW**, kunnen zij de bijdragemap weer publiceren naar de AEM auteursomgeving. Het kan enkele minuten duren voordat de import is voltooid en de nieuw gepubliceerde inhoud in AEM Assets wordt weerspiegeld.

Bovendien blijft alle bestaande functionaliteit ongewijzigd. Brand Portal-gebruikers kunnen middelen weergeven, zoeken en downloaden vanuit de map met bijdragen en vanuit de andere toegestane mappen. En beheerders kunnen de bijdragemap verder delen, eigenschappen wijzigen en elementen toevoegen aan verzamelingen.

![Brand Portal Asset Sourting](assets/asset-sourcing.png)

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

## Vereisten {#prerequisites}

* AEM Assets als Cloud Service-instantie, AEM Assets 6.5.2 of hoger.
* Controleer of uw AEM Assets-exemplaar is geconfigureerd met Brand Portal. Zie [AEM Assets configureren met Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

<!--
* Ensure that your Brand Portal tenant is configured with one AEM Assets author instance.
-->

>[!NOTE]
>
>De functie Asset Sourcing is standaard ingeschakeld op AEM Assets als Cloud Service, AEM Assets 6.5.9 en hoger.
>
>De bestaande configuraties zullen aan de vroegere versies blijven werken.

>[!NOTE]
>
>Er is een bekend probleem in AEM Assets 6.5.4. Brand Portal-gebruikers kunnen de middelen van de map met bijdragen niet naar AEM Assets publiceren bij de upgrade naar de Adobe Developer Console.
>
>De kwestie is vastgelegd in AEM 6.5.5. U kunt uw AEM Assets-instantie upgraden naar het nieuwste servicepack AEM 6.5.5 en [uw configuraties upgraden](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) op de Adobe Developer Console.
>
>Voor directe oplossing op AEM 6.5.4, wordt het geadviseerd [hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) te downloaden en op uw auteursinstantie te installeren.

<!--
## Configure Asset Sourcing {#configure-asset-sourcing}

**Asset Sourcing** is configured from within the AEM Assets author instance. The administrators can enable the Asset Sourcing feature flag configuration from the **AEM Web Console Configuration** and upload the active Brand Portal users list in **AEM Assets**.

>[!NOTE]
>
>Asset Sourcing is by default enabled on AEM Assets as a Cloud Service. The AEM administrator can directly upload the active Brand Portal users to allow them access to the Asset Sourcing feature.

>[!NOTE]
>
>Before you begin with the configuration, ensure that your AEM Assets instance is configured with Brand Portal. See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md). 

The following video demonstrates, how to configure Asset Sourcing on your AEM Assets author instance:

>[!VIDEO](https://video.tv.adobe.com/v/29771)
-->

<!--
### Enable Asset Sourcing {#enable-asset-sourcing}

AEM administrators can enable the Asset Sourcing feature flag from within the AEM Web Console Configuration (a.k.a Configuration Manager).

>[!NOTE]
>
>This step is not applicable for AEM Assets as a Cloud Service.


**To enable Asset Sourcing:**
1. Log in to your AEM Assets author instance and open Configuration Manager. 
Default URL: http:// localhost:4502/system/console/configMgr.
1. Search using the keyword **Asset Sourcing** to locate **[!UICONTROL Asset Sourcing Feature Flag Config]**.
1. Click **[!UICONTROL Asset Sourcing Feature Flag Config]** to open the configuration window.
1. Select the **[!UICONTROL feature.flag.active.status]** check box.
1. Click **[!UICONTROL Save]**.

![](assets/enable-asset-sourcing.png)
-->


### Lijst met Brand Portal-gebruikers uploaden {#upload-bp-user-list}

AEM beheerders kunnen het configuratiebestand (.csv) van de Brand Portal-gebruiker met de actieve Brand Portal-gebruikerslijst in AEM Assets uploaden om ze toegang te geven tot de functie Asset Sourcing.

Een bijdragemap kan alleen worden gedeeld met de actieve Brand Portal-gebruikers die zijn gedefinieerd in de gebruikerslijst. De beheerder kan ook nieuwe gebruikers toevoegen aan het configuratiebestand en de gewijzigde gebruikerslijst uploaden.

>[!NOTE]
>
>Controleer of uw AEM Assets-exemplaar is geconfigureerd met Brand Portal. Zie [AEM Assets configureren met Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

>[!NOTE]
>
>De indeling van het CSV-bestand is gelijk aan de indeling die wordt ondersteund in Admin Console voor het importeren van bulkgebruikers. E-mail, voornaam en achternaam zijn verplicht.

De beheerders kunnen nieuwe gebruikers in AEM Admin Console toevoegen, zie [Gebruikers beheren](brand-portal-adding-users.md) voor gedetailleerde informatie. Na het toevoegen van gebruikers in Admin Console, kunnen deze gebruikers aan het dossier van de de gebruikersconfiguratie van Brand Portal worden toegevoegd en dan toestemming worden toegewezen om tot de bijdrageomslag toegang te hebben.

**Brand Portal-gebruikerslijst uploaden:**
1. Meld u aan bij uw AEM Assets-exemplaar.
1. Navigeer in het deelvenster **Gereedschappen** naar **[!UICONTROL Assets]** > **[!UICONTROL Brand Portal Users]**.

1. Het venster Brand Portal Upload Contributors wordt geopend.
Blader vanaf uw lokale computer en upload **configuratiebestand (.csv)** met de actieve lijst met Brand Portal-gebruikers.
1. Klik op **[!UICONTROL Save]**.

   ![](assets/upload-user-list2.png)


Beheerders kunnen toegang tot specifieke gebruikers bieden vanuit deze gebruikerslijst terwijl ze een bijdragemap configureren. Alleen de gebruikers die zijn toegewezen aan een map met bijdragen hebben toegang tot de map met bijdragen en publiceren middelen van Brand Portal naar AEM Assets.

## Zie ook {#reference-articles}

* [Contribute-map voor Brand Portal configureren en publiceren](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [Bijdragemap publiceren naar AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
