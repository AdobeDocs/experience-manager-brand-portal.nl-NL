---
title: Door elementen bladeren op Brand Portal
seo-title: Door elementen bladeren op Brand Portal
description: Blader door elementen, de hiërarchieën van doorlopende elementen en zoekelementen met behulp van verschillende weergaveopties en UI-elementen op Brand Portal.
seo-description: Blader door elementen, de hiërarchieën van doorlopende elementen en zoekelementen met behulp van verschillende weergaveopties en UI-elementen op Brand Portal.
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
translation-type: tm+mt
source-git-commit: ca60fe1b76c6e99d835457627fcc4bf402b6bd87
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 1%

---


# Door elementen bladeren op Brand Portal {#browsing-assets-on-brand-portal}

AEM Assets Brand Portal biedt verschillende mogelijkheden en gebruikersinterface-elementen die het bladeren door bronnen, het doorlopen van middelenhiërarchieën en het zoeken naar elementen vereenvoudigen terwijl u verschillende weergaveopties gebruikt.

AEM logo in de AEM werkbalk boven in het scherm geeft beheerders toegang tot het deelvenster met beheergereedschappen.

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)<br />

De kiezer voor het spoor linksboven in Brand Portal zet de keuzelijst neer om opties beschikbaar te maken waarmee u in de hiërarchieën van middelen kunt navigeren, uw zoekopdracht kunt stroomlijnen en bronnen kunt weergeven.

![](assets/siderail-1.png)

U kunt elementen weergeven, doorbladeren en selecteren met een van de beschikbare weergaven (Kaart, Kolom en Lijst) in de weergavekiezer in de rechterbovenhoek in Brand Portal.

![](assets/viewselector.png)

## Bronnen weergeven en selecteren {#viewing-and-selecting-resources}

Het bekijken, navigeren, en het selecteren van elk zijn conceptueel het zelfde over alle meningen, maar hebben kleine variaties in behandeling, afhankelijk van de mening u gebruikt.

U kunt de bronnen weergeven, doorbladeren en selecteren (voor verdere actie) met een van de beschikbare weergaven:

* Kolomweergave
* Kaartweergave
* Lijstweergave

### Kaartweergave

![](assets/card-view.png)

In de kaartweergave worden voor elk item op het huidige niveau informatiekaarten weergegeven. Deze kaarten bevatten de volgende gegevens:

* Een visuele weergave van het element/de map.
* Type
* Titel
* Naam
* Datum en tijdstip waarop de middelen van AEM naar Brand Portal zijn gepubliceerd
* Grootte
* Dimensies

U kunt de hiërarchie omlaag navigeren door op de kaart te tikken of erop te klikken (zorg dat u de snelle handelingen voorkomt) of door de [broodkruimels in de koptekst](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader)weer te gebruiken.

![](assets/cardquickactions.png)

#### Kaartweergave voor gebruikers die geen beheerder zijn

Kaarten van mappen geven in de Kaartweergave hiërarchiegegevens weer aan gebruikers die geen beheerder zijn (Editor, Viewer en gastgebruiker). Deze functionaliteit laat de gebruikers de plaats van de omslagen kennen, die zij, met betrekking tot de ouderhiërarchie toegang hebben.
Informatie over de maphiërarchie is vooral handig om onderscheid te maken tussen de mappen waarvan de namen overeenkomen met andere mappen die vanuit een andere maphiërarchie worden gedeeld. Als de gebruikers die geen beheerder zijn niet op de hoogte zijn van de mapstructuur van de elementen die met hen worden gedeeld, lijken elementen/mappen met vergelijkbare namen verwarrend.

* De paden die op de betreffende kaarten worden weergegeven, worden afgekapt om in de kaartgrootten te passen. Gebruikers kunnen het volledige pad echter zien als knopinfo bij het aanwijzen over het afgebroken pad.

![](assets/folder-hierarchy1.png)

**Overzicht, optie om de eigenschappen van elementen weer te geven**

De optie Overzicht is beschikbaar voor gebruikers die geen beheerder zijn (Editors, Viewers, Gastgebruikers) en geeft de eigenschappen van middelen van geselecteerde elementen/mappen weer. De optie Overzicht is zichtbaar:

* in de werkbalk bovenaan bij het selecteren van een middel/map.
* in de vervolgkeuzelijst betreffende de selectie van de spoorstaafkiezer.

Als gebruikers de **[!UICONTROL Overview]** optie selecteren terwijl een element/map is geselecteerd, kunnen ze de titel, het pad en het tijdstip van het maken van het element zien. Terwijl de gebruiker met de optie Overzicht op de pagina met elementdetails de metagegevens van het element kan bekijken.

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### Instellingen weergeven in de kaartweergave

**[!UICONTROL View Settings]** wordt geopend bij het selecteren **[!UICONTROL View Settings]** vanuit de weergavekiezer. Hiermee kunt u de grootte van de elementminiaturen in de kaartweergave wijzigen. Op deze manier kunt u de weergave aanpassen en het aantal weergegeven miniaturen bepalen.

![](assets/cardviewsettings.png)

### Lijstweergave

![](assets/list-view.png)

De lijstmening toont informatie voor elk middel op het huidige niveau. De lijstweergave bevat de volgende details:

