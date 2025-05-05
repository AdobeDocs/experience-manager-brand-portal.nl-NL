---
title: Publish-voorinstellingen, -schema en -facetten naar Brand Portal
description: Leer hoe u voorinstellingen, schema's en facetten naar Brand Portal publiceert.
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: 4d9d7afa2cd45ea68c2e15338c92aa29ecf09f91
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---

# Publish-voorinstellingen, -schema en -facetten naar Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

Het artikel loopt over van AEM Author-instantie naar Brand Portal en bevat voorinstellingen voor afbeeldingen, metagegevensschema&#39;s en aangepaste zoekfacetten. Met de publicatiefunctie kunnen organisaties de voorinstellingen voor afbeeldingen, metagegevensschema&#39;s en zoekfacetten die zijn gemaakt of bewerkt op een AEM Auteur-instantie, opnieuw gebruiken. Deze aanpak vermindert dubbele inspanningen.

>[!NOTE]
>
>De capaciteit om beeldvoorinstellingen, meta-gegevensschema, en onderzoeksfacetten van AEM instantie van de Auteur aan Brand Portal te publiceren is beschikbaar van AEM 6.2 SP1-GVB7 en AEM 6.3 SP1-GFP 1 (6.3.1.1) vanaf.

## Publish-voorinstellingen voor afbeeldingen naar Brand Portal {#publish-image-presets-to-brand-portal}

Voorinstellingen voor afbeeldingen zijn een set opdrachten voor het vergroten of verkleinen en opmaken van de afbeelding die op het moment van de aflevering op de afbeelding worden toegepast. Afbeeldingsvoorinstellingen kunnen in Brand Portal worden gemaakt en gewijzigd. Als in de Dynamic Media-modus een AEM-instantie Auteur wordt uitgevoerd, kunnen gebruikers ook voorinstellingen maken in AEM Auteur en deze publiceren naar AEM Assets Brand Portal. Op deze manier voorkomt u dat dezelfde voorinstellingen opnieuw worden gemaakt in Brand Portal.
Nadat de voorinstelling is gemaakt, wordt deze weergegeven als een dynamische uitvoering in het dialoogvenster voor het weergeven en downloaden van gegevens over elementen.

>[!NOTE]
>
>Als de AEM Author-instantie niet wordt uitgevoerd in **[!UICONTROL Dynamic Media Mode]** (de klant heeft Dynamic Media niet aangeschaft), wordt de **[!UICONTROL Pyramid TIFF]** -uitvoering van de elementen niet gemaakt op het moment van het uploaden. Voorinstellingen voor afbeeldingen of dynamische uitvoeringen werken met **[!UICONTROL Pyramid TIFF]** van een element. Als **[!UICONTROL Pyramid TIFF]** dus niet beschikbaar is voor AEM instantie Auteur, is deze niet beschikbaar voor Brand Portal. Als gevolg hiervan zijn er geen dynamische uitvoeringen aanwezig in de renditions rail van de pagina met elementdetails en het dialoogvenster Downloaden.

Voorinstellingen voor afbeeldingen publiceren naar Brand Portal:

1. Klik in AEM instantie Auteur op het AEM logo om de algemene navigatieconsole te openen, klik op het pictogram Gereedschappen en navigeer naar **[!UICONTROL Assets > Image Presets]** .
1. Selecteer de voorinstelling voor de afbeelding of meerdere voorinstellingen voor de afbeelding in de lijst met voorinstellingen voor afbeeldingen en klik op **[!UICONTROL Publish to Brand Portal]** .

![](assets/publishpreset.png)

>[!NOTE]
>
>Wanneer gebruikers op **[!UICONTROL Publish to Brand Portal]** klikken, worden de voorinstellingen van de afbeelding in de wachtrij voor publicatie geplaatst. De gebruikers worden geadviseerd om het logboek van de replicatieagenten te controleren om te bevestigen of publiceerde succesvol was.

Publicatie van een voorinstelling voor afbeeldingen ongedaan maken vanuit Brand Portal:

1. Klik in AEM instantie Auteur op het AEM logo om de algemene navigatieconsole te openen, klik op het pictogram **[!UICONTROL Tools]** en navigeer naar **[!UICONTROL Assets > Image Presets]** .
1. Selecteer een voorinstelling voor de afbeelding en selecteer **[!UICONTROL Remove from Brand Portal]** uit de opties die bovenaan beschikbaar zijn.

## Publish-metagegevensschema naar Brand Portal {#publish-metadata-schema-to-brand-portal}

Het schema van meta-gegevens beschrijft de lay-out en de eigenschappen die op de eigenschappen pagina van activa/inzamelingen worden getoond.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Als gebruikers het standaardschema op een AEM Author-instantie hebben bewerkt en ze hetzelfde schema als het standaardschema op de Brand Portal willen gebruiken, publiceert u de schema-metagegevensformulieren naar Brand Portal. In zo&#39;n scenario, treden de standaardschema&#39;s die van de AEM instantie van de Auteur worden gepubliceerd het standaardschema in Brand Portal met voeten.

Als gebruikers een aangepast schema op AEM instantie Auteur hebben gemaakt, kunnen ze het aangepaste schema publiceren naar Brand Portal in plaats van hetzelfde aangepaste schema daar opnieuw te maken. Gebruikers kunnen dit aangepaste schema vervolgens toepassen op elke map of verzameling in Brand Portal.

