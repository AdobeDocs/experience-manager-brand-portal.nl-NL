---
title: Publish-voorinstellingen, -schema en -facetten naar Brand Portal
seo-title: Publish presets, schema, and facets to Brand Portal
description: Leer hoe u voorinstellingen, schema's en facetten naar Brand Portal publiceert.
seo-description: Learn how to publish presets, schema, and facets to Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: 133ea1fc342e4460e7d0661205c7411a509143eb
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 0%

---

# Publish-voorinstellingen, -schema en -facetten naar Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

Het artikel loopt over van AEM Author-instantie naar Brand Portal en bevat voorinstellingen voor afbeeldingen, metagegevensschema&#39;s en aangepaste zoekfacetten. Met de publicatiefunctie kunnen organisaties de voorinstellingen voor afbeeldingen, metagegevensschema&#39;s en zoekfacetten die in AEM instantie Auteur zijn gemaakt/gewijzigd opnieuw gebruiken, waardoor dubbele inspanningen afnemen.

>[!NOTE]
>
>De capaciteit om beeldvoorinstellingen, meta-gegevensschema, en onderzoeksfacetten van AEM instantie van de Auteur aan Brand Portal te publiceren is beschikbaar AEM 6.2 SP1-GVB7 en AEM 6.3 SP1-GFP 1 (6.3.1.1) vanaf.

## Publish-voorinstellingen voor afbeeldingen naar Brand Portal {#publish-image-presets-to-brand-portal}

Voorinstellingen voor afbeeldingen zijn een set opdrachten voor het vergroten of verkleinen en opmaken van de afbeelding die op het moment van de aflevering op de afbeelding worden toegepast. Afbeeldingsvoorinstellingen kunnen in Brand Portal worden gemaakt en gewijzigd. Als AEM instantie Auteur wordt uitgevoerd in de dynamische-mediamodus, kunnen gebruikers ook voorinstellingen maken bij de AEM Auteur en deze publiceren naar AEM Assets Brand Portal, en voorkomen dat ze dezelfde voorinstellingen opnieuw maken in Brand Portal.\
Nadat de voorinstelling is gemaakt, wordt deze weergegeven als dynamische uitvoering op het dialoogvenster voor het weergeven en downloaden van gegevens over elementen.

>[!NOTE]
>
>Als AEM instantie Auteur niet wordt uitgevoerd in **[!UICONTROL Dynamic Media Mode]** (klant heeft Dynamic Media niet aangeschaft), wordt de **[!UICONTROL Pyramid TIFF]** -uitvoering van de elementen niet gemaakt op het moment van het uploaden. Voorinstellingen voor afbeeldingen of dynamische uitvoeringen werken met **[!UICONTROL Pyramid TIFF]** van een element. Als **[!UICONTROL Pyramid TIFF]** niet beschikbaar is voor AEM instantie Auteur, is het dus niet meer beschikbaar voor Brand Portal. Hierdoor zijn er geen dynamische uitvoeringen aanwezig in de renditions rail of asset details page and download dialog.

Voorinstellingen voor afbeeldingen publiceren naar Brand Portal:

1. Tik/klik in AEM instantie Auteur op het AEM logo om de algemene navigatieconsole te openen en tik/klik op het pictogram Extra en navigeer naar **[!UICONTROL Assets > Image Presets]** .
1. Selecteer de voorinstelling voor de afbeelding of meerdere voorinstellingen voor de afbeelding in de lijst met voorinstellingen voor afbeeldingen en klik/tik op **[!UICONTROL Publish to Brand Portal]** .

![](assets/publishpreset.png)

>[!NOTE]
>
>Wanneer gebruikers op **[!UICONTROL Publish to Brand Portal]** klikken, worden de voorinstellingen in de wachtrij voor publicatie geplaatst. De gebruikers worden geadviseerd om het logboek van de replicatieagenten te controleren om te bevestigen of publiceerde succesvol was.

Publicatie van een voorinstelling voor afbeeldingen ongedaan maken vanuit Brand Portal:

1. Tik/klik in AEM instantie Auteur op het AEM logo om de algemene navigatieconsole te openen, klik op het pictogram **[!UICONTROL Tools]** en navigeer naar **[!UICONTROL Assets > Image Presets]** .
1. Selecteer een voorinstelling voor de afbeelding en selecteer **[!UICONTROL Remove from Brand Portal]** uit de opties die bovenaan beschikbaar zijn.

## Publish-metagegevensschema naar Brand Portal  {#publish-metadata-schema-to-brand-portal}

Het schema van meta-gegevens beschrijft de lay-out en de eigenschappen die op de eigenschappen pagina van activa/inzamelingen worden getoond.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Als gebruikers het standaardschema op AEM instantie Auteur hebben uitgegeven en bereid zijn om het zelfde schema zoals standaardschema op Brand Portal te gebruiken, kunnen zij de vormen van het meta-gegevensschema aan Brand Portal eenvoudig publiceren. In een dergelijk scenario wordt het standaardschema in Brand Portal overschreven door de standaardschema&#39;s die zijn gepubliceerd vanuit AEM instantie Auteur.

Als gebruikers een aangepast schema op AEM instantie Auteur hebben gemaakt, kunnen ze het aangepaste schema publiceren naar Brand Portal in plaats van hetzelfde aangepaste schema daar opnieuw te maken. Gebruikers kunnen dit aangepaste schema vervolgens toepassen op elke map of verzameling in Brand Portal.

