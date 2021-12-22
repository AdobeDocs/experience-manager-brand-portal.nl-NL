---
title: Elementen uploaden en de map Contribution van Brand Portal naar Experience Manager Assets publiceren
seo-title: Upload assets and publish the Contribution folder from Brand Portal to Experience Manager Assets
description: Bekijk meer inzicht in het uploaden van nieuwe middelen en het publiceren van de map met bijdragen van Brand Portal naar Experience Manager Assets.
seo-description: Get an insight into uploading new assets and publishing the contribution folder from Brand Portal to Experience Manager Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 7dcf445d-97ed-4fa5-959c-c4c48e325766
source-git-commit: 3845d9fa17e75d59493383303ca0978349ca0401
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 0%

---

# Bijdragemap publiceren naar Experience Manager Assets {#using-asset-souring-in-bp}

Brand Portal-gebruikers met de juiste machtigingen kunnen meerdere elementen of mappen met meerdere elementen uploaden naar de map met bijdragen. Brand Portal-gebruikers kunnen echter alleen elementen uploaden naar **NIEUW** map. De **GEDEELD** Deze map is bedoeld voor de distributie van basislijnelementen (referentie-inhoud) die door Brand Portal-gebruikers kunnen worden gebruikt bij het maken van nieuwe elementen voor een bijdrage.

Brand Portal-gebruikers die toegang hebben tot de map Contribution, kunnen de volgende activiteiten uitvoeren:

