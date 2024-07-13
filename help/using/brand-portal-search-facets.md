---
title: Aangepaste zoekfacetten gebruiken
seo-title: Use custom search facets
description: Beheerders kunnen voorspelden voor zoekopdrachten toevoegen aan het deelvenster Filters om de zoekfunctie aan te passen en veelzijdig te maken.
seo-description: Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
role: Admin
exl-id: c07e1268-2c83-40ba-8dcd-5dade3a10141
source-git-commit: c5c16d2aa1b488efac90dbc77023bba9897ae929
workflow-type: tm+mt
source-wordcount: '1218'
ht-degree: 2%

---

# Aangepaste zoekfacetten gebruiken {#use-custom-search-facets}

Beheerders kunnen voorspelden voor zoekopdrachten toevoegen aan het deelvenster [!UICONTROL Filters] om de zoekfunctie aan te passen en veelzijdig te maken.

Brand Portal steunt [ beperkte onderzoek ](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) naar korrelige onderzoeken van goedgekeurde merkactiva, die mogelijk toe te schrijven aan [**Filters** paneel ](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) is. Zoekfacetten worden via **[!UICONTROL Search Form]** in de beheerfuncties beschikbaar gesteld in het deelvenster Filters. Een standaardzoekformulier met de naam Asset Admin Search Rail bestaat op de pagina Search Forms in de beheerprogramma&#39;s. Beheerders kunnen het standaarddeelvenster Filters echter aanpassen door het standaardformulier voor zoekopdrachten (Asset Admin Search Rail) te bewerken door zoekvoorspelden toe te voegen, te wijzigen of te verwijderen, waardoor de zoekfunctionaliteit veelzijdig wordt.

U kunt verschillende zoekvoorinstellingen gebruiken om het deelvenster **[!UICONTROL Filters]** aan te passen. Voeg bijvoorbeeld de voorspelling van de eigenschap toe om te zoeken naar elementen die overeenkomen met één eigenschap die u in deze voorspelling opgeeft. Voeg de voorspelling van de opties toe om te zoeken naar elementen die overeenkomen met een of meer waarden die u voor een bepaalde eigenschap opgeeft. Voeg het datumbereik toe om te zoeken naar elementen die binnen een opgegeven datumbereik zijn gemaakt.

>[!NOTE]
>
>Experience Manager Assets staat organisaties toe om [ de aangepaste onderzoeksvormen van AEM Auteur ](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) aan Brand Portal te publiceren, in plaats van het opnieuw creëren van de zelfde vorm op Brand Portal.

## Een zoekvoorspelling toevoegen {#add-a-search-predicate}

Een voorspelling van zoekopdrachten toevoegen aan het deelvenster **[!UICONTROL Filters]** :

1. Als u beheergereedschappen wilt openen, klikt u op het logo van de Experience Manager op de werkbalk boven in het scherm.

   ![](assets/aemlogo.png)

1. Klik in het deelvenster met beheergereedschappen op **[!UICONTROL Search Forms]** .

   ![](assets/navigation-panel-1.png)

1. Selecteer **[!UICONTROL Assets Admin Search Rail]** op de pagina **[!UICONTROL Search Forms]** .

   ![](assets/search-forms-page.png)

1. Klik op de werkbalk boven in het scherm op **[!UICONTROL Edit]** om het zoekformulier te openen.

   ![](assets/edit-search-form-1.png)

1. Sleep op de pagina [!UICONTROL Edit Search Form] een voorspelling van het tabblad [!UICONTROL Select Predicate] naar het hoofdvenster. Sleep bijvoorbeeld **[!UICONTROL Property Predicate]** .

   Het veld **[!UICONTROL Property]** wordt weergegeven in het hoofdvenster en op het tabblad **[!UICONTROL Settings]** rechts ziet u de voorspelling van de eigenschap.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >Het koptekstlabel op het tabblad **[!UICONTROL Settings]** geeft het type voorspelling aan dat u selecteert.

1. Voer op het tabblad **[!UICONTROL Settings]** een label, plaatsaanduidingstekst en beschrijving in voor de voorspelling van de eigenschap.

   * Selecteer **[!UICONTROL Partial Search]** als u wilt toestaan dat op basis van de opgegeven eigenschapswaarde gedeeltelijk wordt gezocht naar woordgroepen (en zoeken naar jokertekens) van elementen. Standaard wordt in de voorvertoning de zoekopdracht met volledige tekst ondersteund.
   * Selecteer **[!UICONTROL Ignore Case]** als u wilt dat het zoeken naar elementen op basis van de eigenschapswaarde niet hoofdlettergevoelig is. Standaard is het zoeken naar eigenschapswaarden in de zoekfilter hoofdlettergevoelig.

   >[!NOTE]
   >
   >Als u het selectievakje **[!UICONTROL Partial Search]** inschakelt, is **[!UICONTROL Ignore Case]** standaard ingeschakeld.

