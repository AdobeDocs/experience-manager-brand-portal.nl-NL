---
title: Middelen zoeken op Brand Portal
description: Met de zoekfunctie van Brand Portal kunt u snel naar relevante middelen zoeken met behulp van Omverkennend onderzoek. Met zoekfilters kunt u uw zoekopdracht verder beperken. Sla uw zoekopdrachten op als slimme verzamelingen voor de toekomst.
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1280'
ht-degree: 0%

---

# Middelen zoeken op Brand Portal {#search-assets-on-brand-portal}

Met de zoekfunctie van Brand Portal kunt u snel relevante middelen zoeken met behulp van Omnissearch en facetzoekfunctie die filters gebruiken om u te helpen uw zoekopdracht verder te beperken. U kunt middelen op dossiers of omslagniveau zoeken en uw onderzoeksresultaten opslaan als slimme inzamelingen.

>[!NOTE]
>
>Brand Portal biedt geen ondersteuning voor het zoeken naar verzamelingen met behulp van Omnsearch.
>
>Nochtans, kunt u [&#x200B; onderzoeksfilters gebruiken om de lijst van relevante inzamelingen &#x200B;](#search-collection) te krijgen.

## Middelen zoeken met Omgaan {#search-assets-using-omnisearch}

Op Brand Portal zoeken naar elementen:

1. Klik op het pictogram **[!UICONTROL Search]** op de werkbalk of druk op de toets **[!UICONTROL /]** (schuine streep naar voren) om het onderdeel Onderzoek te starten.

   ![](assets/omnisearchicon-1.png)

1. Typ in het zoekvak een trefwoord voor de elementen die u wilt zoeken.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >* Er zijn minimaal 3 tekens vereist in de zoekfunctie om zoeksuggesties te kunnen weergeven.
   >* Wanneer u naar `mountain biking` zoekt, retourneert Onderzoek alle elementen in de zoekresultaten die zowel `mountain` als `biking` beschikbaar zijn in de metagegevensvelden. Bijvoorbeeld `mountain` in het `Title` veld en `biking` in het `Description` veld. Beide termen moeten beschikbaar zijn in de metagegevensvelden om in de zoekresultaten te kunnen worden weergegeven. Het element wordt echter geretourneerd in de zoekresultaten, zelfs als slechts een van de twee termen beschikbaar is in het metagegevensveld Slimme tags. Stel dat een element `mountain` heeft als een slimme tag, maar `biking` niet heeft in andere metagegevensvelden. Vervolgens zoekt u naar `mountain biking` . Het middel wordt nog steeds in de zoekresultaten geretourneerd. Deze workflow zorgt ervoor dat elementen met relevante tags niet worden overgeslagen.

1. Maak een keuze uit de verwante suggesties die in de vervolgkeuzelijst worden weergegeven om snel toegang te krijgen tot relevante elementen.

   ![](assets/assets-search-result.png)

   *Onderzoek van Activa gebruikend Onderzoek*

Om meer over onderzoeksgedrag met slimme geëtiketteerde activa te weten, ga [&#x200B; onderzoeksresultaten en gedrag &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-manager-65/content/assets/using/search-assets) begrijpen.

## Zoeken met facetten in het deelvenster Filters {#search-using-facets-in-filters-panel}

Met zoekfacetten in het deelvenster Filters kunt u de zoekervaring korter maken en de zoekfunctionaliteit efficiënter maken. De facetten van het onderzoek gebruiken veelvoudige dimensies (predikaten) die u toelaten om complexe onderzoeken uit te voeren. U kunt gemakkelijk tot het gewenste niveau van detail voor een gerichter onderzoek boor.

Als u bijvoorbeeld een afbeelding zoekt, kunt u kiezen of u een bitmap- of een vectorafbeelding wilt. U kunt het zoekbereik verder beperken door het MIME-type van de afbeelding op te geven in de zoekfacet Bestandstype. Op dezelfde manier kunt u bij het zoeken naar documenten de indeling opgeven, bijvoorbeeld de indeling PDF of MS® Word.

![&#x200B; het paneel van Filters in Brand Portal &#x200B;](assets/file-type-search.png " het paneel van Filters in Brand Portal ")

Het deelvenster **[!UICONTROL Filters]** bevat een aantal standaardfacetten, zoals - **[!UICONTROL Path Browser]** , **[!UICONTROL File Type]** , **[!UICONTROL File Size]** , **[!UICONTROL Status]** en **[!UICONTROL Orientation]** .
Nochtans, kunt u [&#x200B; de facetten van het douaneonderzoek &#x200B;](../using/brand-portal-search-facets.md) toevoegen of specifieke degenen verwijderen uit het **[!UICONTROL Filters]** paneel. Bewerk gewoon de voorspellingen in het onderliggende zoekformulier. Zie de lijst van de beschikbare en bruikbare [&#x200B; onderzoeksvoorspelling op Brand Portal &#x200B;](../using/brand-portal-search-facets.md#list-of-search-predicates).

Om filters op uw onderzoek toe te passen, gebruikend de beschikbare [&#x200B; onderzoeksfacetten &#x200B;](../using/brand-portal-search-facets.md):

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

   U kunt [&#x200B; facetten van het douaneonderzoek gebruiken &#x200B;](../using/brand-portal-search-facets.md) in het paneel van Filters door de onderliggende Vorm van het Onderzoek uit te geven.

   * **[!UICONTROL Property Predicate]** gebruikt in het formulier Zoeken, kunt u zoeken naar elementen die overeenkomen met een metagegevenseigenschap waaraan de voorspelling is toegewezen.\
     Als Eigenschapsvoorspelling bijvoorbeeld wordt toegewezen aan `jcr:content/metadata/dc:title` , kunt u zoeken naar elementen op basis van hun titel.\
     De [!UICONTROL Property Predicate] biedt ondersteuning voor tekstzoekopdrachten naar:

     **Gedeeltelijke uitdrukkingen**
Schakel het selectievakje **[!UICONTROL Partial Search]** in Zoekformulier in om het zoeken met gebruik van gedeeltelijke woordgroepen in Eigenschapcontrole mogelijk te maken. Met deze methode kunt u naar de gewenste elementen zoeken, zelfs als u niet precies de woorden of uitdrukkingen opgeeft die in de metagegevens van de elementen worden gebruikt.

     >[!NOTE]
     >
     > Brand Portal ondersteunt de volgende velden voor gedeeltelijk zoeken:
     >
     >* `jcr:content/metadata/dc:title`
     >* `jcr:content/jcr:title`
     >* `jcr:content/metadata/dc:format`

     U kunt:
      * Geef een woord op dat in de gezochte woordgroep voorkomt in het facet in het deelvenster Filters. Bijvoorbeeld, als u naar de termijn **klimt** (en het Voorwerp van het Bezit wordt in kaart gebracht aan het `dc:title` bezit) zoekt, dan zijn alle activa met het woord **klimt** in hun titeluitdrukking teruggekeerd.
      * Specificeer een deel van het woord dat in uw gezochte uitdrukking voorkomt, samen met een vervangingskarakter (&#42;) om de hiaten te vullen.
Bijvoorbeeld bij het zoeken naar:
         * **klimt&#42;** keert alle activa terug die woorden hebben die met de karakters &quot;klimmen&quot;in hun titeluitdrukking beginnen.
         * **&#42;klimt** keert alle activa terug die woorden hebben die met karakters &quot;klimmen&quot;in hun titeluitdrukking eindigen.
         * **&#42;klimt&#42;** keert alle activa terug die woorden hebben die de karakters &quot;klimmen&quot;in hun titeluitdrukking omvatten.

     **Niet-hoofdlettergevoelige tekst**
U kunt niet-hoofdlettergevoelige zoekopdrachten toestaan in Eigenschapcontrole. Schakel het selectievakje **[!UICONTROL Ignore Case]** in het zoekformulier in. Standaard is bij het zoeken naar tekst in Eigenschappenvoorspelling onderscheid gemaakt tussen hoofdletters en kleine letters.

   >[!NOTE]
   >
   >Als u het selectievakje **[!UICONTROL Partial Search]** selecteert, is **[!UICONTROL Ignore Case]** standaard geselecteerd.

   ![](assets/wildcard-prop-1.png)

   De zoekresultaten worden weergegeven op basis van de toegepaste filters en het aantal zoekresultaten.

   ![](assets/omnisearch-with-filters.png)

   Resultaat van middelenzoekopdracht met aantal zoekresultaten.

1. U kunt gemakkelijk naar een punt van het onderzoeksresultaat navigeren, en aan het zelfde onderzoeksresultaat terugkeren gebruikend de achterknoop in uw browser zonder het moeten de onderzoeksvraag opnieuw in werking stellen.

## Uw zoekopdrachten opslaan als slimme verzameling {#save-your-searches-as-smart-collection}

U kunt de zoekinstellingen opslaan als een slimme verzameling zodat u dezelfde zoekopdracht snel kunt herhalen zonder dat u later dezelfde instellingen opnieuw hoeft uit te voeren. U kunt echter geen zoekfilters toepassen in een verzameling.

De zoekinstellingen opslaan als een slimme verzameling:

1. Klik op **[!UICONTROL Save Smart Collection]** en geef een naam op voor de slimme verzameling.

   Selecteer **[!UICONTROL Public]** als u de slimme verzameling toegankelijk wilt maken voor alle gebruikers. Een bericht bevestigt dat de slimme verzameling is gemaakt en toegevoegd aan de lijst met opgeslagen zoekopdrachten.

   >[!NOTE]
   >
   >U kunt niet-beheerders beperken in het openbaar maken van slimme verzamelingen om te voorkomen dat een groot aantal openbare slimme verzamelingen wordt gemaakt door gebruikers die geen beheerder zijn, op de Brand Portal van de organisatie. Organisaties kunnen de **[!UICONTROL Allow public smart collections creation]** -configuratie uitschakelen op basis van de **[!UICONTROL General]** -instellingen die beschikbaar zijn in het deelvenster met beheergereedschappen.

   ![](assets/save_smartcollectionui.png)

1. Als u de slimme verzameling onder een andere naam wilt opslaan en het selectievakje **[!UICONTROL Public]** wilt in- of uitschakelen, klikt u op **[!UICONTROL Edit Smart Collection]** .

   ![](assets/edit_smartcollection.png)

1. Selecteer **[!UICONTROL Save As]** in het dialoogvenster **[!UICONTROL Edit Smart Collection]** en voer een naam in voor de slimme verzameling. Klik op **[!UICONTROL Save]**.

   ![](assets/saveas_smartsearch.png)


## Zoekverzameling {#search-collection}

Omnissearch wordt niet ondersteund voor verzamelingen. U kunt echter wel zoekfilters toepassen om de relevante verzamelingen weer te geven vanuit de interface van [!UICONTROL Collections] .

Klik vanuit de interface [!UICONTROL Collections] op het bedekkingspictogram om het filterdeelvenster in de linkerspoorstaaf te openen. Pas enkele of meerdere zoekfilters toe op basis van de beschikbare filters (`modified date` , `access type` en `tags` ). De meest relevante verzameling verzamelingen wordt weergegeven op basis van de toegepaste filters.

![](assets/collection-search.png)