* [Elementvereisten downloaden](#download-asset-requirements)
* [Nieuwe elementen uploaden naar de map voor bijdragen](#uplad-new-assets-to-contribution-folder)
* [Bijdragemap publiceren naar Experience Manager Assets](#publish-contribution-folder-to-aem)

## Elementvereisten downloaden {#download-asset-requirements}

Brand Portal-gebruikers ontvangen automatisch e-mail-/pulsmeldingen wanneer een bijdragemap wordt gedeeld door de Experience Manager Assets-gebruiker, zodat deze het korte document (met elementvereisten) kunnen downloaden en de basiselementen (referentie-inhoud) kunnen downloaden van de **GEDEELD** om te controleren of ze de vereisten voor middelen begrijpen.

Brand Portal-gebruikers voeren de volgende activiteiten uit om de vereisten voor middelen te downloaden:

* **Download overzicht**: Download de samenvatting (document met middelenvereisten) die is toegevoegd aan de bijdragemap en die informatie bevat over elementen zoals het type middelen, het doel, de ondersteunde indelingen, de maximale grootte van de middelen, enz.
* **Basiselementen downloaden**: Download de basislijnelementen die kunnen worden gebruikt om de vereiste typen elementen te begrijpen. Brand Portal-gebruikers kunnen deze middelen gebruiken als referentie om nieuwe middelen te maken voor hun bijdrage.

Het Brand Portal-dashboard weerspiegelt alle bestaande mappen die aan de Brand Portal-gebruiker zijn toegestaan, samen met de nieuw gedeelde bijdragemap. In dit voorbeeld heeft de Brand Portal-gebruiker alleen toegang tot de zojuist gemaakte map met bijdragen. Er wordt geen andere bestaande map gedeeld met de gebruiker.

**Elementvereisten downloaden:**

1. Meld u aan bij uw Brand Portal-exemplaar.
1. Selecteer de map met bijdragen in het Brand Portal-dashboard.
1. Klik op **[!UICONTROL Properties]**. Het venster van het Bezit dat de details van de bijdrageomslag bevat opent.

   ![](assets/properties.png)

   ![](assets/download-asset-requirement2.png)

1. Klik op de knop **[!UICONTROL Download Brief]** om het document met de elementvereisten op uw lokale computer te downloaden.

   ![](assets/download.png)

1. Ga terug naar het Brand Portal-dashboard.
1. Klik om de map met bijdragen te openen. U ziet twee submappen-**[!UICONTROL SHARED]** en **[!UICONTROL NEW]** in de map met Help. De map SHARED bevat alle basiselementen (referentie-inhoud) die door de beheerders worden gedeeld.
1. U kunt de **[!UICONTROL SHARED]** map met alle basislijnelementen op uw lokale computer.
U kunt ook de opdracht **[!UICONTROL SHARED]** en klik op de knop **Downloaden** pictogram om afzonderlijke bestanden/mappen te downloaden.

   ![](assets/download.png)

   ![](assets/download-asset-requirement5.png)

Doorloop de samenvatting (document met vereisten voor elementen) en verwijs naar de basiselementen om inzicht te krijgen in de vereisten voor elementen. Nu kunt u nieuwe middelen maken voor de bijdrage en deze uploaden naar de map met bijdragen.


## Elementen uploaden naar de bijdragemap {#uplad-new-assets-to-contribution-folder}

Nadat de gebruikers van Brand Portal de elementvereisten hebben doorlopen, kunnen ze nieuwe middelen maken voor hun bijdrage en deze uploaden naar de map NEW in de bijdragemap.

>[!NOTE]
>
>De Brand Portal-gebruikers kunnen alleen elementen uploaden naar de map NEW.
>
>De maximale uploadlimiet voor Brand Portal-gebruikers is **10** GB dat cumulatief wordt toegepast op alle bijdragemappen.
>
>De naar Brand Portal geüploade elementen worden niet verwerkt voor uitvoeringen en bevatten geen voorvertoningen.

>[!NOTE]
>
>U wordt aangeraden de uploadruimte vrij te geven nadat u de map met bijdragen naar Experience Manager Assets hebt gepubliceerd, zodat deze beschikbaar is voor de andere Brand Portal-gebruikers voor een bijdrage.
>
>Als het nodig is om de uploadlimiet van je Brand Portal-huurder te overschrijden **10** GB, neem contact op met de Klantenondersteuning om de vereiste op te geven.


**Nieuwe elementen uploaden:**

1. Meld u aan bij uw Brand Portal-exemplaar.
Het Brand Portal-dashboard weerspiegelt alle bestaande mappen die aan de Brand Portal-gebruiker zijn toegestaan, samen met de nieuw gedeelde bijdragemap.

1. Selecteer de map met de bijdrage en klik om deze te openen. De map met de bijdrage bevat twee submappen - **[!UICONTROL SHARED]** en **[!UICONTROL NEW]**.

1. Klik op de knop **[!UICONTROL NEW]** map.

   ![](assets/upload-new-assets4.png)

1. Klikken **[!UICONTROL Create]** > **[!UICONTROL Files]** om afzonderlijke bestanden of mappen (.zip) met meerdere elementen te uploaden.

   ![](assets/upload-new-assets5.png)

1. Blader naar elementen (bestanden of mappen) en upload deze naar de **[!UICONTROL NEW]** map.

   ![](assets/upload-asset4.png)

Nadat u alle elementen of mappen naar de map NEW hebt geüpload, publiceert u de map met bijdragen naar Experience Manager Assets.


## Bijdragemap publiceren naar Experience Manager Assets {#publish-contribution-folder-to-aem}

Brand Portal-gebruikers kunnen de map met bijdragen publiceren naar Experience Manager Assets zonder dat ze toegang hoeven te hebben tot het exemplaar van de auteur van de Experience Manager.

Zorg ervoor dat u de elementvereisten hebt doorlopen en upload de nieuwe elementen in **NIEUW** map in de map met Help.

**Map met bijdragen publiceren:**

1. Meld u aan bij uw Brand Portal-exemplaar.

1. Selecteer de map met bijdragen in het Brand Portal-dashboard.
1. Klik op **[!UICONTROL Publish to AEM]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem1.png)

Er wordt een e-mail-/pulsmelding verzonden naar de Brand Portal-gebruiker en -beheerders in verschillende stadia van de publicatieworkflow:

1. **In wachtrij** - Er wordt een melding verzonden naar de Brand Portal-gebruiker en Brand Portal-beheerders wanneer een publicatieworkflow in Brand Portal wordt geactiveerd.

1. **Voltooid** - Er wordt een melding verzonden naar de Brand Portal-gebruiker en Brand Portal-beheerders wanneer de bijdragemap correct is gepubliceerd naar Experience Manager Assets.

Na publicatie van de zojuist gemaakte middelen naar Experience Manager Assets kunnen de Brand Portal-gebruikers deze verwijderen uit de map NEW. De Brand Portal-beheerder kan de elementen echter verwijderen uit zowel de map NEW als de map SHARED.

Zodra het doel van het creëren van de bijdrageomslag wordt bereikt, kan de beheerder van Brand Portal de bijdrageomslag schrappen om uploadruimte voor andere gebruikers vrij te geven.

## Status van taak publiceren {#publishing-job-status}

Er zijn twee rapporten die de beheerders kunnen gebruiken om de status van de omslagen van de activabijdrage te bekijken die van Brand Portal aan Experience Manager Assets worden gepubliceerd.

* Navigeer in Brand Portal naar **[!UICONTROL Tools]** > **[!UICONTROL Asset Contribution Status]**. Dit rapport geeft de status van alle publicatietaken in verschillende stadia van de publicatieworkflow weer.

   ![](assets/contribution-folder-status.png)

* Navigeer in Experience Manager Assets (op locatie of beheerde service) naar **[!UICONTROL Assets]** > **[!UICONTROL Jobs]**. Dit rapport geeft de uiteindelijke status (Voltooid of Fout) weer van alle publicatietaken.

   ![](assets/publishing-status.png)

* Ga in Experience Manager Assets as a Cloud Service naar **[!UICONTROL Assets]** > **[!UICONTROL Jobs]**.

   U kunt ook rechtstreeks navigeren naar **[!UICONTROL Jobs]** van de globale navigatie.

   Dit rapport geeft de uiteindelijke status (Succesvol of Fout) weer van alle publicatietaken, inclusief de import van activa van Brand Portal naar Experience Manager Assets as a Cloud Service.

   ![](assets/cloud-service-job-status.png)

<!--
>[!NOTE]
>
>Currently, no report is generated in AEM Assets as a Cloud Service for the Asset Sourcing workflow. 
-->