>[!NOTE]
>
>Standaardschema&#39;s kunnen niet naar de Brand Portal worden gepubliceerd als ze op het AEM zijn vergrendeld. Ze worden dus niet bewerkt.

![](assets/default-schema-form.png)

>[!NOTE]
>
>Als op AEM instantie Auteur een schema is toegepast op een map, moet hetzelfde schema ook op de Brand Portal staan. Hierdoor blijft de consistentie behouden op de pagina met eigenschappen van elementen op AEM Auteur en Brand Portal.

Een metagegevensschema van AEM instantie Auteur naar Brand Portal publiceren:

1. Klik in AEM instantie Auteur op het AEM logo om de algemene navigatieconsole te openen, klik op het pictogram Gereedschappen en navigeer naar **[!UICONTROL Assets > Metadata Schemas]** .
1. Selecteer een metagegevensschema en selecteer **[!UICONTROL Publish to Brand Portal]** uit de opties die boven beschikbaar zijn.

>[!NOTE]
>
>Wanneer gebruikers op **[!UICONTROL Publish to Brand Portal]** klikken, worden de metagegevensschema&#39;s in de wachtrij voor publicatie geplaatst. De gebruikers worden geadviseerd om het logboek van de replicatieagenten te controleren om te bevestigen of publiceerde succesvol was.

Publicatie van een metagegevensschema vanuit Brand Portal ongedaan maken:

1. Klik in AEM instantie Auteur op het AEM logo om de algemene navigatieconsole te openen, klik op het pictogram Gereedschappen en navigeer naar **[!UICONTROL Assets > Metadata Schemas]** .
1. Selecteer een metagegevensschema en selecteer **[!UICONTROL Remove from Brand Portal]** uit de opties die boven beschikbaar zijn.

## Publish-zoekfacetten naar Brand Portal {#publish-search-facets-to-brand-portal}

De vormen van het onderzoek verstrekken het vermogen van [ beperkt onderzoek ](../using/brand-portal-search-facets.md) aan gebruikers op Brand Portal. Zoeken in facetten geeft zoekopdrachten op Brand Portal meer granulariteit. Alle [ voorspelden toegevoegd ](https://experienceleague.adobe.com/nl/docs/experience-manager-65/content/assets/administer/search-facets) in de onderzoeksvorm zijn beschikbaar aan gebruikers als onderzoeksfacetten in onderzoeksfilters.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Als u een aangepast zoekformulier wilt gebruiken op **[!UICONTROL Assets Admin Search Rail]** van AEM instantie Auteur, publiceert u het rechtstreeks naar Brand Portal in plaats van het opnieuw te maken.

>[!NOTE]
>
>Als u een vergrendeld zoekformulier wilt publiceren op **[!UICONTROL Assets Admin Search Rail]** van AEM Assets naar Brand Portal, moet u het eerst bewerken. Als dit zoekformulier eenmaal is bewerkt en gepubliceerd, wordt het bestaande zoekformulier op Brand Portal genegeerd.

De bewerkte zoekfacet publiceren van AEM instantie Auteur naar Brand Portal:

1. Klik op het AEM en ga naar **[!UICONTROL Tools > General > Search Forms]** .
1. Selecteer het bewerkte zoekformulier en selecteer **[!UICONTROL Publish to Brand Portal]** .

   >[!NOTE]
   >
   >Wanneer gebruikers op **[!UICONTROL Publish to Brand Portal]** klikken, worden de zoekfacetten in de wachtrij voor publicatie geplaatst. De gebruikers worden geadviseerd om het logboek van de replicatieagenten te controleren om te bevestigen of publiceerde succesvol was.

U kunt als volgt zoekformulieren verwijderen uit Brand Portal:

1. Klik in AEM instantie Auteur op het AEM logo om de algemene navigatieconsole te openen, klik op het pictogram Gereedschappen en navigeer naar **[!UICONTROL General > Search Forms]** .
1. Selecteer het zoekformulier en selecteer **[!UICONTROL Remove from Brand Portal]** uit de opties die boven aan het scherm beschikbaar zijn.

>[!NOTE]
>
>Met de handeling **[!UICONTROL Unpublish from Brand Portal]** blijft het standaardzoekformulier in Brand Portal en wordt het laatst gebruikte zoekformulier niet hersteld voordat het wordt gepubliceerd.

### Beperkingen {#limitations}

1. Weinig zoekvoorspellen zijn niet van toepassing op zoekfilters op de Brand Portal. Wanneer deze zoekvoorspelling wordt gepubliceerd als onderdeel van het zoekformulier van AEM instantie Auteur naar Brand Portal, worden ze uitgefilterd. Gebruikers zien daarom minder voorspellingen in de gepubliceerde vorm op de Brand Portal. Zie [ onderzoek voorspelt toepasselijk op filters op Brand Portal ](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. Als een gebruiker bijvoorbeeld [!UICONTROL Options Predicate] een aangepast pad gebruikt om opties te lezen voor een AEM instantie Auteur, werkt dit niet voor Brand Portal. Deze extra paden en opties worden niet met het zoekformulier naar Brand Portal gepubliceerd. In dit geval kunnen gebruikers de optie **[!UICONTROL Manual]** in **[!UICONTROL Add Options]** within **[!UICONTROL Options Predicate]** selecteren om deze opties handmatig in Brand Portal toe te voegen.

![](assets/options-predicate-manual.png)
