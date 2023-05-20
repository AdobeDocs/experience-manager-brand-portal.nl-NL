---
title: Asset Sourting in Brand Portal
seo-title: Asset Sourcing in Brand Portal
description: Bekijk de functie voor het aanschaffen van bedrijfsmiddelen die in de Adobe Experience Manager Assets Brand Portal wordt uitgebracht.
seo-description: Get an insight into the asset sourcing feature released in the Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
sub-product: assets
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
exl-id: 2c132a7a-ed10-4856-8378-67939167ea60
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Overzicht van Asset Souring {#overview-asset-sourcing-in-bp}

**Asset Sourting** Hiermee kunnen de Experience Manager Assets-gebruikers (beheerders/gebruikers die geen beheerder zijn) nieuwe mappen maken met een extra **Bijdrage activa** , zodat de nieuwe map die u hebt gemaakt, kan worden verzonden door Brand Portal-gebruikers. Dit activeert automatisch een workflow die twee extra submappen maakt, genaamd **GEDEELD** en **NIEUW**, binnen de nieuwe **Bijdrage** map. De beheerder bepaalt dan het vereiste door een kort overzicht van de types van activa te uploaden die aan de bijdrageomslag, evenals een reeks basiselementen, aan de **GEDEELD** om ervoor te zorgen dat BP-gebruikers beschikken over de benodigde informatie. De beheerder kan actieve Brand Portal-gebruikers dan toegang verlenen tot de bijdragemap voordat het zojuist gemaakte **Bijdrage** naar Brand Portal. Wanneer de gebruiker klaar is met het toevoegen van inhoud in de **NIEUW** , kunnen zij de bijdrageomslag terug naar het auteursmilieu van de Experience Manager publiceren. Het kan enkele minuten duren voordat de import is voltooid en de nieuw gepubliceerde inhoud in Experience Manager Assets wordt weerspiegeld.

Bovendien blijft alle bestaande functionaliteit ongewijzigd. Brand Portal-gebruikers kunnen middelen weergeven, zoeken en downloaden vanuit de map met bijdragen en vanuit de andere toegestane mappen. En beheerders kunnen de bijdragemap verder delen, eigenschappen wijzigen en elementen toevoegen aan verzamelingen.

![Brand Portal Asset Sourting](assets/asset-sourcing.png)

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

## Vereisten {#prerequisites}

* as a Cloud Service Experience Manager Assets-instantie, Experience Manager Assets 6.5.2 of hoger.
* Controleer of uw Experience Manager Assets-exemplaar is geconfigureerd met Brand Portal. Zie, [Experience Manager Assets configureren met Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

<!--
* Ensure that your Brand Portal tenant is configured with one AEM Assets author instance.
-->

>[!NOTE]
>
>De functie Asset Sourcing is standaard ingeschakeld op Experience Manager Assets as a Cloud Service, Experience Manager Assets 6.5.9 en hoger.
>
>De bestaande configuraties zullen aan de vroegere versies blijven werken.

>[!NOTE]
>
>Er is een bekend probleem in Experience Manager Assets 6.5.4. Brand Portal-gebruikers kunnen de middelen van de map met bijdragen niet naar Experience Manager Assets publiceren bij de upgrade naar Adobe Developer Console.
>
>Het probleem is opgelost in Experience Manager Assets 6.5.5. U kunt uw Experience Manager Assets-exemplaar upgraden naar het nieuwste servicepakket en [upgrade uitvoeren van uw configuraties](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) op Adobe Developer Console.

<!--

>For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your author instance.
-->

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

Experience Manager Assets-beheerders kunnen het Brand Portal-gebruikersconfiguratiebestand (.csv) met de actieve Brand Portal-gebruikerslijst in Experience Manager Assets uploaden om ze toegang te geven tot de functie voor het zoeken naar middelen.

Een bijdragemap kan alleen worden gedeeld met de actieve Brand Portal-gebruikers die zijn gedefinieerd in de gebruikerslijst. De beheerder kan ook nieuwe gebruikers toevoegen aan het configuratiebestand en de gewijzigde gebruikerslijst uploaden.

>[!NOTE]
>
>Controleer of uw Experience Manager Assets-exemplaar is geconfigureerd met Brand Portal. Zie, [Experience Manager Assets configureren met Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

>[!NOTE]
>
>De indeling van het CSV-bestand is gelijk aan de indeling die wordt ondersteund in Admin Console voor het importeren van bulkgebruikers. E-mail, voornaam en achternaam zijn verplicht.

De beheerders kunnen nieuwe gebruikers in Admin Console toevoegen, zie [Gebruikers beheren](brand-portal-adding-users.md) voor nadere informatie. Na het toevoegen van gebruikers in Admin Console, kunnen deze gebruikers aan het dossier van de de gebruikersconfiguratie van Brand Portal worden toegevoegd en dan toestemming worden toegewezen om tot de bijdrageomslag toegang te hebben.

**Brand Portal-gebruikerslijst uploaden:**

1. Meld u aan bij uw Experience Manager Assets-exemplaar.
1. Van de **Gereedschappen**  deelvenster, navigeren naar **[!UICONTROL Assets]** > **[!UICONTROL Brand Portal Users]**.

1. Het venster Brand Portal Upload Contributors wordt geopend.
Bladeren op uw lokale computer en uploaden **configuratiebestand (.csv)** met de actieve gebruikerslijst van Brand Portal.
1. Klik op **[!UICONTROL Save]**.

   ![](assets/upload-user-list2.png)


Beheerders kunnen toegang tot specifieke gebruikers bieden vanuit deze gebruikerslijst terwijl ze een bijdragemap configureren. Alleen de gebruikers die zijn toegewezen aan een map met bijdragen hebben toegang tot de map met bijdragen en publiceren middelen van Brand Portal naar Experience Manager Assets.

## Zie ook {#reference-articles}

* [Contribute-map voor Brand Portal configureren en publiceren](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [Bijdragemap publiceren naar Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
