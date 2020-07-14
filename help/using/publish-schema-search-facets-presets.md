---
title: Voorinstellingen, schema en facetten publiceren naar Brand Portal
seo-title: Voorinstellingen, schema en facetten publiceren naar Brand Portal
description: Leer hoe u voorinstellingen, schema's en facetten naar Brand Portal publiceert.
seo-description: Leer hoe u voorinstellingen, schema's en facetten naar Brand Portal publiceert.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---


# Publish presets, schema, and facets to Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

Het artikel loopt over van AEM Author-instantie naar Brand Portal en publiceert voorinstellingen voor afbeeldingen, metagegevensschema&#39;s en aangepaste zoekfacetten. Met de publicatiefunctie kunnen organisaties de voorinstellingen voor afbeeldingen, metagegevensschema&#39;s en zoekfacetten die in een AEM Author-instantie zijn gemaakt/gewijzigd, opnieuw gebruiken, waardoor dubbele inspanningen afnemen.

>[!NOTE]
>
>De capaciteit om beeldvoorinstellingen, meta-gegevensschema, en onderzoeksfacetten van AEM Author instantie aan het Portaal van het Merk te publiceren is beschikbaar AEM 6.2 SP1-GVB7 en AEM 6.3 SP 1-GFP 1 (6.3.1.1) vanaf.

## Voorinstellingen voor afbeeldingen publiceren naar Brand Portal {#publish-image-presets-to-brand-portal}

Voorinstellingen voor afbeeldingen zijn een set opdrachten voor het vergroten of verkleinen en opmaken van de afbeelding die op het moment van de aflevering op de afbeelding worden toegepast. Afbeeldingsvoorinstellingen kunnen worden gemaakt en gewijzigd op Brand Portal. Als de AEM Author-instantie in de dynamische mediamodus wordt uitgevoerd, kunnen gebruikers ook voorinstellingen op de AEM Author maken en deze publiceren naar het Brand Portal van de AEM Assets. Zo voorkomt u dat dezelfde voorinstellingen op het Brand Portal opnieuw worden gemaakt.\
Nadat de voorinstelling is gemaakt, wordt deze weergegeven als dynamische uitvoering op het dialoogvenster voor het weergeven en downloaden van gegevens over elementen.

>[!NOTE]
>
>Als de AEM Author-instantie niet wordt uitgevoerd **[!UICONTROL Dynamic Media Mode]** (klant heeft geen Dynamic Media aangeschaft), wordt de **[!UICONTROL Pyramid TIFF]** uitvoering van de elementen niet gemaakt op het moment van uploaden. Voorinstellingen voor afbeeldingen of dynamische uitvoeringen werken op **[!UICONTROL Pyramid TIFF]** een element. Als dit niet **[!UICONTROL Pyramid TIFF]** het geval is voor een AEM Author-instantie, is het dus niet meer beschikbaar op Brand Portal. Hierdoor zijn er geen dynamische uitvoeringen aanwezig in de renditions rail of asset details page and download dialog.

Voorinstellingen voor afbeeldingen publiceren naar Brand Portal:

