---
title: Voorinstellingen voor afbeeldingen of dynamische uitvoeringen toepassen
seo-title: Voorinstellingen voor afbeeldingen of dynamische uitvoeringen toepassen
description: 'Net als bij een macro is een voorinstelling voor afbeeldingen een vooraf gedefinieerde verzameling opdrachten voor grootte en opmaak die onder een naam zijn opgeslagen. Met voorinstellingen voor afbeeldingen kunnen AEM Assets Brand Portal dynamisch afbeeldingen van verschillende grootten, indelingen en eigenschappen leveren. '
seo-description: 'Net als bij een macro is een voorinstelling voor afbeeldingen een vooraf gedefinieerde verzameling opdrachten voor grootte en opmaak die onder een naam zijn opgeslagen. Met voorinstellingen voor afbeeldingen kunnen AEM Assets Brand Portal dynamisch afbeeldingen van verschillende grootten, indelingen en eigenschappen leveren. '
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
translation-type: tm+mt
source-git-commit: 8fb85750f30ea1fee93cd770b94412bed7698c17
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 1%

---


# Voorinstellingen voor afbeeldingen of dynamische uitvoeringen toepassen {#apply-image-presets-or-dynamic-renditions}

Net als bij een macro is een voorinstelling voor afbeeldingen een vooraf gedefinieerde verzameling opdrachten voor grootte en opmaak die onder een naam zijn opgeslagen. Met voorinstellingen voor afbeeldingen kunnen AEM Assets Brand Portal dynamisch afbeeldingen van verschillende grootten, indelingen en eigenschappen leveren.

Een voorinstelling voor afbeeldingen wordt gebruikt om dynamische uitvoeringen te genereren van afbeeldingen die u kunt voorvertonen en downloaden. Wanneer u een voorvertoning weergeeft van afbeeldingen en de bijbehorende uitvoeringen, kunt u een voorinstelling kiezen om de afbeeldingen opnieuw op te maken volgens de specificaties die zijn ingesteld door uw beheerder.

(*Als AEM (Auteur)-instantie wordt uitgevoerd in de **dynamische modus***Media Hybrid) Als u dynamische uitvoeringen van een element wilt weergeven in Brand Portal, moet u ervoor zorgen dat de Pyramid-versiering bestaat in de AEM auteur-instantie van de locatie waar u publiceert naar Brand Portal. Wanneer u het element publiceert, wordt de PTIFF-uitvoering ook gepubliceerd naar Brand Portal.

