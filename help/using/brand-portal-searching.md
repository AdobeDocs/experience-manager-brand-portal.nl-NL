---
title: Middelen zoeken op Brand Portal
seo-title: Zoeken naar middelen en opgeslagen zoekopdracht op AEM-merkportal
description: Met de zoekfunctie van het Brand Portal kunt u snel naar relevante middelen zoeken met behulp van alzoekopdrachten. Met de zoekfilters kunt u uw zoekopdracht verder beperken. Sla uw zoekopdrachten op als slimme verzamelingen voor de toekomst.
seo-description: Met de zoekfunctie van het Brand Portal kunt u snel naar relevante middelen zoeken met behulp van alzoekopdrachten. Met de zoekfilters kunt u uw zoekopdracht verder beperken. Sla uw zoekopdrachten op als slimme verzamelingen voor de toekomst.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Middelen zoeken op Brand Portal {#search-assets-on-brand-portal}

Met de zoekfunctie van het Brand Portal kunt u snel relevante middelen zoeken met behulp van alleszoekopdrachten en zoeken naar facetten die filters gebruiken om uw zoekopdracht verder te beperken. U kunt uw zoekopdrachten ook opslaan als slimme verzamelingen voor de toekomst.

## Middelen zoeken met Omgaan {#search-assets-using-omnisearch}

Op Brand Portal zoeken naar elementen:

1. Klik op het **[!UICONTROL Search]** pictogram op de werkbalk of druk op de toets &quot;**[!UICONTROL /]**&quot; om het venster Onderzoek te starten.

   ![](assets/omnisearchicon-1.png)

1. Typ in het zoekvak een trefwoord voor de elementen die u wilt zoeken.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Er zijn minimaal 3 tekens nodig om zoeksuggesties te kunnen weergeven.

1. Maak een keuze uit de verwante suggesties die in de vervolgkeuzelijst worden weergegeven, zodat u snel toegang hebt tot relevante elementen.

   ![](assets/assets-search-result.png)

   *Zoeken van middelen met alzoekfunctie*

Zie [Zoekresultaten en gedrag](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-assets.html)begrijpen voor informatie over het zoekgedrag met slimme gecodeerde elementen.

## Zoeken met facetten in het deelvenster Filters {#search-using-facets-in-filters-panel}

Met zoekfacetten in het deelvenster Filters kunt u de zoekervaring korter maken en de zoekfunctionaliteit efficiënt maken. De facetten van het onderzoek gebruiken veelvoudige dimensies (predikaten) die u toelaten om complexe onderzoeken uit te voeren. U kunt gemakkelijk tot het gewenste niveau van detail voor een gerichter onderzoek boor.

Als u bijvoorbeeld een afbeelding zoekt, kunt u kiezen of u een bitmap- of een vectorafbeelding wilt. U kunt het zoekbereik verder beperken door het MIME-type voor de afbeelding op te geven in de zoekfacet Bestandstype. Op dezelfde manier kunt u bij het zoeken naar documenten de indeling opgeven, bijvoorbeeld PDF- of MS Word-indeling.<br />

![Deelvenster Filters in het deelvenster](assets/file-type-search.png "Poortfilters voor merken in Brand Portal")

Het **[!UICONTROL Filters]** deelvenster bevat enkele standaardfacetten, zoals- **[!UICONTROL Path Browser]**, **[!UICONTROL File Type]**, **[!UICONTROL File Size]**, **[!UICONTROL Status]** en **[!UICONTROL Orientation]**. U kunt echter aangepaste zoekfacetten [](../using/brand-portal-search-facets.md) toevoegen of specifieke zoekfacetten uit het **[!UICONTROL Filters]** deelvenster verwijderen door voorspelden toe te voegen of te verwijderen in het onderliggende zoekformulier. Zie de lijst van beschikbare en bruikbare [onderzoeksvoorspellingen op het Portaal](../using/brand-portal-search-facets.md#list-of-search-predicates)van het Merk.

Filters toepassen op de zoekopdracht met behulp van de beschikbare [zoekfacetten](../using/brand-portal-search-facets.md):

1. Klik op het bedekkingspictogram en selecteer **[!UICONTROL Filter]**.

   ![](assets/selectorrail.png)

1. Selecteer in het **[!UICONTROL Filters]** linkerdeelvenster de gewenste opties om de relevante filters toe te passen.
Gebruik bijvoorbeeld de volgende standaardfilters:

   * **[!UICONTROL Path Browser]** om elementen in een specifieke map te zoeken. Het standaardonderzoekspad van predikaat voor Browser van de Weg is, `/content/dam/mac/<tenant-id>/`die kan worden gevormd door de standaardonderzoeksvorm uit te geven.
   >[!NOTE]
   >
   >Voor gebruikers die geen beheerder zijn, geeft [!UICONTROL Path Browser] in [!UICONTROL Filter] het deelvenster alleen de inhoudsstructuur weer van de mappen (en hun bovenliggende mappen) die met hen worden gedeeld.\
   >Om gebruikers te beheren, staat Browser van de Weg toe navigerend aan om het even welke omslag in het Portaal van het Merk.

   * **[!UICONTROL File Type]** om het type elementbestand op te geven (afbeelding, document, multimedia, archief) dat u zoekt. Verder kunt u het bereik van de zoekopdracht beperken door bijvoorbeeld het MIME-type (TIFF, Bitmap, GIMP-afbeeldingen) voor de afbeelding of indeling (PDF of MS Word) voor de documenten op te geven.
   * **[!UICONTROL File Size]** om te zoeken naar elementen op basis van hun grootte. U kunt de onder- en bovengrenzen voor het groottebereik opgeven om de zoekopdracht te beperken en de maateenheid voor de zoekactie opgeven.
   * **[!UICONTROL Status]** om te zoeken naar elementen die zijn gebaseerd op de status van elementen, zoals Goedgekeurd, Wijzigingen aangevraagd, Geweigerd, In behandeling) en Verlopen.
   * **[!UICONTROL Average Rating]** het zoeken naar activa op basis van de rating van de activa.
   * **[!UICONTROL Orientation]** om te zoeken naar elementen op basis van de richting (horizontaal, verticaal, vierkant) van de elementen.
   * **[!UICONTROL Style]** om te zoeken naar elementen op basis van de stijl (gekleurd, monochroom) van de elementen.
   * **[!UICONTROL Video Format]** naar video-elementen zoeken op basis van hun indeling (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).
   U kunt [aangepaste zoekfacetten](../using/brand-portal-search-facets.md) in het deelvenster Filters gebruiken door het onderliggende zoekformulier te bewerken.

   * **[!UICONTROL Property Predicate]** als u deze functie gebruikt in het zoekformulier, kunt u zoeken naar elementen die overeenkomen met een eigenschap metadata waaraan de voorspelling wordt toegewezen.\
      Als Eigenschapvoorspelling bijvoorbeeld is toegewezen aan [!UICONTROL `jcr:content /metadata/dc:title`], kunt u zoeken naar elementen op basis van hun titel.\
      De [!UICONTROL Property Predicate] functie ondersteunt tekstzoekopdrachten naar:

      **Gedeeltelijke zinnen** Schakel het **[!UICONTROL Partial Search]** selectievakje Zoekformulier in om het zoeken naar elementen mogelijk te maken met gebruik van gedeeltelijke woordgroepen in voorspelling van eigenschappen.\
      Op deze manier kunt u naar de gewenste assets zoeken, zelfs als u niet de exacte woorden/woordgroepen opgeeft die in de metadata van de assets worden gebruikt.\
      U kunt:
      * Geef een woord op dat in de gezochte woordgroep voorkomt in het facet in het deelvenster Filters. For example, if you search for the term **climb** (and Property Predicate is mapped to [!UICONTROL `dc:title`] property), then all the assets with the word **climb** in their title phrase are returned.
      * Een deel van het woord opgeven dat in de gezochte woordgroep voorkomt, samen met een jokerteken (*) om de tussenruimten te vullen.
Bijvoorbeeld bij het zoeken naar:
         * **klimmen*** retourneert alle elementen met woorden die beginnen met de tekens &quot;klimmen&quot; in hun titelzin.
         * ***klib** retourneert alle elementen met woorden die eindigen met tekens &quot;klimmen&quot; in hun titelzin.
         * ***klib*** retourneert alle elementen met woorden bestaande uit de tekens &quot;klimmen&quot; in hun titelzin.
      **Niet-hoofdlettergevoelige tekst** Schakel het **[!UICONTROL Ignore Case]** selectievakje Formulier zoeken in om niet-hoofdlettergevoelige zoekopdrachten in te schakelen tussen voorspelling van eigenschappen. Standaard is bij het zoeken naar eigenschappen hoofdlettergevoelig.
   >[!NOTE]
   >
   >Als u **[!UICONTROL Partial Search]** selectievakje selecteert, **[!UICONTROL Ignore Case]** is dit standaard ingeschakeld.

   ![](assets/wildcard-prop-1.png)

   De zoekresultaten worden weergegeven op basis van de toegepaste filters en het aantal zoekresultaten.

   ![](assets/omnisearch-with-filters.png)

   Resultaat van middelenzoekopdracht met aantal zoekresultaten.

1. U kunt gemakkelijk naar een punt van het onderzoeksresultaat navigeren, en aan het zelfde onderzoeksresultaat terugkeren gebruikend de achterknoop in uw browser zonder het moeten de onderzoeksvraag opnieuw in werking stellen.

## Uw zoekopdrachten opslaan als slimme verzameling {#save-your-searches-as-smart-collection}

U kunt de zoekinstellingen opslaan als een slimme verzameling zodat u dezelfde zoekopdracht snel kunt herhalen zonder dat u later dezelfde instellingen opnieuw hoeft uit te voeren.

De zoekinstellingen opslaan als een slimme verzameling:

1. Tik/klik op **[!UICONTROL Save Smart Collection]** en geef een naam op voor de slimme verzameling.

   Selecteer de slimme verzameling als u deze toegankelijk wilt maken voor alle gebruikers **[!UICONTROL Public]**. Een bericht bevestigt dat de slimme verzameling is gemaakt en toegevoegd aan de lijst met opgeslagen zoekopdrachten.

   >[!NOTE]
   >
   >Gebruikers die geen beheerder zijn, kunnen worden beperkt in het openbaar maken van slimme verzamelingen om te voorkomen dat er een enorm aantal openbare slimme verzamelingen wordt gemaakt door gebruikers die geen beheerder zijn, op het Brand Portal van de organisatie. Organisaties kunnen de **[!UICONTROL Allow public smart collections creation]** configuratie uitschakelen op basis van de **[!UICONTROL General]** instellingen in het deelvenster met beheergereedschappen.

   ![](assets/save_smartcollectionui.png)

1. Als u de slimme verzameling onder een andere naam wilt opslaan en het **[!UICONTROL Public]** selectievakje wilt in- of uitschakelen, klikt u **[!UICONTROL Edit Smart Collection]**.

   ![](assets/edit_smartcollection.png)

1. Selecteer in het **[!UICONTROL Edit Smart Collection]** dialoogvenster de naam van de slimme verzameling **[!UICONTROL Save As]** en voer een naam in. Klik op **[!UICONTROL Save]**.

   ![](assets/saveas_smartsearch.png)
