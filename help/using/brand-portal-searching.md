---
title: Middelen zoeken op Brand Portal
seo-title: Asset searching and saved search on Experience Manager Assets Brand Portal
description: Met de zoekfunctie van Brand Portal kunt u snel naar relevante middelen zoeken met alzoekopdrachten en met zoekfilters kunt u uw zoekopdracht verder beperken. Sla uw zoekopdrachten op als slimme verzamelingen voor de toekomst.
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: 100b0945c04a21a7bf6810c9ae0fee750809ebdb
workflow-type: tm+mt
source-wordcount: '1162'
ht-degree: 4%

---

# Middelen zoeken op Brand Portal {#search-assets-on-brand-portal}

Met de zoekfunctie van Brand Portal kunt u snel relevante middelen zoeken aan de hand van alzoekopdrachten en zoeken naar facetten die filters gebruiken om uw zoekopdracht verder te beperken. U kunt middelen op dossiers of omslagniveau zoeken en uw onderzoeksresultaten opslaan als slimme inzamelingen.

>[!NOTE]
>
>Brand Portal biedt geen ondersteuning voor het zoeken naar verzamelingen met alzoekopdrachten.
>
>U kunt echter [zoekfilters om de lijst met relevante verzamelingen op te halen](#search-collection).

## Middelen zoeken met Omgaan {#search-assets-using-omnisearch}

Op Brand Portal zoeken naar elementen:

1. Klik in de werkbalk op de knop **[!UICONTROL Search]** of druk op &quot;**[!UICONTROL /]**&quot;.

   ![](assets/omnisearchicon-1.png)

1. Typ in het zoekvak een trefwoord voor de elementen die u wilt zoeken.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Er zijn minimaal 3 tekens nodig om zoeksuggesties te kunnen weergeven.

1. Maak een keuze uit de verwante suggesties die in de vervolgkeuzelijst worden weergegeven, zodat u snel toegang hebt tot relevante elementen.

   ![](assets/assets-search-result.png)

   *Zoeken van middelen met alzoekfunctie*

Zie voor meer informatie over het zoekgedrag met slimme gecodeerde elementen [zoekresultaten en gedrag begrijpen](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html).

## Zoeken met facetten in het deelvenster Filters {#search-using-facets-in-filters-panel}

Met zoekfacetten in het deelvenster Filters kunt u de zoekervaring korter maken en de zoekfunctionaliteit efficiënt maken. De facetten van het onderzoek gebruiken veelvoudige dimensies (predikaten) die u toelaten om complexe onderzoeken uit te voeren. U kunt gemakkelijk tot het gewenste niveau van detail voor een gerichter onderzoek boor.

Als u bijvoorbeeld een afbeelding zoekt, kunt u kiezen of u een bitmap- of een vectorafbeelding wilt. U kunt het zoekbereik verder beperken door het MIME-type voor de afbeelding op te geven in de zoekfacet Bestandstype. Op dezelfde manier kunt u bij het zoeken naar documenten de indeling opgeven, bijvoorbeeld de indeling PDF of MS Word.

![Deelvenster Filters in Brand Portal](assets/file-type-search.png "Deelvenster Filters in Brand Portal")

De **[!UICONTROL Filters]** bevat enkele standaardfacetten, zoals **[!UICONTROL Path Browser]**, **[!UICONTROL File Type]**, **[!UICONTROL File Size]**, **[!UICONTROL Status]**, en **[!UICONTROL Orientation]**. U kunt echter [aangepaste zoekfacetten toevoegen](../using/brand-portal-search-facets.md) of specifieke zoekfacetten verwijderen uit de **[!UICONTROL Filters]** door voorspelden toe te voegen aan of te verwijderen uit het onderliggende zoekformulier. Zie de lijst met beschikbare en bruikbare [zoekresultaten op Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

Filters toepassen op uw zoekopdracht met de beschikbare [zoekfacetten](../using/brand-portal-search-facets.md):

1. Klik op het bedekkingspictogram en selecteer **[!UICONTROL Filter]**.

   ![](assets/selectorrail.png)

1. Van de **[!UICONTROL Filters]** Selecteer de gewenste opties om de relevante filters toe te passen.
Gebruik bijvoorbeeld de volgende standaardfilters:

   * **[!UICONTROL Path Browser]** om elementen in een specifieke map te zoeken. Het standaardzoekpad van de voorspelling voor de padbrowser is `/content/dam/mac/<tenant-id>/`, die kan worden geconfigureerd door het standaardzoekformulier te bewerken.
   >[!NOTE]
   >
   >Voor gebruikers die geen beheerder zijn, [!UICONTROL Path Browser] in [!UICONTROL Filter] toont alleen de inhoudsstructuur van de mappen (en hun bovenliggende mappen) die met hen worden gedeeld.\
   >Als u gebruikers wilt beheren, kunt u in de padbrowser naar een willekeurige map in Brand Portal navigeren.

   * **[!UICONTROL File Type]** om het type elementbestand op te geven (afbeelding, document, multimedia, archief) dat u zoekt. Verder kunt u het bereik van uw zoekopdracht beperken door bijvoorbeeld het MIME-type (TIFF, Bitmap, GIMP-afbeeldingen) voor de afbeelding of de indeling (PDF of MS Word) voor de documenten op te geven.
   * **[!UICONTROL File Size]** om te zoeken naar elementen op basis van hun grootte. U kunt de onder- en bovengrenzen voor het groottebereik opgeven om de zoekopdracht te beperken en de maateenheid voor de zoekactie opgeven.
   * **[!UICONTROL Status]** om te zoeken naar elementen die zijn gebaseerd op de status van elementen, zoals Goedgekeurd, Wijzigingen aangevraagd, Geweigerd, In behandeling) en Verlopen.
   * **[!UICONTROL Average Rating]** het zoeken naar activa op basis van de rating van de activa.
   * **[!UICONTROL Orientation]** om te zoeken naar elementen op basis van de richting (horizontaal, verticaal, vierkant) van de elementen.
   * **[!UICONTROL Style]** om te zoeken naar elementen op basis van de stijl (gekleurd, monochroom) van de elementen.
   * **[!UICONTROL Video Format]** naar video-elementen zoeken op basis van hun indeling (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).

   U kunt [aangepaste zoekfacetten](../using/brand-portal-search-facets.md) in het deelvenster Filters door het onderliggende zoekformulier te bewerken.

   * **[!UICONTROL Property Predicate]** als u deze functie gebruikt in het zoekformulier, kunt u zoeken naar elementen die overeenkomen met een eigenschap metadata waaraan de voorspelling wordt toegewezen.\
      Als u bijvoorbeeld Eigenschapvoorspelling wilt toewijzen aan [!UICONTROL `jcr:content /metadata/dc:title`], kunt u elementen zoeken op basis van hun titel.\
      De [!UICONTROL Property Predicate] ondersteunt zoekopdrachten naar tekst:

      **Gedeeltelijke zinnen**
Als u het zoeken van elementen wilt toestaan met gebruik van gedeeltelijke woordgroepen in voorspelling van eigenschappen, schakelt u de optie **[!UICONTROL Partial Search]** Schakel het selectievakje Formulier zoeken in.\
      Op deze manier kunt u naar de gewenste assets zoeken, zelfs als u niet de exacte woorden/woordgroepen opgeeft die in de metadata van de assets worden gebruikt.\
      U kunt:
      * Geef een woord op dat in de gezochte woordgroep voorkomt in het facet in het deelvenster Filters. Als u bijvoorbeeld zoekt naar de term **klimmen** (en Eigenschappenvoorspelling wordt toegewezen aan [!UICONTROL `dc:title`] eigenschap), dan alle elementen met het woord **klimmen** in hun titel worden de woorden teruggegeven.
      * Een deel van het woord opgeven dat in de gezochte woordgroep voorkomt, samen met een jokerteken (*) om de tussenruimten te vullen.
Bijvoorbeeld bij het zoeken naar:
         * **klimmen*** retourneert alle elementen met woorden die beginnen met de tekens &quot;klimmen&quot; in de titelzin.
         * ***klimmen** retourneert alle elementen met woorden die eindigen met tekens &quot;klimmen&quot; in de titelzin.
         * ***klimmen*** retourneert alle elementen met woorden die de tekens &quot;klimmen&quot; in hun titelzin bevatten.

Als u niet-hoofdlettergevoelig zoeken in voorspelling van eigenschappen wilt toestaan, schakelt u het       **Niet-hoofdlettergevoelige tekst**
Als u niet-hoofdlettergevoelig zoeken in voorspelling van eigenschappen wilt toestaan, schakelt u het **[!UICONTROL Ignore Case]** Schakel het selectievakje Formulier zoeken in. Standaard is bij het zoeken naar eigenschappen hoofdlettergevoelig.
   >[!NOTE]
   >
   >Bij selecteren **[!UICONTROL Partial Search]** selectievakje, **[!UICONTROL Ignore Case]** is standaard geselecteerd.

   ![](assets/wildcard-prop-1.png)

   De zoekresultaten worden weergegeven op basis van de toegepaste filters en het aantal zoekresultaten.

   ![](assets/omnisearch-with-filters.png)

   Resultaat van middelenzoekopdracht met aantal zoekresultaten.

1. U kunt gemakkelijk naar een punt van het onderzoeksresultaat navigeren, en aan het zelfde onderzoeksresultaat terugkeren gebruikend de achterknoop in uw browser zonder het moeten de onderzoeksvraag opnieuw in werking stellen.

## Uw zoekopdrachten opslaan als slimme verzameling {#save-your-searches-as-smart-collection}

U kunt de zoekinstellingen opslaan als een slimme verzameling zodat u dezelfde zoekopdracht snel kunt herhalen zonder dat u later dezelfde instellingen opnieuw hoeft uit te voeren. U kunt echter geen zoekfilters toepassen in een verzameling.

De zoekinstellingen opslaan als een slimme verzameling:

1. Tikken/ klikken **[!UICONTROL Save Smart Collection]** en geef een naam op voor de slimme verzameling.

   Selecteer **[!UICONTROL Public]**. Een bericht bevestigt dat de slimme verzameling is gemaakt en toegevoegd aan de lijst met opgeslagen zoekopdrachten.

   >[!NOTE]
   >
   >Niet-beheerders kunnen worden beperkt in het openbaar maken van slimme verzamelingen om te voorkomen dat een enorm aantal openbare slimme verzamelingen wordt gemaakt door gebruikers die geen beheerder zijn, op de Brand Portal van de organisatie. Organisaties kunnen de **[!UICONTROL Allow public smart collections creation]** configuratie van **[!UICONTROL General]** instellingen beschikbaar in het deelvenster met beheergereedschappen.

   ![](assets/save_smartcollectionui.png)

1. Als u de slimme verzameling onder een andere naam wilt opslaan, selecteert of wist u de naam **[!UICONTROL Public]** selectievakje, klikken **[!UICONTROL Edit Smart Collection]**.

   ![](assets/edit_smartcollection.png)

1. Op de **[!UICONTROL Edit Smart Collection]** dialoogvenster selecteert u **[!UICONTROL Save As]** en voer een naam in voor de slimme verzameling. Klik op **[!UICONTROL Save]**.

   ![](assets/saveas_smartsearch.png)


## Zoekverzameling {#search-collection}

Omnissearch wordt niet ondersteund voor verzamelingen. U kunt echter wel zoekfilters toepassen om de relevante verzamelingen weer te geven vanuit de [!UICONTROL Collections] interface.

Van de [!UICONTROL Collections] klikt u op het bedekkingspictogram om het filterdeelvenster in de linkerspoorstaaf te openen. Enkele of meerdere zoekfilters toepassen op basis van de beschikbare filters (`modified date`, `access type`, en `tags`). De meest relevante verzameling verzamelingen wordt weergegeven op basis van de toegepaste filters.

![](assets/collection-search.png)
