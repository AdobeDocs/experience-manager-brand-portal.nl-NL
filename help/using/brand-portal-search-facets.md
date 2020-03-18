---
title: Aangepaste zoekfacetten gebruiken
seo-title: Aangepaste zoekfacetten gebruiken
description: Beheerders kunnen voorspelden voor zoekopdrachten toevoegen aan het deelvenster Filters om de zoekfunctie aan te passen en veelzijdig te maken.
seo-description: Beheerders kunnen voorspelden voor zoekopdrachten toevoegen aan het deelvenster Filters om de zoekfunctie aan te passen en veelzijdig te maken.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Aangepaste zoekfacetten gebruiken {#use-custom-search-facets}

Beheerders kunnen voorspelden voor zoekopdrachten aan het [!UICONTROL Filters] deelvenster toevoegen om de zoekfunctie aan te passen en veelzijdig te maken.

Brand Portal ondersteunt [beperkte zoekopdrachten](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) naar korrelige zoekopdrachten naar goedgekeurde merkmiddelen, wat mogelijk is vanwege het deelvenster [**Filters **](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). De facetten van het onderzoek worden beschikbaar gemaakt op het paneel van Filters door **[!UICONTROL Search Form]**in de admin hulpmiddelen. Een standaardzoekformulier met de naam Asset Admin Search Rail bestaat op de pagina Zoekformulieren in beheerprogramma&#39;s. Beheerders kunnen het standaarddeelvenster Filters echter aanpassen door het standaardformulier voor zoekopdrachten (Asset Admin Search Rail) te bewerken door zoekvoorspelden toe te voegen, te wijzigen of te verwijderen, waardoor de zoekfunctionaliteit veelzijdig wordt.

U kunt verschillende zoekvoorinstellingen gebruiken om het **[!UICONTROL Filters]** deelvenster aan te passen. Voeg bijvoorbeeld de voorspelling van de eigenschap toe om te zoeken naar elementen die overeenkomen met één eigenschap die u in deze voorspelling opgeeft. Voeg de voorspelling van de opties toe om te zoeken naar elementen die overeenkomen met een of meer waarden die u voor een bepaalde eigenschap opgeeft. Voeg het datumbereik toe om te zoeken naar elementen die binnen een opgegeven datumbereik zijn gemaakt.

>[!NOTE]
>
>Met AEM kunnen organisaties de aangepaste zoekformulieren van AEM Author [to Brand Portal](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) publiceren in plaats van hetzelfde formulier opnieuw te maken op Brand Portal.

## Een zoekvoorspelling toevoegen {#add-a-search-predicate}

Een voorspelling van zoekopdrachten toevoegen aan het **[!UICONTROL Filters]** deelvenster:

1. Als u beheergereedschappen wilt openen, klikt u op het AEM-logo op de werkbalk boven in het venster.

   ![](assets/aemlogo.png)

1. Klik in het deelvenster met beheergereedschappen op **[!UICONTROL Search Forms]**.

   ![](assets/navigation-panel-1.png)

1. Selecteer op de **[!UICONTROL Search Forms]** pagina **[!UICONTROL Assets Admin Search Rail]**.

   ![](assets/search-forms-page.png)

1. Klik op de werkbalk boven in het scherm om het zoekformulier **[!UICONTROL Edit]** te openen.

   ![](assets/edit-search-form-1.png)

1. In the [!UICONTROL Edit Search Form] page, drag a predicate from the [!UICONTROL Select Predicate] tab to the main pane. Sleep bijvoorbeeld **[!UICONTROL Property Predicate]**.

   Het **[!UICONTROL Property]** veld wordt weergegeven in het hoofdvenster en op de **[!UICONTROL Settings]** tab rechts ziet u de voorspelling van de eigenschap.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >Het koptekstlabel op het **[!UICONTROL Settings]** tabblad geeft het type voorspelling aan dat u selecteert.

1. Voer op het **[!UICONTROL Settings]** tabblad een label, plaatsaanduidingstekst en een beschrijving in voor de voorspelling van de eigenschap.

   * Selecteer deze optie **[!UICONTROL Partial Search]** als u wilt toestaan dat op basis van de opgegeven eigenschapswaarde wordt gezocht naar woordgroepen (en zoeken naar jokertekens) van elementen. Standaard wordt in de voorvertoning de zoekopdracht met volledige tekst ondersteund.
   * Select **[!UICONTROL Ignore Case]**, if you want the asset search based on property value to be non-case sensitive. Standaard is het zoeken naar eigenschapswaarden in de zoekfilter hoofdlettergevoelig.
   >[!NOTE]
   >
   >Als u **[!UICONTROL Partial Search]** selectievakje selecteert, **[!UICONTROL Ignore Case]** is dit standaard ingeschakeld.

1. Open in het **[!UICONTROL Property Name]** veld de eigenschapkiezer en selecteer de eigenschap op basis waarvan de zoekopdracht wordt uitgevoerd. U kunt ook een naam voor de eigenschap invoeren. Voer bijvoorbeeld `  jcr :content/metadata/dc:title` of `./jcr:content/metadata/dc:title` in.

   ![](assets/title-prop.png)

1. Click **[!UICONTROL Done]** to save the settings.
1. Klik in de [!UICONTROL Assets] gebruikersinterface op het bedekkingspictogram en kies **[!UICONTROL Filter]** om naar het **[!UICONTROL Filters]** deelvenster te navigeren. Het predicaat **[!UICONTROL Property]** wordt toegevoegd aan het deelvenster.

   ![](assets/property-filter-panel.png)

1. Enter a title for the asset to be searched in the **[!UICONTROL Property]** text box. For example, &quot;Adobe&quot;. When you perform a search, assets with the title matching &quot;Adobe&quot; are displayed in the search results.

## List of search predicates {#list-of-search-predicates}

Similar to the way you add a **[!UICONTROL Property]** predicate, you can add the following predicates to the **[!UICONTROL Filters]** panel:

| **Naam voorspelling** | **Beschrijving** | **Eigenschappen** |
|-------|-------|----------|
| **[!UICONTROL Path Browser]** | Zoeken voorspelt dat op een bepaalde locatie naar elementen wordt gezocht. **Note:** *For a logged-in user, path browser on Filter shows only the content structure of the folders (and their ancestors) shared with the user.* <br> Admin users can search assets in any folder by navigating to that folder using Path Browser. <br> Niet-beheerders kunnen echter naar elementen in een map (die voor hen toegankelijk is) zoeken door in de padbrowser naar die map te navigeren. | <ul><li>Veldlabel</li><li>Pad</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Property]** | Zoeken in elementen op basis van een bepaalde eigenschap voor metagegevens. **Opmerking:** Bij *het selecteren van Gedeeltelijk zoeken is Hoofd-kleine letter negeren standaard* geselecteerd. | <ul><li>Veldlabel</li><li>Plaatsaanduiding</li><li>Eigenschapnaam</li><li>Gedeeltelijk zoeken</li><li>Hoofdlettergebruik negeren</li><li> Beschrijving</li></ul> |
| **[!UICONTROL Multi-Value Property]** | Vergelijkbaar met eigenschap voorspellen, maar er kunnen meerdere invoerwaarden worden geretourneerd, gescheiden door een scheidingsteken (standaard is COMMA[,]standaard). | <ul><li>Veldlabel</li><li>Plaatsaanduiding</li><li>Eigenschapnaam</li><li>Delimiter-ondersteuning</li><li>Hoofdlettergebruik negeren</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Tags]** | Zoeken voorspellen om elementen te zoeken op basis van tags. U kunt het bezit van de Weg vormen om diverse markeringen in de lijst van Markeringen te bevolken. *Opmerking: Beheerders moeten mogelijk de padwaarde wijzigen [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]als ze het zoekformulier publiceren vanuit AEM, waarbij het pad bijvoorbeeld geen huurdersgegevens bevat [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Pad</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Path]** | Zoeken voorspelt dat op een bepaalde locatie naar elementen wordt gezocht. | <ul><li>Veldlabel</li><li>Pad</li><li>Beschrijving</li></ul> |  |
| **[!UICONTROL Relative Date]** | Zoeken voorspelt dat er wordt gezocht naar elementen op basis van de relatieve datum waarop deze zijn gemaakt. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Relatieve datum</li></ul> |
| **[!UICONTROL Range]** | Zoeken voorspelt hoe u elementen kunt zoeken die binnen een opgegeven reeks eigenschapswaarden liggen. In het deelvenster Filters kunt u minimum- en maximumeigenschapswaarden voor het bereik opgeven. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Date Range]** | Zoeken voorspelt hoe u elementen die binnen een opgegeven bereik zijn gemaakt, kunt zoeken naar een datumeigenschap. In het deelvenster Filters kunt u begin- en einddatums opgeven. | <ul><li>Veldlabel</li><li>Plaatsaanduiding</li><li>Eigenschapnaam</li><li>Tekst bereik (van)</li><li>Tekst bereik (naar)</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Date]** | Zoeken voorspelt hoe elementen op basis van een schuifregelaar worden doorzocht op basis van een eigenschap date. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL File Size]** | Zoeken voorspelt hoe u elementen kunt zoeken op basis van hun grootte. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Pad</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Asset Last Modified]** | Zoeken voorspelt hoe u elementen kunt zoeken op basis van de laatste gewijzigde datum. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Approval Status]** | Zoeken voorspelt hoe u elementen kunt zoeken op basis van de eigenschap voor metagegevens van goedkeuring. De standaardeigenschapnaam is **dam:status**. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Checkout Status]** | Zoeken voorspelt dat er wordt gezocht naar middelen op basis van de uitcheckstatus van een middel toen het vanuit AEM Assets werd gepubliceerd. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Checked Out By]** | Zoeken voorspelt hoe u elementen kunt zoeken op basis van de gebruiker die het element heeft uitgecheckt. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Expiry Status]** | Zoeken voorspelt dat er op basis van de vervalstatus naar elementen wordt gezocht. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |
| **[!UICONTROL Member of collection]** | Search predicate to search assets based on whether an asset is a part of a collection. | Beschrijving |
| **[!UICONTROL Hidden]** | Dit voorspellen is niet uitdrukkelijk zichtbaar aan het eind - gebruikers en wordt gebruikt voor om het even welke verborgen beperkingen typisch voor het beperken van het type van onderzoeksresultaten tot **dam:Activum**. | <ul><li>Veldlabel</li><li>Eigenschapnaam</li><li>Beschrijving</li></ul> |