1. Open in het veld **[!UICONTROL Property Name]** de eigenschapkiezer en selecteer de eigenschap op basis waarvan de zoekopdracht wordt uitgevoerd. U kunt ook een naam voor de eigenschap invoeren. Voer bijvoorbeeld `jcr :content/metadata/dc:title` of `./jcr:content/metadata/dc:title` in.

   >[!NOTE]
   >
   >In Brand Portal worden alle tekenreekseigenschappen (behalve de eigenschappen die beginnen met `xmp` ) in `jcrcontent/metadata` of `dam:asset` standaard geïndexeerd. Alle andere aangepaste eigenschappen van een willekeurig type worden standaard niet geïndexeerd.
   >
   >Om het even welk bezit dat wordt geïndexeerd kan worden gebruikt terwijl het creëren van een bezit voorspelt. Als om het even welk niet-geïndexeerd bezit wordt gevormd, kan de onderzoeksvraag op een niet-geïndexeerd bezit geen onderzoeksresultaat geven.

   ![](assets/title-prop.png)

1. Klik op **[!UICONTROL Done]** om de instellingen op te slaan.
1. Klik in de gebruikersinterface van [!UICONTROL Assets] op het bedekkingspictogram en kies **[!UICONTROL Filter]** om naar het deelvenster **[!UICONTROL Filters]** te navigeren. Het predicaat **[!UICONTROL Property]** wordt toegevoegd aan het deelvenster.

   ![](assets/property-filter-panel.png)

1. Voer in het tekstvak **[!UICONTROL Property]** een titel in voor het element dat moet worden doorzocht. Bijvoorbeeld &#39;Adobe&#39;. Wanneer u een zoekopdracht uitvoert, worden elementen waarvan de titel overeenkomt met de Adobe, weergegeven in de zoekresultaten.

## Lijst met zoekresultaten {#list-of-search-predicates}

Net als bij de manier waarop u een **[!UICONTROL Property]** voorspelling toevoegt, kunt u de volgende voorspelling toevoegen aan het deelvenster **[!UICONTROL Filters]** :

