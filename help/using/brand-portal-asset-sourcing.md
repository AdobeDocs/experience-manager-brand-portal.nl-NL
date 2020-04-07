---
title: Asset Sourting in Brand Portal
seo-title: Asset Sourting in Brand Portal
description: Meer informatie over de functie voor het aanschaffen van bedrijfsmiddelen die beschikbaar is in de Adobe Experience Manager Assets Brand Portal.
seo-description: Meer informatie over de functie voor het aanschaffen van bedrijfsmiddelen die beschikbaar is in de Adobe Experience Manager Assets Brand Portal.
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
source-git-commit: ca71b51ea51a92f23fc4c7d6682f73c4c204a5f2

---


# Overzicht van Asset Souring {#overview-asset-sourcing-in-bp}

**Met Asset Sourcing** kunnen AEM-gebruikers (beheerders/gebruikers die geen beheerder zijn) nieuwe mappen maken met een extra eigenschap voor **Asset Contribution** , zodat de nieuwe map die is gemaakt, kan worden verzonden door gebruikers van Brand Portal. Dit leidt automatisch tot een werkschema dat tot twee extra subomslagen, genoemd **GEDEELD** en **NIEUW**, binnen de pas gecreëerde omslag van de **Bijdrage** leidt. De beheerder van AEM bepaalt dan het vereiste door een kort over de types van activa te uploaden die aan de bijdrageomslag, evenals een reeks basiselementen, aan de **GEDEELDE** omslag moeten worden toegevoegd om BP gebruikers te verzekeren hebben de verwijzingsinformatie zij nodig hebben. De beheerder kan actieve gebruikers van het Brand Portal dan toegang tot de bijdrageomslag verlenen alvorens de pas gecreëerde omslag van de **Bijdrage** aan het Portaal van het Merk te publiceren. Als de gebruiker klaar is met het toevoegen van inhoud in de map **NEW** , kan hij of zij de map met bijdragen weer publiceren naar de AEM-auteuromgeving. Het kan enkele minuten duren voordat de import is voltooid en de nieuw gepubliceerde inhoud in AEM Assets wordt weerspiegeld.

Bovendien blijft alle bestaande functionaliteit ongewijzigd. Gebruikers van het Brand Portal kunnen middelen weergeven, zoeken en downloaden vanuit de bijdragemap en vanuit de andere toegestane mappen. En beheerders kunnen de bijdragemap verder delen, eigenschappen wijzigen en elementen toevoegen aan verzamelingen.

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

>[!NOTE]
>
>Asset Sourcing in Brand Portal wordt ondersteund op AEM 6.5.2.0 en hoger.
>
>De functie wordt niet ondersteund in eerdere versies - AEM 6.3 en AEM 6.4.
>
>Neem contact op met de ondersteuning van Adobe om uw AEM-exemplaar bij te werken naar de meest recente ondersteunde AEM-versie.

![Brand Portal Asset Sourting](assets/asset-sourcing.png)


>[!NOTE]
>
>Als u een gebruiker van AEM 6.5.4 bent, zal de eigenschap van de Verkoop van Activa blijven werken aan de &quot;erfenis integratie OAuth&quot;.
>
>Gebruikers van Brand Portal kunnen echter geen middelen uit de bijdragemap naar AEM Assets publiceren bij de upgrade naar Adobe I/O op AEM 6.5.4.
>
>Dit probleem wordt opgelost in het volgende servicepack AEM 6.5.5.
>
>Voor directe correctie op AEM 6.5.4 wordt aangeraden de hotfix [te](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) downloaden en op de auteurinstantie te installeren.


## Vereisten {#prerequisites}

* AEM 6.5.0.2 of hoger.
* Zorg ervoor dat uw AEM Assets-instantie is geconfigureerd met Brand Portal. Zie AEM-middelen [configureren met Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

## Zie ook {#reference-articles}

**Voor beheerders**

* [Asset Souring configureren in AEM](brand-portal-configure-asset-sourcing.md)
* [Lijst met gebruikers van Brand Portal uploaden](brand-portal-configure-asset-sourcing.md)
* [Contribute-map configureren](brand-portal-contribution-folder.md)
* [Basislijnelementen uploaden naar de bijdragemap](brand-portal-upload-baseline-assets.md)
* [Map met bijdragen publiceren naar Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

**Voor gebruikers van Brand Portal**

* [Elementvereisten downloaden](brand-portal-download-asset-requirements.md)
* [Nieuwe elementen uploaden naar de bijdragemap](brand-portal-upload-assets-to-contribution-folder.md)
* [Map met bijdragen publiceren naar AEM-elementen](brand-portal-publish-contribution-folder-to-aem-assets.md)