>[!NOTE]
>
>Do not use **[!UICONTROL Options Predicate]**, **[!UICONTROL Publish Status Predicate]**, and **[!UICONTROL Rating Predicate]** as these predicates are not functional in Brand Portal.

## Delete a search predicate {#delete-a-search-predicate}

To delete a search predicate, follow these steps:

1. Click the Adobe logo to access administrative tools.

   ![](assets/aemlogo.png)

1. Klik in het deelvenster met beheergereedschappen op **[!UICONTROL Search Forms]**.

   ![](assets/navigation-panel-2.png)

1. Selecteer op de **[!UICONTROL Search Forms]** pagina **[!UICONTROL Assets Admin Search Rail]**.

   ![](assets/search-forms-page.png)

1. Klik op de werkbalk boven in het scherm om het zoekformulier **[!UICONTROL Edit]** te openen.

   ![](assets/edit-search-form-2.png)

1. Selecteer op de [!UICONTROL Edit Search Form] pagina in het hoofdvenster de voorspelling die u wilt verwijderen. For example, select **[!UICONTROL Property Predicate]**.

   Op het **[!UICONTROL Settings]** tabblad rechts worden de eigenschappenvoorspelvelden weergegeven.

1. Als u de voorspelling van de eigenschap wilt verwijderen, klikt u op het binpictogram. Klik in het **[!UICONTROL Delete Field]** dialoogvenster **[!UICONTROL Delete]** om de verwijderactie te bevestigen.

   Het **[!UICONTROL Property Predicate]** veld wordt verwijderd uit het hoofdvenster en het **[!UICONTROL Settings]** tabblad wordt leeg.

   ![](assets/search-form-delete-predicate.png)

1. Klik op de werkbalk om de wijzigingen op te slaan. **[!UICONTROL Done]**
1. Klik in de **[!UICONTROL Assets]** gebruikersinterface op het bedekkingspictogram en kies **[!UICONTROL Filter]** om naar het **[!UICONTROL Filters]** deelvenster te navigeren. De **[!UICONTROL Property]** voorspelling wordt verwijderd uit het deelvenster.

   ![](assets/property-predicate-removed.png)