| **Predicate Naam** | **Beschrijving** | **Eigenschappen** |
|-------|-------|----------|
| **[!UICONTROL Path Browser]** | Zoeken voorspelt dat op een bepaalde locatie naar elementen wordt gezocht. **Nota:** *voor een het programma geopende gebruiker, wegbrowser op Filter toont slechts de inhoudsstructuur van de omslagen (en hun voorouders) die met de gebruiker worden gedeeld.* <br> Gebruikers met beheerdersrechten kunnen zoeken in middelen in een willekeurige map door met de padbrowser naar die map te navigeren. <br> Gebruikers die geen beheerder zijn, kunnen zoeken in middelen in een map (toegankelijk voor hen) door naar die map te navigeren in de padbrowser. | <ul><li>Veldlabel</li><li>Pad</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Property]** | Zoeken in elementen op basis van een bepaalde eigenschap voor metagegevens. **Nota:** *bij het selecteren van Gedeeltelijk Onderzoek, negeert het Geval wordt geselecteerd door gebrek*. | <ul><li>Veldlabel</li><li>Plaatsaanduiding</li><li>Eigenschapnaam</li><li>Gedeeltelijk zoeken</li><li>Hoofdlettergebruik negeren</li><li> Beschrijving</li></ul> |
| **[!UICONTROL Multi-Value Property]** | Gelijkaardig aan bezit voorspelt maar staat veelvoudige inputwaarden toe, die door een scheidingsteken (gebrek is COMMA [ worden gescheiden, ]) activa die om het even welke inputwaarden aanpassen zijn teruggekeerd in resultaten. | <ul><li>Veldlabel</li><li>Plaatsaanduiding</li><li>Eigenschapnaam</li><li>Delimiter-ondersteuning</li><li>Hoofdlettergebruik negeren</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Tags]** | Zoeken voorspellen om elementen te zoeken op basis van tags. U kunt het bezit van de Weg vormen om diverse markeringen in de lijst van Markeringen te bevolken. *Opmerking: mogelijk moeten beheerders de padwaarde wijzigen, bijvoorbeeld [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`] , als ze het zoekformulier publiceren vanuit AEM, waar het pad geen huurdersgegevens bevat, bijvoorbeeld [!UICONTROL `/etc/tags/<custom_tag_namespace>`] . | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Pad</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Path]** | Zoeken voorspelt dat op een bepaalde locatie naar elementen wordt gezocht. | <ul><li>Veldlabel</li><li>Pad</li><li>Beschrijving</li></ul> |                                                     |
| **[!UICONTROL Relative Date]** | Zoeken voorspelt dat er wordt gezocht naar elementen op basis van de relatieve datum waarop deze zijn gemaakt. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Relatieve datum</li></ul> |
| **[!UICONTROL Range]** | Zoeken voorspelt hoe u elementen kunt zoeken die binnen een opgegeven reeks eigenschapswaarden liggen. In het deelvenster Filters kunt u minimum- en maximumeigenschapswaarden voor het bereik opgeven. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Date Range]** | Zoeken voorspelt hoe u elementen die binnen een opgegeven bereik zijn gemaakt, kunt zoeken naar een datumeigenschap. In het deelvenster Filters kunt u begin- en einddatums opgeven. | <ul><li>Veldlabel</li><li>Plaatsaanduiding</li><li>Eigenschapnaam</li><li>Tekst bereik (van)</li><li>Tekst bereik (naar)</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Date]** | Zoeken voorspelt hoe elementen op basis van een schuifregelaar worden doorzocht op basis van een eigenschap date. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL File Size]** | Zoeken voorspelt hoe u elementen kunt zoeken op basis van hun grootte. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Pad</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Asset Last Modified]** | Zoeken voorspelt hoe u elementen kunt zoeken op basis van de datum waarop het laatst is gewijzigd. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Approval Status]** | Zoeken voorspelt hoe u elementen kunt zoeken op basis van de eigenschap voor metagegevens van goedkeuring. De standaardbezitsnaam is **dam:status**. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Checkout Status]** | Zoeken voorspelt dat er wordt gezocht naar middelen op basis van de uitcheckstatus van een middel toen het vanuit AEM Assets werd gepubliceerd. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Checked Out By]** | Zoeken voorspelt hoe u elementen kunt zoeken op basis van de gebruiker die het element heeft uitgecheckt. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Expiry Status]** | Zoeken voorspelt dat er wordt gezocht naar elementen die zijn gebaseerd op de vervalstatus. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Member of collection]** | Zoeken voorspelt hoe u elementen kunt zoeken op basis van het feit of een element deel uitmaakt van een verzameling. | Beschrijving |
| **[!UICONTROL Hidden]** | Dit predikaat is niet uitdrukkelijk zichtbaar aan het eind - gebruikers en voor om het even welke verborgen beperkingen typisch gebruikt voor het beperken van het type van onderzoeksresultaten aan **dam:Activa**. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |

>[!NOTE]
>
>* Gebruik **[!UICONTROL Options Predicate]** , **[!UICONTROL Publish Status Predicate]** en **[!UICONTROL Rating Predicate]** niet omdat deze voorspellingen niet functioneren in Brand Portal.
>* Voorspelfunctie voor maptypen `(nt:folder type)` wordt niet ondersteund op Brand Portal en kan prestatieproblemen veroorzaken. Als het aanwezig is in het gepubliceerde aangepaste zoekformulier, kan het worden verwijderd door het zoekformulier te bewerken.

## Een zoekvoorspelling verwijderen {#delete-a-search-predicate}

Ga als volgt te werk om een voorspeld in een zoekopdracht te verwijderen:

1. Klik op het logo van de Adobe voor toegang tot beheergereedschappen.

   ![](assets/aemlogo.png)

1. Klik in het deelvenster met beheergereedschappen op **[!UICONTROL Search Forms]** .

   ![](assets/navigation-panel-2.png)

1. Selecteer **[!UICONTROL Assets Admin Search Rail]** op de pagina **[!UICONTROL Search Forms]** .

   ![](assets/search-forms-page.png)

1. Klik op de werkbalk boven in het scherm op **[!UICONTROL Edit]** om het zoekformulier te openen.

   ![](assets/edit-search-form-2.png)

1. Selecteer op de pagina [!UICONTROL Edit Search Form] in het hoofdvenster de voorspelling die u wilt verwijderen. Selecteer bijvoorbeeld **[!UICONTROL Property Predicate]** .

   Op het tabblad **[!UICONTROL Settings]** aan de rechterkant worden voorspelvelden van eigenschappen weergegeven.

1. Als u de voorspelling van de eigenschap wilt verwijderen, klikt u op het binpictogram. Klik in het dialoogvenster **[!UICONTROL Delete Field]** op **[!UICONTROL Delete]** om de verwijderactie te bevestigen.

   Het veld **[!UICONTROL Property Predicate]** wordt verwijderd uit het hoofdvenster en het tabblad **[!UICONTROL Settings]** wordt leeg.

   ![](assets/search-form-delete-predicate.png)

1. Klik op **[!UICONTROL Done]** op de werkbalk om de wijzigingen op te slaan.
1. Klik in de gebruikersinterface van **[!UICONTROL Assets]** op het bedekkingspictogram en kies **[!UICONTROL Filter]** om naar het deelvenster **[!UICONTROL Filters]** te navigeren. De voorspelling **[!UICONTROL Property]** wordt verwijderd uit het deelvenster.

   ![](assets/property-predicate-removed.png)
