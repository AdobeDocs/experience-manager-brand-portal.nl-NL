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
product: experience-manager
sub-product: elementen
feature: brand-portal
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: 9c937603cf325919cb49d3418b06266fa1b93cf1
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---


# Overzicht van Asset Souring {#overview-asset-sourcing-in-bp}

**Met Asset Sourcing** kunnen AEM gebruikers (beheerders/gebruikers die geen beheerder zijn) nieuwe mappen maken met een extra eigenschap **Asset Contribution** , zodat de nieuwe map die is gemaakt, toegankelijk is voor de gebruikers van de Brand Portal. Dit leidt automatisch tot een werkschema dat tot twee extra subomslagen, genoemd **GEDEELD** en **NIEUW**, binnen de pas gecreëerde omslag van de **Bijdrage** leidt. De AEM beheerder bepaalt dan het vereiste door een kort over de types van activa te uploaden die aan de bijdrageomslag, evenals een reeks basislijnactiva, aan de **GEDEELDE** omslag moeten worden toegevoegd om BP gebruikers te verzekeren hebben de verwijzingsinformatie zij nodig hebben. De beheerder kan actieve gebruikers van het Brand Portal dan toegang tot de bijdrageomslag verlenen alvorens de pas gecreëerde omslag van de **Bijdrage** aan het Portaal van het Merk te publiceren. Als de gebruiker klaar is met het toevoegen van inhoud in de map **NEW** , kan hij of zij de map met de bijdrage weer publiceren naar de AEM auteuromgeving. Het kan enkele minuten duren voordat de import is voltooid en de nieuw gepubliceerde inhoud in AEM Assets wordt weerspiegeld.

Bovendien blijft alle bestaande functionaliteit ongewijzigd. Gebruikers van het Brand Portal kunnen middelen weergeven, zoeken en downloaden vanuit de bijdragemap en vanuit de andere toegestane mappen. En beheerders kunnen de bijdragemap verder delen, eigenschappen wijzigen en elementen toevoegen aan verzamelingen.

## Vereisten {#prerequisites}

* AEM 6.5.2 of hoger.
* Zorg ervoor dat uw AEM Assets-exemplaar is geconfigureerd met Brand Portal. See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
* Zorg ervoor dat uw Poorthuurder van het Merk met één de auteursinstantie van AEM Assets wordt gevormd.

>[!NOTE]
>
>Asset Sourcing wordt niet ondersteund op AEM Assets als Cloud Service.


>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![Brand Portal Asset Sourting](assets/asset-sourcing.png)


>[!NOTE]
>
>In AEM 6.5.4 is een probleem bekend. Gebruikers van het Brand Portal kunnen de middelen van de map met bijdragen niet naar AEM Assets publiceren bij de upgrade naar de Adobe Developer Console.
>
>De kwestie is vastgelegd in AEM 6.5.5. U kunt uw AEM Assets-exemplaar upgraden naar het nieuwste servicepack AEM 6.5.5 en uw configuraties [](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) upgraden op de Adobe Developer Console.
>
>Voor directe correctie op AEM 6.5.4 wordt aangeraden de hotfix [te](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) downloaden en op de auteurinstantie te installeren.


## Zie ook {#reference-articles}

**Voor beheerders**

* [Middelen in AEM configureren](brand-portal-configure-asset-sourcing.md)
* [Lijst met gebruikers van Brand Portal uploaden](brand-portal-configure-asset-sourcing.md)
* [Contribute-map configureren](brand-portal-contribution-folder.md)
* [Basislijnelementen uploaden naar de bijdragemap](brand-portal-upload-baseline-assets.md)
* [Map met bijdragen publiceren naar Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

**Voor gebruikers van Brand Portal**

* [Elementvereisten downloaden](brand-portal-download-asset-requirements.md)
* [Nieuwe elementen uploaden naar de bijdragemap](brand-portal-upload-assets-to-contribution-folder.md)
* [Bijdragemap publiceren naar AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