>[!NOTE]
>
>Wanneer u afbeeldingen en de bijbehorende uitvoeringen downloadt, is er geen optie om te kiezen uit de bestaande voorinstellingen. In plaats daarvan kunt u de eigenschappen van een aangepaste voorinstelling voor afbeeldingen opgeven. Zie [Afbeeldingsvoorinstellingen toepassen tijdens het downloaden van afbeeldingen](../using/brand-portal-image-presets.md#main-pars-text-1403412644)voor meer informatie.


Zie [Voorinstellingen](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html)afbeelding beheren voor meer informatie over de parameters die nodig zijn voor het maken van voorinstellingen voor afbeeldingen.

## Een voorinstelling voor afbeeldingen maken {#create-an-image-preset}

De AEM beheerders kunnen voorinstellingen voor afbeeldingen maken die als dynamische uitvoeringen op de pagina met elementdetails worden weergegeven. U kunt een geheel nieuwe voorinstelling voor afbeeldingen maken of een bestaande voorinstelling met een nieuwe naam opslaan. Wanneer u een voorinstelling voor afbeeldingen maakt, kiest u een grootte voor de levering van de afbeelding en de opmaakopdrachten. Wanneer een afbeelding voor weergave wordt geleverd, wordt de weergave ervan geoptimaliseerd volgens de gekozen opdrachten.


>[!NOTE]
>
>Dynamische uitvoeringen van een afbeelding worden gemaakt met de Piramide TIFF. Als de Piramid TIFF niet beschikbaar is voor een element, kunnen dynamische uitvoeringen voor dat element niet worden opgehaald in het Brand-portaal.
>
>Als AEM (Auteur)-instantie wordt uitgevoerd in de **Dynamic Media Hybrid-modus**, worden Pyramid TIFF-uitvoeringen van afbeeldingselementen gemaakt en opgeslagen in AEM opslagplaats.
>
>Terwijl AEM (Auteur) instantie op **Dynamische Scène 7 van Media wijze**loopt, dan bestaan de Verlopen van de Piramide TIFF van beeldactiva op de server van Scene 7.
>Wanneer dergelijke middelen op brandportal worden gepubliceerd, worden voorinstellingen voor afbeeldingen toegepast en dynamische uitvoeringen weergegeven.


1. Klik op de AEM werkbalk boven in het scherm op het Adobe-logo voor toegang tot de beheergereedschappen.

1. Klik in het deelvenster met beheergereedschappen op **[!UICONTROL Image Presets]**.

   ![](assets/admin-tools-panel-4.png)

1. Klik op de pagina met voorinstellingen voor afbeeldingen **[!UICONTROL Create]**.

   ![](assets/image_preset_homepage.png)

1. In the **[!UICONTROL Edit Image Preset]** page, enter values into the **[!UICONTROL Basic]** and **[!UICONTROL Advanced]** tabs as appropriate, including a name. The options are outlined in [Image Preset options](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options). Voorinstellingen worden weergegeven in het linkerdeelvenster en kunnen direct samen met andere assets worden gebruikt.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >U kunt de **[!UICONTROL Edit Image Preset]** pagina ook gebruiken om de eigenschappen van een bestaande voorinstelling te bewerken. Als u een voorinstelling voor afbeeldingen wilt bewerken, selecteert u deze op de pagina met voorinstellingen voor afbeeldingen en klikt u **[!UICONTROL Edit]** op deze pagina.

1. Klik op **[!UICONTROL Save]**. De voorinstelling voor de afbeelding wordt gemaakt en weergegeven op de pagina met voorinstellingen voor de afbeelding.
1. Als u een voorinstelling voor afbeeldingen wilt verwijderen, selecteert u deze op de pagina met voorinstellingen voor afbeeldingen en klikt u **[!UICONTROL Delete]** op deze voorinstelling. Klik op de bevestigingspagina **[!UICONTROL Delete]** om de verwijdering te bevestigen. De voorinstelling voor de afbeelding wordt verwijderd van de pagina met voorinstellingen voor de afbeelding.

## Afbeeldingsvoorinstellingen toepassen bij voorvertoningen van afbeeldingen  {#apply-image-presets-when-previewing-images}

Als u een voorvertoning weergeeft van afbeeldingen en de bijbehorende uitvoeringen, kiest u een van de bestaande voorinstellingen om de afbeeldingen opnieuw op te maken volgens de specificaties die zijn ingesteld door uw beheerder.

1. Klik in de interface Brand Portal op een afbeelding om deze te openen.
1. Klik op het bedekkingspictogram aan de linkerkant en kies **[!UICONTROL Renditions]**.

   ![](assets/image-preset-previewrenditions.png)

1. Selecteer in de **[!UICONTROL Renditions]** lijst bijvoorbeeld de juiste dynamische vertoning **[!UICONTROL Thumbnail]**. De voorvertoningsafbeelding wordt weergegeven op basis van uw keuze voor de vertoning.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Afbeeldingsvoorinstellingen toepassen bij het downloaden van afbeeldingen {#apply-image-presets-when-downloading-images}

Wanneer u afbeeldingen en de bijbehorende uitvoeringen downloadt van Brand Portal, kunt u geen voorinstellingen voor bestaande afbeeldingen kiezen. U kunt de eigenschappen van voorinstellingen voor afbeeldingen echter aanpassen op basis waarvan u de afbeeldingen opnieuw wilt opmaken.

1. Voer een van de volgende handelingen uit vanuit de interface Brand Portal:

   * Houd de aanwijzer boven de afbeelding die u wilt downloaden. Klik op het **[!UICONTROL Download]** pictogram van de snelactieminiaturen die beschikbaar zijn.

   ![](assets/downloadsingleasset.png)

   * Selecteer de afbeelding die u wilt downloaden. Klik op het **[!UICONTROL Download]** pictogram op de werkbalk boven in het scherm.

   ![](assets/downloadassets.png)

1. Selecteer in het **[!UICONTROL Download]** dialoogvenster de vereiste opties, afhankelijk van het feit of u het element met of zonder de uitvoeringen wilt downloaden.

   ![](assets/donload-assets-dialog.png)

1. Selecteer de **[!UICONTROL Dynamic Rendition(s)]** optie om dynamische uitvoeringen van het element te downloaden.
1. Pas vooraf ingestelde eigenschappen van een afbeelding aan op basis waarvan u de afbeelding en de vertoningen tijdens het downloaden dynamisch opnieuw wilt opmaken. Geef de grootte, indeling, kleurruimte, resolutie en afbeeldingswijziging op.

   ![](assets/dynamicrenditions.png)

1. Klik op **[!UICONTROL Download]**. De aangepaste dynamische uitvoeringen worden gedownload in een ZIP-bestand, samen met de afbeelding en vertoningen die u hebt gedownload. Er wordt echter geen ZIP-bestand gemaakt als één element wordt gedownload, waardoor het snel kan worden gedownload.
