---
title: Voorinstellingen voor afbeeldingen of dynamische uitvoeringen toepassen
seo-title: Apply image presets or dynamic renditions
description: Net als bij een macro is een voorinstelling voor afbeeldingen een vooraf gedefinieerde verzameling opdrachten voor grootte en opmaak die onder een naam zijn opgeslagen. Met voorinstellingen voor afbeeldingen kan Experience Manager Assets Brand Portal dynamisch afbeeldingen van verschillende grootten, indelingen en eigenschappen leveren.
seo-description: Like a macro, an image preset is a predefined collection of sizing and formatting commands saved under a name. Image presets enable Experience Manager Assets Brand Portal to dynamically deliver images of different sizes, formats, and properties.
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415bac
role: Admin
exl-id: 212a1b3a-686f-4250-be06-b679b6039887
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 2%

---

# Voorinstellingen voor afbeeldingen of dynamische uitvoeringen toepassen {#apply-image-presets-or-dynamic-renditions}

Net als bij een macro is een voorinstelling voor afbeeldingen een vooraf gedefinieerde verzameling opdrachten voor grootte en opmaak die onder een naam zijn opgeslagen. Met voorinstellingen voor afbeeldingen kan Experience Manager Assets Brand Portal dynamisch afbeeldingen van verschillende grootten, indelingen en eigenschappen leveren.

Een voorinstelling voor afbeeldingen wordt gebruikt om dynamische uitvoeringen te genereren van afbeeldingen die u kunt voorvertonen en downloaden. Wanneer u een voorvertoning weergeeft van afbeeldingen en de bijbehorende uitvoeringen, kunt u een voorinstelling kiezen om de afbeeldingen opnieuw op te maken volgens de specificaties die zijn ingesteld door uw beheerder.

(*Als de Experience Manager Assets-instantie van de auteur wordt uitgevoerd **Dynamic Media Hybride, modus***) Als u dynamische uitvoeringen van een element wilt weergeven in Brand Portal, moet u ervoor zorgen dat de betreffende Pyramid tiff-uitvoering bestaat in de Experience Manager Assets-auteur-instantie van de plaats waar u publiceert naar Brand Portal. Wanneer u het element publiceert, wordt de PTIFF-uitvoering ook gepubliceerd naar Brand Portal.