>[!NOTE]
>
>Standaardschema&#39;s kunnen niet naar de Brand Portal worden gepubliceerd als ze bij het AEM zijn vergrendeld (ze worden dus niet bewerkt).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Als op AEM instantie Auteur een schema is toegepast op een map, moet hetzelfde schema ook op de Brand Portal staan om de consistentie te behouden op de pagina met eigenschappen van elementen op AEM Auteur en Brand Portal.

Een metagegevensschema van AEM instantie Auteur naar Brand Portal publiceren:

1. Tik/klik in AEM instantie Auteur op het AEM logo om de algemene navigatieconsole te openen, klik op het pictogram Gereedschappen en navigeer naar **[!UICONTROL Assets > Metadata Schemas]** .
1. Selecteer een metagegevensschema en selecteer **[!UICONTROL Publish to Brand Portal]** uit de opties die boven beschikbaar zijn.

>[!NOTE]
>
>Wanneer gebruikers op **[!UICONTROL Publish to Brand Portal]** klikken, worden de metagegevensschema&#39;s in de wachtrij voor publicatie geplaatst. De gebruikers worden geadviseerd om het logboek van de replicatieagenten te controleren om te bevestigen of publiceerde succesvol was.

Publicatie van een metagegevensschema vanuit Brand Portal ongedaan maken:

1. Tik/klik in AEM instantie Auteur op het AEM logo om de algemene navigatieconsole te openen, klik op het pictogram Gereedschappen en navigeer naar **[!UICONTROL Assets > Metadata Schemas]** .
1. Selecteer een metagegevensschema en selecteer **[!UICONTROL Remove from Brand Portal]** uit de opties die boven beschikbaar zijn.

## Publish-zoekfacetten naar Brand Portal {#publish-search-facets-to-brand-portal}

De vormen van het onderzoek verstrekken het vermogen van [ beperkt onderzoek ](../using/brand-portal-search-facets.md) aan gebruikers op Brand Portal. Zoeken in facetten geeft zoekopdrachten op Brand Portal meer granulariteit. Alle [ voorspelden toegevoegd ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/search-facets.html) in de onderzoeksvorm zijn beschikbaar aan gebruikers als onderzoeksfacetten in onderzoeksfilters.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Als u een aangepast zoekformulier **[!UICONTROL Assets Admin Search Rail]** wilt gebruiken van AEM instantie Auteur, kunt u het aangepaste zoekformulier publiceren van AEM instantie Auteur naar Brand Portal in plaats van hetzelfde formulier opnieuw te maken op Brand Portal.

>[!NOTE]
>
>Vergrendeld zoekformulier **[!UICONTROL Assets Admin Search Rail]** op AEM Assets kan alleen worden gepubliceerd naar Brand Portal als het wordt bewerkt. Als dit zoekformulier eenmaal is bewerkt en gepubliceerd naar Brand Portal, wordt het zoekformulier op Brand Portal genegeerd.

De bewerkte zoekfacet publiceren van AEM instantie Auteur naar Brand Portal:

1. Klik op het AEM en ga naar **[!UICONTROL Tools > General > Search Forms]** .
1. Selecteer het bewerkte zoekformulier en selecteer **[!UICONTROL Publish to Brand Portal]** .

   >[!NOTE]
   >
   >Wanneer gebruikers op **[!UICONTROL Publish to Brand Portal]** klikken, worden de zoekfacetten in de wachtrij voor publicatie geplaatst. De gebruikers worden geadviseerd om het logboek van de replicatieagenten te controleren om te bevestigen of publiceerde succesvol was.

U kunt als volgt zoekformulieren verwijderen uit Brand Portal:

1. Tik/klik in AEM instantie Auteur op het AEM logo om de algemene navigatieconsole te openen, klik op het pictogram Gereedschappen en navigeer naar **[!UICONTROL General > Search Forms]** .
1. Selecteer het zoekformulier en selecteer **[!UICONTROL Remove from Brand Portal]** uit de opties die boven aan het scherm beschikbaar zijn.

>[!NOTE]
>
>Met de handeling **[!UICONTROL Unpublish from Brand Portal]** blijft het standaardzoekformulier in Brand Portal en wordt het laatst gebruikte zoekformulier niet hersteld voordat het wordt gepubliceerd.

### Beperkingen {#limitations}

1. Weinig zoekvoorspellen zijn niet van toepassing op zoekfilters op de Brand Portal. Wanneer deze zoekvoorspelling wordt gepubliceerd als onderdeel van het zoekformulier van AEM instantie Auteur naar Brand Portal, worden ze uitgefilterd. Gebruikers zien daarom minder voorspellingen in de gepubliceerde vorm op de Brand Portal. Zie [ onderzoek voorspelt toepasselijk op filters op Brand Portal ](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. Als een gebruiker bijvoorbeeld [!UICONTROL Options Predicate] een aangepast pad gebruikt om opties te lezen bij AEM instantie Auteur, werkt dit niet bij de Brand Portal. Deze extra paden en opties worden niet met het zoekformulier naar Brand Portal gepubliceerd. In dit geval kunnen gebruikers de optie **[!UICONTROL Manual]** in **[!UICONTROL Add Options]** within **[!UICONTROL Options Predicate]** selecteren om deze opties handmatig in Brand Portal toe te voegen.

![](assets/options-predicate-manual.png)
