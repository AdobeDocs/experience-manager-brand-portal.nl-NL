---
title: Het metagegevensschema gebruiken
seo-title: Het metagegevensschema gebruiken
description: Een meta-gegevensschema beschrijft de lay-out van de pagina van Eigenschappen en de meta-gegevenseigenschappen die voor activa worden getoond die het bepaalde schema gebruiken. Het schema dat u op een element toepast, bepaalt de metagegevensvelden die op de eigenschappenpagina worden weergegeven.
seo-description: Een meta-gegevensschema beschrijft de lay-out van de pagina van Eigenschappen en de meta-gegevenseigenschappen die voor activa worden getoond die het bepaalde schema gebruiken. Het schema dat u op een element toepast, bepaalt de metagegevensvelden die op de eigenschappenpagina worden weergegeven.
uuid: 1a944a3b-5152-425f-b1ea-bfe3331de928
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 500b46da-ef67-46a0-a069-192f4b1a0eca
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Het metagegevensschema gebruiken {#use-the-metadata-schema-form}

Een meta-gegevensschema beschrijft de lay-out van de pagina van Eigenschappen en de meta-gegevenseigenschappen die voor activa worden getoond die het bepaalde schema gebruiken. Het schema dat u op een element toepast, bepaalt de metagegevensvelden die op de eigenschappenpagina worden weergegeven.

De **[!UICONTROL Properties]** pagina voor elk element bevat standaardeigenschappen voor metagegevens, afhankelijk van het MIME-type van het element. Beheerders kunnen de Editor metagegevensschema&#39;s gebruiken om bestaande schema&#39;s te wijzigen of aangepaste metagegevensschema&#39;s toe te voegen. AEM Assets Brand Portal biedt standaardformulieren voor elementen van verschillende MIME-typen. U kunt echter ook aangepaste formulieren voor dergelijke elementen toevoegen.

## Een metagegevensschema toevoegen {#add-a-metadata-schema-form}

Ga als volgt te werk om een nieuw schema voor metagegevens te maken:

1. Klik op de AEM-werkbalk boven in het scherm op het Adobe-logo voor toegang tot beheergereedschappen.

   ![](assets/aemlogo.png)

1. Klik in het deelvenster met beheergereedschappen op **[!UICONTROL Metadata Schemas]**.

   ![](assets/navigation-panel.png)

1. Klik op de **[!UICONTROL Metadata Schema Forms]** pagina **[!UICONTROL Create]**.

   ![](assets/create-metadata-schema-form.png)

1. Geef in het **[!UICONTROL Create Schema Form]** dialoogvenster de titel van het schema-formulier op en klik vervolgens **[!UICONTROL Create]** om het maken van het formulier te voltooien.

   ![](assets/create-schema-form.png)

## Een formulier voor een metagegevensschema bewerken {#edit-a-metadata-schema-form}

U kunt een nieuw toegevoegd of bestaand schema voor metagegevens bewerken. Het metagegevensschema bevat inhoud die is afgeleid van het bovenliggende element, inclusief tabbladen en formulieritems binnen tabbladen. U kunt deze formulieritems toewijzen aan of configureren naar een veld binnen een metagegevensknooppunt.

U kunt nieuwe tabbladen of formulieritems toevoegen aan het metagegevensschemaformulier. De afgeleide tabbladen en formulieritems (van het bovenliggende element) bevinden zich in de vergrendelde status. U kunt deze niet wijzigen op het niveau van het kind.

Ga als volgt te werk om een metagegevensschemaformulier te bewerken:

1. Klik op de AEM-werkbalk boven in het scherm op het Adobe-logo voor toegang tot beheergereedschappen.

   ![](assets/aemlogo.png)

1. Klik in het deelvenster met beheergereedschappen op **[!UICONTROL Metadata Schemas]**.
1. Selecteer op de **[!UICONTROL Metadata Schema Forms]** pagina een schema om bijvoorbeeld de eigenschappen ervan te bewerken **[!UICONTROL collection]**.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >Onbewerkte sjablonen geven vóór de sjablonen een vergrendelingssymbool weer. Als u een van de sjablonen aanpast, verdwijnt het symbool Vergrendelen voordat de sjabloon verdwijnt.

1. Klik op de werkbalk boven in het scherm **[!UICONTROL Edit]**.

   De **[!UICONTROL Metadata Schema Editor]** pagina wordt geopend met links het **[!UICONTROL Basic]** tabblad en rechts het **[!UICONTROL Build Form]** tabblad.

1. In the **[!UICONTROL Metadata Schema Editor]** page, customize the **[!UICONTROL Properties]** page of the asset by dragging one or more components from a list of component types in the **[!UICONTROL Build Form]** tab to the **[!UICONTROL Basic]** tab.

   ![](assets/metadata-schemaeditor-page.png)

1. Als u een component wilt configureren, selecteert u deze en wijzigt u de eigenschappen ervan op het **[!UICONTROL Settings]** tabblad.

### Componenten op het tabblad Formulier samenstellen {#components-in-the-build-form-tab}

Het **[!UICONTROL Build Form]** tabblad bevat items die u in het schema kunt gebruiken. Het **[!UICONTROL Settings]** tabblad bevat de kenmerken van elk item dat u op het **[!UICONTROL Build Form]** tabblad selecteert. De volgende tabel bevat een lijst met formulieritems die beschikbaar zijn op het **[!UICONTROL Build Form]** tabblad:

| Componentnaam | Beschrijving |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **[!UICONTROL Section Header]** | Voeg een sectiekopje toe voor een lijst met gangbare componenten. |
| **[!UICONTROL Single Line Text]** | Voeg een eigenschap voor één regel tekst toe. De eigenschap wordt opgeslagen als een tekenreeks. |
| **[!UICONTROL Multi ValueText]** | Voeg een teksteigenschap met meerdere waarden toe. Deze wordt opgeslagen als een tekenreeks-array. |
| **[!UICONTROL Number]** | Voeg een getalcomponent toe. |
| **[!UICONTROL Date]** | Voeg een datumcomponent toe. |
| **[!UICONTROL Dropdown]** | Voeg een vervolgkeuzelijst toe. |
| **[!UICONTROL Standard Tags]** | Voeg een tag toe. **Opmerking:** Beheerders moeten mogelijk de padwaarde wijzigen `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`als ze de metagegevensschemavorm van AEM publiceren, waarbij het pad bijvoorbeeld geen huurdersinformatie bevat `/etc/tags/<custom_tag_namespace>`. |
| **[!UICONTROL Smart Tags]** | Automatisch gedetecteerde tags als u de invoegtoepassing voor slimme tags van AEM hebt aangeschaft en geconfigureerd. |
| **[!UICONTROL Hidden Field]** | Voeg een verborgen veld toe. Deze wordt als een POST-parameter verzonden wanneer het element wordt opgeslagen. |
| **[!UICONTROL Asset Referenced By]** | Voeg deze component toe om een lijst weer te geven met elementen waarnaar door het element wordt verwezen. |
| **[!UICONTROL Asset Referencing]** | Toevoegen om een lijst weer te geven met elementen die naar het element verwijzen. |
| **[!UICONTROL Asset Rating]** | Gemiddelde rating van een actief dat aan AEM Assets is toegevoegd voordat het aan Brand Portal wordt gepubliceerd. |
| **[!UICONTROL Contextual Metadata]** | Toevoegen om de weergave van andere tabbladen met metagegevens op de pagina Eigenschappen van elementen te bepalen. |

>[!NOTE]
>
>Niet gebruiken **[!UICONTROL Product References]**, omdat het niet functioneel is.

#### De metagegevenscomponent bewerken {#edit-the-metadata-component}

Als u de eigenschappen van een metagegevenscomponent in het formulier wilt bewerken, klikt u op de component en bewerkt u de eigenschappen ervan op het **[!UICONTROL Settings]** tabblad.

* **[!UICONTROL Field Label]**: De naam van de eigenschap metadata die wordt weergegeven op de pagina Eigenschappen van het element.

* **[!UICONTROL Map to Property]**: De waarde van deze eigenschap geeft het relatieve pad/de relatieve naam aan naar het knooppunt met middelen waar het wordt opgeslagen in de CRX-opslagruimte. Het begint met &quot;**./**&quot; omdat het aangeven dat het pad zich onder het knooppunt van het element bevindt.

Hier volgen de geldige waarden voor deze eigenschap:

-- `./jcr:content/metadata/dc:title`: Hiermee wordt de waarde in het metadataknooppunt van de asset opgeslagen als de eigenschap [!UICONTROL `dc:title`].

-- `./jcr:created`: Geeft de JCR-eigenschap weer op het knooppunt van de asset. Als u deze eigenschappen configureert op weergave-eigenschappen, raden wij aan deze te markeren als Bewerken uitschakelen, omdat deze beveiligd zijn. Anders treedt de fout &quot;Wijzigen van asset(s)&quot; op wanneer u de eigenschappen van de asset opslaat.

* **[!UICONTROL Placeholder]**: Gebruik deze eigenschap om de gebruiker relevante informatie over de eigenschap metadata te geven.
* **[!UICONTROL Required]**: Gebruik deze eigenschap om een eigenschap metadata als verplicht op de pagina Eigenschappen te markeren.
* **[!UICONTROL Disable Edit]**: Gebruik deze eigenschap om een eigenschap metadata onbewerkbaar te maken op de pagina Eigenschappen.
* **[!UICONTROL Show Empty Field In Read Only]**: Mark this property to display a metadata property on the Properties page even if it has no value. Wanneer een eigenschap metadata geen waarde heeft, wordt deze standaard niet weergegeven op de pagina Eigenschappen.
* **[!UICONTROL Description]**: Gebruik deze eigenschap om een korte beschrijving toe te voegen voor de metagegevenscomponent.
* **[!UICONTROL Delete icon]**: Klik op dit pictogram om een component uit het schema te verwijderen.

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>Alle metagegevensvelden zijn alleen-lezen in de vorm van de metagegevenseditor van een element. Aangezien metagegevens van het element moeten worden bewerkt in AEM Assets voordat een element naar Brand Portal kan worden gepubliceerd.

#### Een tabblad toevoegen aan of verwijderen uit het schemaformulier {#add-or-delete-a-tab-in-the-schema-form}

The default schema form includes the **[!UICONTROL Basic]** and **[!UICONTROL Advanced]** tabs. Met de schema-editor kunt u een tabblad toevoegen of verwijderen.

![](assets/add_delete_tabs_metadataschemaform.png)

* Als u een nieuw tabblad wilt toevoegen aan een schemaformulier, klikt u op **[!UICONTROL +]**. Standaard heeft het nieuwe tabblad de naam &quot;Naamloos-1&quot;. U kunt de naam wijzigen van het **[!UICONTROL Settings]** tabblad.

![](assets/add-tab-metadata-form.png)

* Als u een tabblad wilt verwijderen, klikt u **[!UICONTROL x]** op. Click **[!UICONTROL Save]** to save the changes.

## Een metagegevensschema toepassen op een map {#apply-a-metadata-schema-to-a-folder}

Met het Brand Portal kunt u het metagegevensschema aanpassen en beheren, zodat op de **[!UICONTROL Properties]** pagina van een element alleen de specifieke informatie wordt weergegeven die u wilt weergeven. Als u de metagegevens wilt beheren die op de **[!UICONTROL Properties]** pagina worden weergegeven, verwijdert u de vereiste metagegevens uit het metagegevensschema en past u deze toe op de specifieke map.

Ga als volgt te werk om een metagegevensschema-formulier toe te passen op een map:

1. Klik op de AEM-werkbalk boven in het scherm op het Adobe-logo voor toegang tot beheergereedschappen.

   ![](assets/aemlogo.png)

1. Klik in het deelvenster met beheergereedschappen op **[!UICONTROL Metadata Schemas]**.

1. Selecteer op de **[!UICONTROL Metadata Schema Forms]** pagina het schema dat u bijvoorbeeld op een element wilt toepassen **[!UICONTROL clothing]**.

   ![](assets/apply-metadata-schema-form-to-folder.png)

1. Klik op de werkbalk boven in het scherm **[!UICONTROL Apply to Folder(s)]**.

1. Navigeer vanaf de **[!UICONTROL Select Folder(s)]** pagina naar de map waarop u bijvoorbeeld het **[!UICONTROL clothing]** metagegevensschema wilt toepassen **[!UICONTROL Gloves]**.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

1. Klik **[!UICONTROL Apply]** om het formulier met het metagegevensschema op de map toe te passen.

   De metagegevens die beschikbaar zijn in het **[!UICONTROL clothing]** metagegevensschema worden toegepast op de **[!UICONTROL Gloves]** map en worden weergegeven op de **[!UICONTROL Properties]** pagina van de map.

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>Als u een schema met geneste schema&#39;s toepast op een map met videobestanden, worden de eigenschappen van metagegevens voor de videobestanden mogelijk niet correct gerenderd. Om ervoor te zorgen dat de eigenschappen van metagegevens correct worden weergegeven, verwijdert u de geneste schema&#39;s en past u alleen het bovenliggende schema toe op de map.

## Een metagegevensschema verwijderen {#delete-a-metadata-schema-form}

Met Merkportal kunt u alleen aangepaste schema-formulieren verwijderen. U kunt hiermee de standaardschema-formulieren/sjablonen niet verwijderen. U kunt echter alle aangepaste wijzigingen in deze formulieren verwijderen.

Als u een formulier wilt verwijderen, selecteert u een formulier en klikt u op het **[!UICONTROL Delete]** pictogram.

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>Nadat u de aangepaste wijzigingen hebt verwijderd die in een standaardformulier zijn aangebracht, wordt het **[!UICONTROL Lock]** symbool opnieuw vóór de formuliernaam weergegeven in de interface van het metagegevensschema om aan te geven dat de standaardstatus van het formulier wordt hersteld.

## Schema-formulieren voor MIME-TYPES {#schema-forms-for-mime-types}

### Nieuwe formulieren toevoegen voor MIME-typen {#adding-new-forms-for-mime-types}

Naast de standaardformulieren kunt u ook aangepaste formulieren toevoegen voor elementen van verschillende MIME-typen of een nieuw formulier maken onder een geschikt formuliertype. Als u bijvoorbeeld een nieuwe sjabloon voor het subtype **[!UICONTROL image/png]** wilt toevoegen, maakt u het formulier onder de &quot;image&quot;-formulieren. De titel voor het schemaformulier is de naam van het subtype. In dit geval is de titel &quot;png&quot;.

#### Het gebruiken van een bestaand schemamalplaatje voor diverse types MIME {#using-an-existing-schema-template-for-various-mime-types}

U kunt een bestaande sjabloon voor een ander MIME-type gebruiken. Gebruik bijvoorbeeld het formulier **image/jpeg** voor elementen van het MIME-type **image/png**.

In dit geval maakt u een nieuw knooppunt in [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`] de CRX-opslagplaats. Geef een naam voor het knooppunt op en definieer de volgende eigenschappen:

| **Naam** | **Type** | **Waarde** |
|---|---|---|
| exposedMimetype | Tekenreeks | image/jpeg |
| mimetypen | Tekenreeks[] | image/png |

* **exposedmimetype**: Naam van het bestaande formulier dat moet worden toegewezen
* **mimetypen**: Lijst met MIME-typen die het formulier gebruiken dat is gedefinieerd in het **kenmerk exposedmimetype**

MIME-typen en -schema&#39;s worden toegewezen aan Brand Portal:

| **Schema-formulier** | **MIME-typen** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-ImageSet | Multipart/aanverwante; type=application/x-ImageSet |
| application/x-SpinSet | Multipart/aanverwante; type=application/x-SpinSet |
| application/x-MixedMediaSet | Multipart/aanverwante; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg4 | video/mp4 |
| video/avi | video/avi, video/msvideo, video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

Hieronder volgt een lijst met standaardeigenschappen van metagegevens:

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr:content/metadata/videoCodec
* jcr:content/metadata/audioCodec
* jcr:content/metadata/dc:title
* jcr:content/metadata/dc:description
* jcr:content/metadata/xmpMM:InstanceID
* jcr:content/metadata/xmpMM:DocumentID
* jcr:content/metadata/dam:sha1
* jcr:content/metadata/dam:solutionContext
* jcr:content/metadata/videoBitrate
* jcr:content/metadata/audioBitrate
* jcr:content/usages/usedBy
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr:content/onTime
* jcr:content/offTime
* jcr:content/metadata/dam:size
* jcr:content/metadata/tiff:ImageWidth
* jcr:content/metadata/tiff:ImageLength