>[!NOTE]
>
>Wanneer u afbeeldingen en de bijbehorende uitvoeringen downloadt, is er geen optie om te kiezen uit de bestaande voorinstellingen. In plaats daarvan kunt u de eigenschappen van een aangepaste voorinstelling voor afbeeldingen opgeven. Zie voor meer informatie [Afbeeldingsvoorinstellingen toepassen bij het downloaden van afbeeldingen](../using/brand-portal-image-presets.md#main-pars-text-1403412644).


Zie voor meer informatie over de parameters die zijn vereist voor het maken van voorinstellingen voor afbeeldingen [Voorinstellingen afbeelding beheren](../using/brand-portal-image-presets.md).

## Een voorinstelling voor afbeeldingen maken {#create-an-image-preset}

De Experience Manager Assets-beheerders kunnen voorinstellingen voor afbeeldingen maken die als dynamische uitvoeringen op de pagina met middelendetails worden weergegeven. U kunt een geheel nieuwe voorinstelling voor afbeeldingen maken of een bestaande voorinstelling met een nieuwe naam opslaan. Wanneer u een voorinstelling voor afbeeldingen maakt, kiest u een grootte voor de levering van de afbeelding en de opmaakopdrachten. Wanneer een afbeelding voor weergave wordt geleverd, wordt de weergave ervan geoptimaliseerd volgens de gekozen opdrachten.

>[!NOTE]
>
>Dynamische uitvoeringen van een afbeelding worden gemaakt met de Piramide-TIFF. Als de Pyramid-TIFF niet beschikbaar is voor een element, kunnen dynamische uitvoeringen voor dat element niet worden opgehaald in het Brand-portaal.
>
>Als de Experience Manager Assets-instantie van de auteur wordt uitgevoerd **Dynamic Media Hybride, modus** En dan worden Pyramid-TIFF-uitvoeringen van afbeeldingselementen gemaakt en opgeslagen in de Experience Manager Assets-opslagplaats.
>
>Als de Experience Manager Assets-instantie van de auteur wordt uitgevoerd **Dynamic Media Scene 7, modus** Dan bestaan er Pyramid-TIFF-uitvoeringen van afbeeldingselementen op Scene 7-server.
>
>Wanneer dergelijke middelen op brandportal worden gepubliceerd, worden voorinstellingen voor afbeeldingen toegepast en dynamische uitvoeringen weergegeven.


1. Klik in de werkbalk boven in het scherm op het logo van de Experience Manager voor toegang tot de beheergereedschappen.

1. Klik in het deelvenster met beheergereedschappen op **[!UICONTROL Image Presets]**.

   ![](assets/admin-tools-panel-4.png)

1. Klik op de pagina met voorinstellingen voor afbeeldingen op **[!UICONTROL Create]**.

   ![](assets/image_preset_homepage.png)

1. In de **[!UICONTROL Edit Image Preset]** pagina, geeft u waarden op in de **[!UICONTROL Basic]** en **[!UICONTROL Advanced]** de juiste tabbladen, inclusief een naam. Voorinstellingen worden weergegeven in het linkerdeelvenster en kunnen direct samen met andere assets worden gebruikt.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >U kunt ook de opdracht **[!UICONTROL Edit Image Preset]** pagina om de eigenschappen van een bestaande voorinstelling voor afbeeldingen te bewerken. Als u een afbeeldingsvoorinstelling wilt bewerken, selecteert u deze op de pagina met voorinstellingen voor afbeeldingen en klikt u op **[!UICONTROL Edit]**.

1. Klik op **[!UICONTROL Save]**. De voorinstelling voor de afbeelding wordt gemaakt en weergegeven op de pagina met voorinstellingen voor de afbeelding.
1. Als u een afbeeldingsvoorinstelling wilt verwijderen, selecteert u deze op de pagina met voorinstellingen voor afbeeldingen en klikt u op **[!UICONTROL Delete]**. Klik op de bevestigingspagina op **[!UICONTROL Delete]** om de schrapping te bevestigen. De voorinstelling voor de afbeelding wordt verwijderd van de pagina met voorinstellingen voor de afbeelding.

## Afbeeldingsvoorinstellingen toepassen bij voorvertoningen van afbeeldingen  {#apply-image-presets-when-previewing-images}

Als u een voorvertoning weergeeft van afbeeldingen en de bijbehorende uitvoeringen, kiest u een van de bestaande voorinstellingen om de afbeeldingen opnieuw op te maken volgens de specificaties die zijn ingesteld door uw beheerder.

1. Klik in de Brand Portal-interface op een afbeelding om deze te openen.
1. Klik op het bedekkingspictogram aan de linkerkant en kies **[!UICONTROL Renditions]**.

   ![](assets/image-preset-previewrenditions.png)

1. Van de **[!UICONTROL Renditions]** selecteert u bijvoorbeeld de juiste dynamische vertoning, **[!UICONTROL Thumbnail]**. De voorvertoningsafbeelding wordt weergegeven op basis van uw keuze voor de vertoning.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Afbeeldingsvoorinstellingen toepassen bij het downloaden van afbeeldingen {#apply-image-presets-when-downloading-images}

Wanneer u afbeeldingen en de bijbehorende uitvoeringen downloadt uit Brand Portal, kunt u geen voorinstellingen voor bestaande afbeeldingen kiezen. U kunt de eigenschappen van voorinstellingen voor afbeeldingen echter aanpassen op basis waarvan u de afbeeldingen opnieuw wilt opmaken.

1. Voer een van de volgende handelingen uit vanuit de Brand Portal-interface:

   * Houd de aanwijzer boven de afbeelding die u wilt downloaden. Klik op de sneltoetsminiaturen die beschikbaar zijn op de knop **[!UICONTROL Download]** pictogram.

   ![](assets/downloadsingleasset.png)

   * Selecteer de afbeelding die u wilt downloaden. Klik in de werkbalk bovenaan op de knop **[!UICONTROL Download]** pictogram.

   ![](assets/downloadassets.png)

1. Van de **[!UICONTROL Download]** selecteert u de vereiste opties, afhankelijk van het feit of u het element met of zonder de uitvoeringen wilt downloaden.

   ![](assets/donload-assets-dialog.png)

1. Als u dynamische uitvoeringen van het element wilt downloaden, selecteert u de optie **[!UICONTROL Dynamic Rendition(s)]** optie.
1. Pas vooraf ingestelde eigenschappen van een afbeelding aan op basis waarvan u de afbeelding en de vertoningen tijdens het downloaden dynamisch opnieuw wilt opmaken. Geef de grootte, indeling, kleurruimte, resolutie en afbeeldingswijziging op.

   ![](assets/dynamicrenditions.png)

1. Klik op **[!UICONTROL Download]**. De aangepaste dynamische uitvoeringen worden gedownload in een ZIP-bestand, samen met de afbeelding en vertoningen die u hebt gedownload. Er wordt echter geen ZIP-bestand gemaakt als één element wordt gedownload, waardoor het snel kan worden gedownload.