* Miniatuurafbeelding van elementen
* Naam
* Titel
* Landinstelling
* Type
* Dimension
* Grootte
* Classificatie
* Mappad met middelenhiërarchie<sup>*</sup>
* Datum van publicatie van het middel op de Brand Portal

Met de padkolom kunt u de middelenlocatie in de mappenhiërarchie gemakkelijk herkennen. U kunt de hiërarchie omlaag navigeren door op de naam van de bron te tikken of erop te klikken en door een back-up te maken met de [broodkruimels in de koptekst](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### Instellingen weergeven in de lijstweergave

In de lijstweergave wordt **[!UICONTROL Name]** standaard de eerste kolom weergegeven. De extra informatie, zoals activa **[!UICONTROL Title]**, **[!UICONTROL Locale]**, **[!UICONTROL Type]**, **[!UICONTROL Dimensions]**, **[!UICONTROL Size]**, **[!UICONTROL Rating]**, wordt ook getoond. U kunt echter wel de kolommen selecteren die u wilt weergeven **[!UICONTROL View Settings]**.

![](assets/list-view-setting.png)

### Kolomweergave

![](assets/column-view.png)

Met de kolomweergave kunt u door een inhoudsstructuur navigeren door een reeks trapsgewijze kolommen. In deze weergave kunt u de hiërarchie van elementen visualiseren en doorlopen.

Als u een bron selecteert in de eerste (meest linkse) kolom, worden onderliggende bronnen weergegeven in de tweede kolom rechts. Als u een bron in de tweede kolom selecteert, worden onderliggende bronnen in de derde kolom rechts weergegeven, enzovoort.

U kunt omhoog en omlaag navigeren in de boom door op de middelnaam of de chevron rechts van de middelnaam te tikken of te klikken.

* De naam en het chevron van de bron worden benadrukt wanneer getikt of geklikt.
* Als u op de miniatuur tikt of erop klikt, wordt de bron geselecteerd.
* Als deze optie is geselecteerd, wordt een vinkje boven de miniatuur geplaatst en wordt de naam van de bron gemarkeerd.
* De details van de geselecteerde bron worden getoond in de definitieve kolom.

Wanneer een element is geselecteerd in de kolomweergave, wordt de visuele weergave van het element weergegeven in de laatste kolom, samen met de volgende details:

* Titel
* Naam
* Dimensies
* Datum en tijdstip waarop de middelen van AEM naar Brand Portal zijn gepubliceerd
* Grootte
* Type
* Meer informatie, optie om op de detailpagina van het element te gaan

<!--
Comment Type: draft

<h3>Selecting Resources</h3>
-->

<!--
Comment Type: draft

<p>Selecting a specific resource depends on a combination of the view and the device:</p>
-->

<!--
Comment Type: draft

<table border="1" cellpadding="1" cellspacing="0" width="100%">
<tbody>
<tr>
<td> </td>
<td>Select</td>
<td>Deselect</td>
</tr>
<tr>
<td>Column View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
<tr>
<td>Card View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap-and-hold the card</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the card</li>
<li>Mobile device:<br /> Tap the card</li>
</ul> </td>
</tr>
<tr>
<td>List View</td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
</tbody>
</table>
-->

<!--
Comment Type: draft

Deselecting All
-->

<!--
Comment Type: draft

<p>In all cases, as you select items the count of the items selected is displayed at the upper right of the toolbar.</p>
<p>You can deselect all items and exit selection mode by clicking or tapping the X next to the count.</p>
-->

<!--
Comment Type: draft

<p>In all views, all items can be deselected by tapping escape on the keyboard if you are using a desktop device.</p>
-->

## Inhoudsstructuur {#content-tree}

Naast deze weergaven gebruikt u de structuurweergave om de hiërarchie van elementen omlaag te doorlopen terwijl u de gewenste elementen of mappen weergeeft en selecteert.

Als u de structuurweergave wilt openen, tikt u op de railkiezer linksboven en selecteert u deze in het **[!UICONTROL Content tree]** menu.

![](assets/contenttree.png)

Navigeer vanuit de inhoudshiërarchie naar het gewenste element.

![](assets/content-tree.png)

## Details van element {#asset-details}

Met de pagina met elementdetails kunt u een element weergeven, downloaden, de koppeling met middelen delen, naar een verzameling verplaatsen of de eigenschappenpagina van het element weergeven. Hiermee kunt u ook door de detailpagina van andere elementen in dezelfde map navigeren.

![](assets/asset-detail.png)

Als u de metagegevens van het element wilt weergeven of de verschillende uitvoeringen wilt bekijken, gebruikt u de railkiezer op de pagina met de elementdetails.

![](assets/asset-overview.png)

U kunt alle beschikbare uitvoeringen van het element weergeven op de pagina met elementdetails en een vertoning selecteren om deze voor te vertonen.

![](assets/renditions.png)

Als u de pagina met eigenschappen van elementen wilt openen, gebruikt u de **[!UICONTROL Properties (p)]** optie in de bovenste balk.

![](assets/asset-properties.png)

U kunt ook een lijst weergeven met alle gerelateerde elementen (bron of afgeleide elementen op AEM) op de eigenschappenpagina van een element, aangezien de elementrelatie ook wordt gepubliceerd van AEM naar Brand Portal.
