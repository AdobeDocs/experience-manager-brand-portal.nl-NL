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
source-git-commit: cbdd943b904882cc9a455bab24c3cf732d5966ca
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 2%

---

# Middelen zoeken op Brand Portal {#search-assets-on-brand-portal}

Met de zoekfunctie van Brand Portal kunt u snel relevante middelen zoeken aan de hand van alzoekopdrachten en zoeken naar facetten die filters gebruiken om uw zoekopdracht verder te beperken. U kunt middelen op dossiers of omslagniveau zoeken en uw onderzoeksresultaten opslaan als slimme inzamelingen.

>[!NOTE]
>
>Brand Portal biedt geen ondersteuning voor het zoeken naar verzamelingen met alzoekopdrachten.
>
>Nochtans, kunt u [ onderzoeksfilters gebruiken om de lijst van relevante inzamelingen ](#search-collection) te krijgen.

## Middelen zoeken met Omgaan {#search-assets-using-omnisearch}

Op Brand Portal zoeken naar elementen:

1. Klik op het pictogram **[!UICONTROL Search]** op de werkbalk of druk op de toets &quot;**[!UICONTROL /]**&quot; om het venster te openen.

   ![](assets/omnisearchicon-1.png)

1. Typ in het zoekvak een trefwoord voor de elementen die u wilt zoeken.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >* Er zijn minimaal 3 tekens nodig om zoeksuggesties te kunnen weergeven.
   >* Wanneer u `mountain biking` zoekt, retourneert de zoekfunctie alle elementen in de zoekresultaten die zowel `mountain` als `biking` beschikbaar zijn in de metagegevensvelden. Bijvoorbeeld `mountain` in het `Title` veld en `biking` in het `Description` veld. Beide termen moeten beschikbaar zijn in de metagegevensvelden om in de zoekresultaten te kunnen worden weergegeven. Het middel wordt echter in de zoekresultaten geretourneerd als slechts een van de twee termen beschikbaar is in het metagegevensveld Slimme tags. Als een element bijvoorbeeld `mountain` bevat als een van de slimme tags en `biking` niet bevat in een ander metagegevensveld en u zoekt naar `mountain biking` , retourneert de zoekopdracht het element nog steeds in de zoekresultaten.

1. Maak een keuze uit de verwante suggesties die in de vervolgkeuzelijst worden weergegeven, zodat u snel toegang hebt tot relevante elementen.

   ![](assets/assets-search-result.png)

   *Onderzoek van Activa die omonderzoek* gebruiken

Om over onderzoeksgedrag met slimme geëtiketteerde activa te weten, zie [ onderzoeksresultaten en gedrag ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html) begrijpen.

## Zoeken met facetten in het deelvenster Filters {#search-using-facets-in-filters-panel}

Met zoekfacetten in het deelvenster Filters kunt u de zoekervaring korter maken en de zoekfunctionaliteit efficiënt maken. De facetten van het onderzoek gebruiken veelvoudige dimensies (predikaten) die u toelaten om complexe onderzoeken uit te voeren. U kunt gemakkelijk tot het gewenste niveau van detail voor een gerichter onderzoek boor.

Als u bijvoorbeeld een afbeelding zoekt, kunt u kiezen of u een bitmap- of een vectorafbeelding wilt. U kunt het zoekbereik verder beperken door het MIME-type voor de afbeelding op te geven in de zoekfacet Bestandstype. Op dezelfde manier kunt u bij het zoeken naar documenten de indeling opgeven, bijvoorbeeld de indeling PDF of MS® Word.

![ het paneel van Filters in Brand Portal ](assets/file-type-search.png " het paneel van Filters in Brand Portal ")

Het deelvenster **[!UICONTROL Filters]** bevat een aantal standaardfacetten, zoals - **[!UICONTROL Path Browser]** , **[!UICONTROL File Type]** , **[!UICONTROL File Size]** , **[!UICONTROL Status]** en **[!UICONTROL Orientation]** . Nochtans, kunt u [ de facetten van het douaneonderzoek ](../using/brand-portal-search-facets.md) toevoegen of specifieke onderzoeksfacetten verwijderen uit het **[!UICONTROL Filters]** paneel door voorspelden in de onderliggende Vorm van het Onderzoek toe te voegen of te verwijderen. Zie de lijst van de beschikbare en bruikbare [ onderzoeksvoorspelling op Brand Portal ](../using/brand-portal-search-facets.md#list-of-search-predicates).

Om filters op uw onderzoek toe te passen, gebruikend de beschikbare [ onderzoeksfacetten ](../using/brand-portal-search-facets.md):

1. Klik op het bedekkingspictogram en selecteer **[!UICONTROL Filter]** .

   ![](assets/selectorrail.png)

1. Selecteer in het deelvenster **[!UICONTROL Filters]** aan de linkerkant de juiste opties om de relevante filters toe te passen.
Gebruik bijvoorbeeld de volgende standaardfilters:

   * **[!UICONTROL Path Browser]** om te zoeken in elementen in een specifieke map. Het standaardzoekpad van de voorspelling voor de padbrowser is `/content/dam/mac/<tenant-id>/` , dat kan worden geconfigureerd door het standaardzoekformulier te bewerken.

   >[!NOTE]
   >
   >Voor gebruikers die geen beheerder zijn, geeft [!UICONTROL Path Browser] in het deelvenster [!UICONTROL Filter] alleen de inhoudsstructuur weer van de mappen (en hun bovenliggende mappen) die met hen worden gedeeld.\
   >Als u gebruikers wilt beheren, kunt u in de padbrowser naar een willekeurige map in Brand Portal navigeren.

   * **[!UICONTROL File Type]** om het type elementbestand op te geven (afbeelding, document, multimedia, archief) dat u zoekt. Verder kunt u het bereik van uw zoekopdracht beperken door bijvoorbeeld het MIME-type (TIFF, Bitmap, GIMP-afbeeldingen) voor de afbeelding of de indeling (PDF of MS® Word) voor de documenten op te geven.
   * **[!UICONTROL File Size]** om te zoeken naar elementen op basis van hun grootte. U kunt de onder- en bovengrenzen voor het groottebereik opgeven om de zoekopdracht te beperken en de maateenheid voor de zoekactie opgeven.
   * **[!UICONTROL Status]** om te zoeken naar elementen die zijn gebaseerd op de status van elementen, zoals Goedkeuring (Goedgekeurd, Wijzigingen aangevraagd, Geweigerd, In behandeling) en Verlopen.
   * **[!UICONTROL Average Rating]** om te zoeken naar elementen op basis van de waardering van de elementen.
   * **[!UICONTROL Orientation]** om te zoeken naar elementen op basis van de richting (horizontaal, verticaal, vierkant) van de elementen.
   * **[!UICONTROL Style]** om te zoeken naar elementen op basis van de stijl (gekleurd, monochroom) van de elementen.
   * **[!UICONTROL Video Format]** om te zoeken naar video-elementen op basis van hun indeling (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).

   U kunt [ facetten van het douaneonderzoek gebruiken ](../using/brand-portal-search-facets.md) in het paneel van Filters door de onderliggende Vorm van het Onderzoek uit te geven.

   * **[!UICONTROL Property Predicate]** gebruikt in het zoekformulier, kunt u zoeken naar elementen die overeenkomen met een eigenschap metadata waaraan de voorspelling wordt toegewezen.\
     Als Eigenschapsvoorspelling bijvoorbeeld wordt toegewezen aan [!UICONTROL `jcr:content /metadata/dc:title`] , kunt u zoeken naar elementen op basis van hun titel.\
     De [!UICONTROL Property Predicate] biedt ondersteuning voor tekstzoekopdrachten naar:

     **Gedeeltelijke uitdrukkingen**
Schakel het selectievakje **[!UICONTROL Partial Search]** in Zoekformulier in om het zoeken naar elementen mogelijk te maken met gebruik van gedeeltelijke woordgroepen in voorspelling van eigenschappen. Op deze manier kunt u naar de gewenste assets zoeken, zelfs als u niet de exacte woorden/woordgroepen opgeeft die in de metadata van de assets worden gebruikt.

     >[!NOTE]
     >
     > Brand Portal ondersteunt de volgende velden voor gedeeltelijk zoeken:
     >* jcr:content/metadata/dc:title
     >* jcr:content/jcr:title
     >* jcr:content/metadata/dam:search_Promoting
     >* jcr:content/metadata/dc:format

     U kunt:
      * Geef een woord op dat in de gezochte woordgroep voorkomt in het facet in het deelvenster Filters. Bijvoorbeeld, als u naar de termijn **klimt** (en het Voorwerp van het Bezit wordt in kaart gebracht aan [!UICONTROL `dc:title`] bezit) zoekt, dan zijn alle activa met het woord **klimt** in hun titeluitdrukking teruggekeerd.
      * Specificeer een deel van het woord, dat in uw gezochte uitdrukking voorkomt, samen met vervangingskarakter (&#42;) om de hiaten te vullen.
Bijvoorbeeld bij het zoeken naar:
         * **klimt&#42;** keert alle activa terug die woorden hebben die met de karakters &quot;klimmen&quot;in hun titeluitdrukking beginnen.
         * **&#42;klimt** keert alle activa terug die woorden hebben die met karakters &quot;klimmen&quot;in hun titeluitdrukking eindigen.
         * **&#42;klimt&#42;** keert alle activa terug die woorden hebben die de karakters &quot;klimmen&quot;in hun titeluitdrukking omvatten.

     **Niet-hoofdlettergevoelige tekst**
Schakel het selectievakje **[!UICONTROL Ignore Case]** in Zoekformulier in als u wilt toestaan dat niet-hoofdlettergevoelig wordt gezocht in de voorspelling van eigenschappen. Standaard is de tekstzoekopdracht voor de voorspelling van eigenschappen hoofdlettergevoelig.

   >[!NOTE]
   >
   >Als u het selectievakje **[!UICONTROL Partial Search]** inschakelt, is **[!UICONTROL Ignore Case]** standaard ingeschakeld.

   ![](assets/wildcard-prop-1.png)

   De zoekresultaten worden weergegeven op basis van de toegepaste filters en het aantal zoekresultaten.

   ![](assets/omnisearch-with-filters.png)

   Resultaat van middelenzoekopdracht met aantal zoekresultaten.

1. U kunt gemakkelijk naar een punt van het onderzoeksresultaat navigeren, en aan het zelfde onderzoeksresultaat terugkeren gebruikend de achterknoop in uw browser zonder het moeten de onderzoeksvraag opnieuw in werking stellen.

## Uw zoekopdrachten opslaan als slimme verzameling {#save-your-searches-as-smart-collection}

U kunt de zoekinstellingen opslaan als een slimme verzameling zodat u dezelfde zoekopdracht snel kunt herhalen zonder dat u later dezelfde instellingen opnieuw hoeft uit te voeren. U kunt echter geen zoekfilters toepassen in een verzameling.

De zoekinstellingen opslaan als een slimme verzameling:

1. Tik/klik **[!UICONTROL Save Smart Collection]** en geef een naam op voor de slimme verzameling.

   Selecteer **[!UICONTROL Public]** als u de slimme verzameling toegankelijk wilt maken voor alle gebruikers. Een bericht bevestigt dat de slimme verzameling is gemaakt en toegevoegd aan de lijst met opgeslagen zoekopdrachten.

   >[!NOTE]
   >
   >Niet-beheerders kunnen worden beperkt in het openbaar maken van slimme verzamelingen om te voorkomen dat een enorm aantal openbare slimme verzamelingen wordt gemaakt door gebruikers die geen beheerder zijn, op de Brand Portal van de organisatie. Organisaties kunnen de **[!UICONTROL Allow public smart collections creation]** -configuratie uitschakelen via **[!UICONTROL General]** -instellingen die beschikbaar zijn in het deelvenster met beheergereedschappen.

   ![](assets/save_smartcollectionui.png)

1. Als u de slimme verzameling onder een andere naam wilt opslaan en het selectievakje **[!UICONTROL Public]** wilt in- of uitschakelen, klikt u op **[!UICONTROL Edit Smart Collection]** .

   ![](assets/edit_smartcollection.png)

1. Selecteer **[!UICONTROL Save As]** in het dialoogvenster **[!UICONTROL Edit Smart Collection]** en voer een naam in voor de slimme verzameling. Klik op **[!UICONTROL Save]**.

   ![](assets/saveas_smartsearch.png)


## Zoekverzameling {#search-collection}

Omnissearch wordt niet ondersteund voor verzamelingen. U kunt echter wel zoekfilters toepassen om de relevante verzamelingen weer te geven vanuit de interface van [!UICONTROL Collections] .

Klik vanuit de interface [!UICONTROL Collections] op het bedekkingspictogram om het filterdeelvenster in de linkerspoorstaaf te openen. Pas enkele of meerdere zoekfilters toe op basis van de beschikbare filters (`modified date` , `access type` en `tags` ). De meest relevante verzameling verzamelingen wordt weergegeven op basis van de toegepaste filters.

![](assets/collection-search.png)