1. Tik/klik in AEM Author-instantie op het AEM-logo om de algemene navigatieconsole te openen en tik/klik op het pictogram Extra en navigeer naar **[!UICONTROL Assets > Image Presets]**.
1. Selecteer de voorinstelling voor de afbeelding of meerdere voorinstellingen voor de afbeelding in de lijst met voorinstellingen voor de afbeelding en klik/tik **[!UICONTROL Publish to Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Wanneer gebruikers op **[!UICONTROL Publish to Brand Portal]** de voorinstellingen voor afbeeldingen klikken, worden deze in de wachtrij voor publicatie geplaatst. De gebruikers worden geadviseerd om het logboek van de replicatieagenten te controleren om te bevestigen of publiceerde succesvol was.

Publicatie van een voorinstelling voor afbeeldingen via Brand Portal ongedaan maken:

1. Tik/klik in AEM Author-instantie op het AEM-logo om de algemene navigatieconsole te openen en tik/klik op het **[!UICONTROL Tools]** pictogram en navigeer naar **[!UICONTROL Assets > Image Presets]**.
1. Selecteer een voorinstelling voor de afbeelding en selecteer de opties **[!UICONTROL Remove from Brand Portal]** die bovenaan beschikbaar zijn.

## Metagegevensschema publiceren naar Brand Portal  {#publish-metadata-schema-to-brand-portal}

Het schema van meta-gegevens beschrijft de lay-out en de eigenschappen die op de eigenschappen pagina van activa/inzamelingen worden getoond.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Als de gebruikers het standaardschema op instantie van AEM Author hebben uitgegeven en bereid zijn om het zelfde schema zoals standaardschema op het Portaal van het Merk te gebruiken, kunnen zij de vormen van het meta-gegevensschema aan het Portaal van het Merk eenvoudig publiceren. In een dergelijk scenario, wordt het standaardschema bij het Portaal van het Merk overschreven door de standaardschema&#39;s die van de instantie van AEM Author worden gepubliceerd.

Als gebruikers een aangepast schema op een AEM Author-instantie hebben gemaakt, kunnen ze het aangepaste schema publiceren naar Brand Portal in plaats van hetzelfde aangepaste schema daar opnieuw te maken. De gebruikers kunnen dit douaneschema op om het even welke omslag/inzameling in het Portaal van het Merk dan toepassen.

>[!NOTE]
>
>De standaardschema&#39;s kunnen niet aan het Portaal van het Merk worden gepubliceerd als zij bij de instantie AEM (namelijk worden zij niet uitgegeven) worden gesloten.

![](assets/default-schema-form.png)

>[!NOTE]
>
>Als op een map een schema is toegepast op een AEM Author-instantie, moet op het Brand Portal hetzelfde schema staan om de consistentie van de pagina met eigenschappen van de elementen op de pagina AEM Author en Brand Portal te behouden.

Een metagegevensschema publiceren van een AEM Author-instantie naar een Brand Portal:

1. Tik/klik in AEM Author-instantie op het AEM-logo om de algemene navigatieconsole te openen en tik/klik op het pictogram Extra en navigeer naar **[!UICONTROL Assets > Metadata Schemas]**.
1. Selecteer een metagegevensschema en selecteer de opties **[!UICONTROL Publish to Brand Portal]** die bovenaan beschikbaar zijn.

>[!NOTE]
>
>Wanneer de gebruikers klikken **[!UICONTROL Publish to Brand Portal]**, worden de meta-gegevensschema&#39;s een rij gevormd voor publicatie. De gebruikers worden geadviseerd om het logboek van de replicatieagenten te controleren om te bevestigen of publiceerde succesvol was.

Publicatie van een metagegevensschema via Brand Portal ongedaan maken:

1. Tik/klik in AEM Author-instantie op het AEM-logo om de algemene navigatieconsole te openen en tik/klik op het pictogram Extra en navigeer naar **[!UICONTROL Assets > Metadata Schemas]**.
1. Selecteer een metagegevensschema en selecteer de opties **[!UICONTROL Remove from Brand Portal]** die bovenaan beschikbaar zijn.

## Zoekfacetten publiceren naar Brand Portal {#publish-search-facets-to-brand-portal}

Met zoekformulieren kunt u [gemakkelijk op Brand Portal zoeken](../using/brand-portal-search-facets.md) . Zoeken in facetten geeft meer granulariteit bij zoekopdrachten op Brand Portal. Alle [voorvertoningen die in het zoekformulier zijn toegevoegd](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) , zijn beschikbaar voor gebruikers als zoekfactoren in zoekfilters.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Als u een aangepast zoekformulier wilt gebruiken **[!UICONTROL Assets Admin Search Rail]** van AEM Author-instantie, kunt u het aangepaste zoekformulier publiceren van AEM Author-exemplaar naar Brand Portal in plaats van hetzelfde formulier opnieuw te maken op Brand Portal.

>[!NOTE]
>
>Vergrendeld zoekformulier **[!UICONTROL Assets Admin Search Rail]** op AEM Assets kan alleen worden gepubliceerd naar Brand Portal als het wordt bewerkt. Als dit zoekformulier eenmaal is bewerkt en gepubliceerd naar Brand Portal, wordt het zoekformulier op Brand Portal genegeerd.

De bewerkte zoekfacet publiceren van een AEM Author-exemplaar naar een Brand Portal:

1. Tik of klik op het AEM-logo en ga naar **[!UICONTROL Tools > General > Search Forms]**.
1. Selecteer het bewerkte zoekformulier en selecteer **[!UICONTROL Publish to Brand Portal]**.

   >[!NOTE]
   >
   >Wanneer de gebruikers klikken **[!UICONTROL Publish to Brand Portal]**, worden de onderzoeksfacetten een rij gevormd voor publicatie. De gebruikers worden geadviseerd om het logboek van de replicatieagenten te controleren om te bevestigen of publiceerde succesvol was.

U kunt als volgt zoekformulieren niet publiceren vanaf Brand Portal:

1. Tik/klik in AEM Author-instantie op het AEM-logo om de algemene navigatieconsole te openen en tik/klik op het pictogram Extra en navigeer naar **[!UICONTROL General > Search Forms]**.
1. Selecteer het zoekformulier en selecteer de opties **[!UICONTROL Remove from Brand Portal]** die bovenaan beschikbaar zijn.

>[!NOTE]
>
>De **[!UICONTROL Unpublish from Brand Portal]** actie verlaat het standaardonderzoeksformulier op het Portaal van het Merk, en herstelt niet aan het laatste onderzoeksformulier dat alvorens te publiceren wordt gebruikt.

### Beperkingen {#limitations}

1. Weinig zoekvoorspellen zijn niet van toepassing op zoekfilters op de Brand Portal. Wanneer deze zoekvoorspellen worden gepubliceerd als onderdeel van het zoekformulier van AEM Author-exemplaar naar Brand Portal, worden ze uitgefilterd. Gebruikers zien daarom minder voorspellingen in de gepubliceerde vorm op het Brand Portal. Zie [zoekvoorspelling die van toepassing is op filters op Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. Bijvoorbeeld, als een gebruiker om het even welk douanepad gebruikt om opties bij instantie van AEM Author te lezen, zal het niet bij de Poort van het Merk werken. [!UICONTROL Options Predicate] Deze extra paden en opties worden niet met het zoekformulier naar Brand Portal gepubliceerd. In dit geval kunnen gebruikers de **[!UICONTROL Manual]** optie in **[!UICONTROL Add Options]** de toepassing selecteren om deze opties handmatig bij Brand Portal toe **[!UICONTROL Options Predicate]** te voegen.

![](assets/options-predicate-manual.png)
