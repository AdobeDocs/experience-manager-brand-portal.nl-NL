---
title: Elementen uploaden en de map Contribution van Brand Portal naar Experience Manager Assets publiceren
description: Bekijk meer inzicht in het uploaden van nieuwe middelen en het publiceren van de map met bijdragen van Brand Portal naar Experience Manager Assets.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: 7dcf445d-97ed-4fa5-959c-c4c48e325766
source-git-commit: 10f89ded6febb1a024cbe181fa48a290d90223f0
workflow-type: tm+mt
source-wordcount: '1430'
ht-degree: 0%

---

# Publish Contributiemap naar Experience Manager Assets {#using-asset-souring-in-bp}

Brand Portal-gebruikers met de juiste machtigingen kunnen meerdere elementen of mappen met meerdere elementen uploaden naar de map met bijdragen. Nochtans, kunnen de gebruikers van Brand Portal slechts activa aan de **NIEUWE** omslag uploaden. De **GEDEELDE** omslag wordt bedoeld voor de distributie van basislijnactiva (verwijzingsinhoud) die door de gebruikers van Brand Portal terwijl het creëren van nieuwe activa voor bijdrage worden gebruikt.

Brand Portal-gebruikers die toegang hebben tot de map Contribution, kunnen de volgende activiteiten uitvoeren:

* [Elementvereisten downloaden](#download-asset-requirements)
* [Nieuwe elementen uploaden naar de map voor bijdragen](#uplad-new-assets-to-contribution-folder)
* [Publish Contributiemap naar Experience Manager Assets](#publish-contribution-folder-to-aem)

## Elementvereisten downloaden {#download-asset-requirements}

Brand Portal-gebruikers ontvangen automatisch e-mail- en pulsmeldingen wanneer een Experience Manager Assets-gebruiker een bijdragemap deelt. Dit werkschema laat hen het korte (activavereiste) document en basislijnactiva (verwijzingsinhoud) van de **GEDEELDE** omslag downloaden om de activavereisten te begrijpen.

Brand Portal-gebruikers voeren de volgende activiteiten uit om de vereisten voor middelen te downloaden:

* **Download samenvatting** - Download het korte (document van de activavereiste) verbonden aan de bijdrageomslag. Het bevat informatie over elementen, zoals het type elementen, het doel, ondersteunde indelingen, de maximale grootte van de elementen en meer.
* **de basislijnactiva van de Download** - Download de basislijnactiva, die kunnen worden gebruikt om de vereiste types van activa te begrijpen. Brand Portal-gebruikers kunnen deze middelen gebruiken als referentie om nieuwe middelen te maken voor hun bijdrage.

Het Brand Portal-dashboard weerspiegelt alle bestaande mappen die aan de Brand Portal-gebruiker zijn toegestaan, samen met de nieuw gedeelde bijdragemap. In dit voorbeeld heeft de Brand Portal-gebruiker alleen toegang tot de zojuist gemaakte map met bijdragen. Er wordt geen andere bestaande map met de gebruiker gedeeld.

**om activavereisten te downloaden:**

1. Meld u aan bij uw Brand Portal-exemplaar.
1. Selecteer een bijdragemap op het Brand Portal-dashboard.
1. Klik op **[!UICONTROL Properties]**. Het venster van het Bezit dat de details van de bijdrageomslag bevat opent.

   ![](assets/properties.png)

   ![](assets/download-asset-requirement2.png)

1. Klik op de optie **[!UICONTROL Download Brief]** om het document met elementvereisten te downloaden naar uw lokale computer.

   ![](assets/download.png)

1. Ga terug naar het Brand Portal-dashboard.
1. Klik op de map met bijdragen om deze te openen. U ziet twee submappen: **[!UICONTROL SHARED]** en **[!UICONTROL NEW]** in de map met bijdragen. De map SHARED bevat alle basiselementen (referentie-inhoud) die door de beheerders worden gedeeld.
1. U kunt de map **[!UICONTROL SHARED]** met alle basislijnelementen downloaden op uw lokale computer.
Of, kunt u de **[!UICONTROL SHARED]** omslag openen en het **2&rbrace; pictogram van de Download &lbrace;klikken om individuele dossiers/omslagen te downloaden.**

   ![](assets/download.png)

   ![](assets/download-asset-requirement5.png)

Doorloop het korte document (document met vereisten voor elementen) en verwijs naar de basiselementen om inzicht te krijgen in de vereisten voor elementen. Nu kunt u nieuwe middelen maken voor de bijdrage en deze uploaden naar de map met bijdragen.

## Elementen uploaden naar de bijdragemap {#upload-new-assets-to-contribution-folder}

Nadat de gebruikers van Brand Portal de elementvereisten hebben doorlopen, kunnen ze nieuwe middelen maken voor hun bijdrage en deze uploaden naar de map NEW in de bijdragemap. Een gebruiker kan meerdere elementen uploaden naar een map voor middelenbijdragen. Er kan echter maar één map tegelijk worden gemaakt.

>[!NOTE]
>
>De Brand Portal-gebruikers kunnen elementen (maximaal twee gigabyte per bestandsgrootte) uploaden naar de map NEW.
>
>De maximale uploadlimiet voor elke Brand Portal-huurder is tien gigabyte, die cumulatief wordt toegepast op alle mappen voor de bijdrage.
>
>De naar Brand Portal geüploade elementen worden niet verwerkt voor uitvoeringen en bevatten geen voorvertoningen.

>[!NOTE]
>
>Adobe raadt u aan de uploadruimte vrij te geven nadat u de map met bijdragen naar Experience Manager Assets hebt gepubliceerd, zodat deze beschikbaar is voor de andere Brand Portal-gebruikers voor een bijdrage.
>
>Als er een behoefte is om de uploadlimiet van uw Brand Portal huurder voorbij **10** GB uit te breiden, contacteer de Steun van de Klant die het vereiste specificeert.


**om nieuwe activa te uploaden:**

1. Meld u aan bij uw Brand Portal-exemplaar.
Het Brand Portal-dashboard weerspiegelt alle bestaande mappen die aan de Brand Portal-gebruiker zijn toegestaan, samen met de nieuw gedeelde bijdragemap.

1. Selecteer de map met de bijdrage en klik om deze te openen. De map met de bijdrage bevat twee submappen - **[!UICONTROL SHARED]** en **[!UICONTROL NEW]** .

1. Klik op de map **[!UICONTROL NEW]** .

   ![](assets/upload-new-assets4.png)

1. Klik op **[!UICONTROL Create]** > **[!UICONTROL Files]** om afzonderlijke bestanden of mappen (.zip) met meerdere elementen te uploaden.

   ![](assets/upload-new-assets5.png)

1. Blader naar en upload elementen (bestanden of mappen) naar de map **[!UICONTROL NEW]** .

   ![](assets/upload-asset4.png)

Nadat u alle elementen of mappen naar de map NEW hebt geüpload, publiceert u de map met bijdragen naar Experience Manager Assets.


## Publish Contributiemap naar Experience Manager Assets {#publish-contribution-folder-to-aem}

Brand Portal-gebruikers kunnen de map met bijdragen publiceren naar Experience Manager Assets zonder dat ze toegang hoeven te hebben tot het exemplaar van de auteur van de Experience Manager.

Zorg ervoor dat u door de activavereisten bent gegaan en de onlangs gecreeerde activa in de **NIEUWE** omslag binnen de bijdrageomslag uploadt.

**om een bijdrageomslag te publiceren:**

1. Meld u aan bij uw Brand Portal-exemplaar.

1. Selecteer een bijdragemap op het Brand Portal-dashboard.
1. Klik op **[!UICONTROL Publish to AEM]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem1.png)

Er wordt een e-mail-/pulsmelding verzonden naar de Brand Portal-gebruiker en -beheerders in verschillende stadia van de publicatieworkflow:

1. **In een rij opgenomen** - een bericht wordt verzonden naar de gebruiker van Brand Portal en de beheerders van Brand Portal wanneer een het publiceren werkschematrekkers in Brand Portal.

1. **Volledig** - een bericht wordt verzonden naar de gebruiker van Brand Portal en de beheerders van Brand Portal wanneer de bijdrageomslag met succes aan Experience Manager Assets wordt gepubliceerd.

Na publicatie van de zojuist gemaakte middelen naar Experience Manager Assets kunnen de Brand Portal-gebruikers deze verwijderen uit de map NEW. De Brand Portal-beheerder kan de elementen echter verwijderen uit de map NEW en Shared.

Zodra het doel van het creëren van de bijdrageomslag wordt bereikt, kan de beheerder van Brand Portal de bijdrageomslag schrappen om uploadruimte voor andere gebruikers vrij te geven.

## Status van taak publiceren {#publishing-job-status}

Beheerders kunnen twee rapporten gebruiken om de status te bekijken van mappen voor middelenbijdragen die van Brand Portal naar Experience Manager Assets zijn gepubliceerd.

* Navigeer in Brand Portal naar **[!UICONTROL Tools]** > **[!UICONTROL Asset Contribution Status]** . Dit rapport geeft de status van alle publicatietaken in verschillende stadia van de publicatieworkflow weer.

  ![](assets/contribution-folder-status-v2.png)

* Navigeer in Experience Manager Assets (op locatie of beheerde service) naar **[!UICONTROL Assets]** > **[!UICONTROL Jobs]** . Dit rapport geeft de uiteindelijke status (Voltooid of Fout) weer van alle publicatietaken.

  ![](assets/publishing-status.png)

* Navigeer in Experience Manager Assets as a Cloud Service naar **[!UICONTROL Assets]** > **[!UICONTROL Jobs]** .

  U kunt ook rechtstreeks vanuit de globale navigatie naar **[!UICONTROL Jobs]** navigeren.

  Dit rapport geeft de uiteindelijke status (Succesvol of Fout) weer van alle publicatietaken, inclusief de import van activa van Brand Portal naar Experience Manager Assets as a Cloud Service.

  ![](assets/cloud-service-job-status.png)

<!--
>[!NOTE]
>
>Currently, no report is generated in AEM Assets as a Cloud Service for the Asset Sourcing workflow. 
-->

## Automatische verwijdering van naar Experience Manager Assets gepubliceerde middelen uit de map Contribution {#automatically-delete-published-assets-from-contribution-folder}

Brand Portal voert nu om de twaalf uur automatische taken uit om alle bijdragemappen te scannen en alle middelen te verwijderen die naar AEM zijn gepubliceerd. Dientengevolge, te hoeven u niet de activa in de omslag van de Bijdrage manueel te schrappen om de omslaggrootte onder de [&#x200B; drempelgrens &#x200B;](#upload-new-assets-to-contribution-folder) te houden. U kunt ook de status controleren van de verwijdertaken die de afgelopen zeven dagen automatisch zijn uitgevoerd. Het rapport voor een baan verstrekt de volgende details:

* Begintijd taak
* Eindtijd van taak
* Taakstatus
* Totaal aan activa inbegrepen in een baan
* Totaal aantal elementen is verwijderd in een taak
* Totale opslag beschikbaar gesteld als gevolg van de uitvoering van de taak

  ![&#x200B; Rapport van de Schrapping &#x200B;](assets/deletion-reports.png)

U kunt ook verder naar beneden boren om de details van elk middel te bekijken inbegrepen in een schrappingsbaan. De details zoals activa titel, grootte, auteur, schrappingsstatus, en schrappingstijd zijn inbegrepen in het rapport.

![&#x200B; Gedetailleerd Rapport van de Schrapping &#x200B;](assets/deletion-reports-detailed.png)

>[!NOTE]
>
> * Klanten kunnen de Klantenondersteuning van de Adobe vragen om de automatische functionaliteit voor het verwijderen van taken uit te schakelen en weer in te schakelen of de uitvoeringsfrequentie te wijzigen.
> * Deze functie is beschikbaar in Experience Manager 6.5.13.0 en latere versies.

### Verwijderingsrapporten weergeven en downloaden {#view-delete-jobs}

Rapporten voor een verwijdertaak weergeven en downloaden:

1. In Brand Portal, navigeer aan **[!UICONTROL Tools]**> **[!UICONTROL Asset Contribution Status]**> **[!UICONTROL Deletion Reports]** optie.

1. Selecteer een baan en klik **[!UICONTROL View]** om het rapport te bekijken.

   Bekijk de details van elk middel inbegrepen in een schrappingsbaan. De details zoals activa titel, grootte, auteur, schrappingsstatus, en schrappingstijd zijn inbegrepen in het rapport. Klik op **[!UICONTROL Download]** om het rapport voor de taak in CSV-indeling te downloaden.

   De verwijderstatus voor een element in het rapport kan de volgende mogelijke waarden hebben:

   * **schrapte** - het element wordt met succes geschrapt van de omslag van de Bijdrage.

   * **niet Gevonden** - Brand Portal kon niet de activa in de omslag van de Bijdrage vinden. Het element wordt al handmatig uit de map verwijderd.

   * **Overgeslagen** - Brand Portal overgeslagen de activaschrapping aangezien er een nieuwe versie beschikbaar voor het element in de omslag van de Bijdrage is, die nog niet aan Experience Manager wordt gepubliceerd.

   * **Ontbroken** - Brand Portal ontbrak om de activa te schrappen. Er zijn drie pogingen om middelen met een `Failed` verwijderstatus opnieuw te verwijderen. Als het element de derde poging tot verwijderen mislukt, moet u het element handmatig verwijderen.

### Een rapport verwijderen

Met Brand Portal kunt u ook een of meerdere rapporten selecteren en deze handmatig verwijderen.

Een rapport verwijderen:

1. Navigeer aan **[!UICONTROL Tools]**> **[!UICONTROL Asset Contribution Status]**> **[!UICONTROL Deletion Reports]** optie.

1. Selecteer een of meer rapporten en klik op **[!UICONTROL Delete]** .


