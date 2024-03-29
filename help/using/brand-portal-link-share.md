---
title: Elementen delen als koppeling
seo-title: Share assets as a link
description: Adobe Experience Manager Assets Brand Portal-beheerders kunnen koppelingen van meerdere middelen delen met geautoriseerde interne gebruikers en externe entiteiten, waaronder partners en leveranciers. Editors kunnen alleen de elementen weergeven en delen die met hen worden gedeeld.
seo-description: Adobe Experience Manager Assets Brand Portal Administrators can share links of multiple assets with authorized internal users and external entities, including partners and vendors. Editors can view and share only the assets shared with them.
uuid: 8889ac24-c56d-4a47-b792-80c34ffb5c3f
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
exl-id: 9d254e95-a4fc-468d-ae1f-9690ddd3b4a1
source-git-commit: e3e35ad4be5c082ad7bac7bed8ea20a186d245ad
workflow-type: tm+mt
source-wordcount: '935'
ht-degree: 0%

---

# Elementen delen als koppeling {#share-assets-as-a-link}

Adobe Experience Manager Assets Brand Portal-beheerders kunnen koppelingen van meerdere middelen delen met geautoriseerde interne gebruikers en externe entiteiten, waaronder partners en leveranciers. Editors kunnen alleen de elementen weergeven en delen die met hen worden gedeeld.

Het delen van elementen via een koppeling is een handige manier om deze beschikbaar te maken voor externe partijen, aangezien de ontvangers zich niet hoeven aan te melden bij Brand Portal om toegang te krijgen tot de middelen.

<!-- Link sharing access is restricted to editors and administrators. 
-->

Zie voor meer informatie [Gebruikers, groepen en gebruikersrollen beheren](../using/brand-portal-adding-users.md#manage-user-roles).


Hieronder vindt u de stappen voor het delen van elementen als een koppeling:

1. Meld u aan bij uw Brand Portal-huurder. Standaard worden de **[!UICONTROL Files]** wordt geopend met alle gepubliceerde elementen en mappen.

1. Selecteer de elementen of mappen die u wilt delen, of navigeer naar de **[!UICONTROL Collections]** om de gemaakte verzamelingen te delen.

   ![select-multiple-assets](assets/select-assets-new.png)

1. Klik in de werkbalk bovenaan op de knop **[!UICONTROL Share Link]** pictogram.

   De **[!UICONTROL Link Sharing]** wordt weergegeven.

   ![](assets/link-sharing.png)

   * Typ in het vak E-mailadres de e-mailadres van de gebruiker met wie u de koppeling wilt delen. U kunt de koppeling delen met meerdere gebruikers. Als de gebruiker lid is van uw organisatie, selecteert u de desbetreffende e-mailadres in de suggesties in de vervolgkeuzelijst. Als de gebruiker extern is, typt u de volledige e-mailid en drukt u op **[!UICONTROL Enter]**; e-mailadres wordt toegevoegd aan de lijst met gebruikers.

      ![](assets/link-sharing-text.png)

   * In de **[!UICONTROL Subject]** typt u een onderwerp voor het element dat u wilt delen.
   * In de **[!UICONTROL Message]** Typ indien nodig een bericht.
   * In de **[!UICONTROL Expiration]** in het veld gebruikt u de datumkiezer om een vervaldatum en -tijd voor de koppeling op te geven. De vervaldatum is standaard ingesteld op 7 dagen vanaf de datum waarop u de koppeling deelt.
   * De optie **[!UICONTROL Allow downlod of original file]** Schakel het selectievakje in zodat de ontvangers de oorspronkelijke vertoning kunnen downloaden.

   De elementen die via de koppeling worden gedeeld, verlopen nadat de datum en tijd die in de **[!UICONTROL Expiration]** veld. Voor informatie over het gedrag van verlopen activa en wijzigingen in de toegestane activiteiten op basis van gebruikersrollen in Brand Portal raadpleegt u [Digitale rechten van middelen beheren](../using/manage-digital-rights-of-assets.md#asset-expiration).

   >[!NOTE]
   >
   >De standaardvervaltijd voor de verbinding is 7 dagen. De koppeling moet naar de gebruikers worden gemaild met de **[!UICONTROL Link Sharing]** kopiëren en delen de koppeling niet afzonderlijk.

1. Klik op **[!UICONTROL Share]**. Een bericht bevestigt dat de koppeling wordt gedeeld met de gebruikers. Gebruikers ontvangen een e-mail met de gedeelde koppeling.

   ![](assets/link-share-email.png)

   >[!NOTE]
   >
   >Beheerders kunnen het e-mailbericht aanpassen. Dit omvat het aanpassen van het logo, de beschrijving en de voettekst met [Branding](../using/brand-portal-branding.md) gebruiken.

## Elementen downloaden van gedeelde koppelingen {#download-assets-from-shared-links}

Klik op de koppeling in de e-mail om het gedeelde element te openen. De pagina AEM delen van koppeling wordt geopend.

De gedeelde elementen downloaden:

1. Klik op de elementen of mappen en klik vervolgens op de knop **[!UICONTROL Download]** op de werkbalk.

   ![](assets/download-share-link.png)

   >[!NOTE]
   >
   >Op dit moment kunt u, afhankelijk van de bestandsindeling, alleen voor bepaalde elementen een voorvertoning en miniatuur genereren. Voor meer informatie over de ondersteunde bestandsindelingen raadpleegt u [Ondersteuning voor voorvertoningen en miniaturen van asset-indelingen](#preview-thumbnail-support).

1. De **[!UICONTROL Download]** wordt weergegeven.

   ![download-dialog](assets/download-dialog-box-new.png)

1. Standaard worden de **[!UICONTROL Fast Download]** instelling is ingeschakeld in het dialoogvenster **[!UICONTROL Download Settings]**. Daarom wordt een bevestigingsvenster weergegeven waarin u kunt doorgaan met downloaden met IBM Aspera Connect.

   Als u wilt doorgaan met gebruiken **[!UICONTROL Fast Download]**, klikt u op **[!UICONTROL Allow]**.

   Alle geselecteerde uitvoeringen worden gedownload in een ZIP-map met een aparte map voor elk element.

   >[!NOTE]
   >
   >Voor elk element wordt een aparte map gemaakt terwijl de elementen worden gedownload van een gedeelde koppeling.
   >
   >Als er een map, verzameling of meer dan 20 elementen zijn geselecteerd om te worden gedownload, wordt de opdracht **[!UICONTROL Download]** wordt overgeslagen en alle elementenuitvoeringen die voor de gebruiker toegankelijk zijn, met uitzondering van de dynamische uitvoeringen, worden gedownload in een ZIP-map met een aparte map voor elk element.

   >[!NOTE]
   >
   >Oorspronkelijke uitvoeringen worden niet gedownload via de gedeelde koppeling als de gebruiker die de elementen als koppeling heeft gedeeld, [door de beheerder gemachtigd om toegang te hebben tot de oorspronkelijke vertoningen](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).


>[!NOTE]
>
>Brand Portal beperkt het downloaden van mappen of elementen met een grootte van meer dan 5 GB aan de hand van gedeelde koppelingen.

<!--
1. The **[!UICONTROL Download]** dialog box appears.

   ![](assets/download-linkshare.png)

    * To speed up the download of asset files shared as the link, select **[!UICONTROL Enable download acceleration]** option and [follow the wizard](../using/accelerated-download.md#download-workflow-using-file-accelerator). To know more about the fast download of assets on Brand Portal refer [Guide to accelerate downloads from Brand Portal](../using/accelerated-download.md).
    
1. To download the renditions of assets in addition to the assets from the shared link, select **[!UICONTROL Rendition(s)]** option. When you do so, **[!UICONTROL Exclude System Renditions]** option appears that is selected by default. This prevents the download of out-of-the-box renditions along with approved assets or their custom renditions.

   However, to allow auto-generated renditions to download along with custom renditions, deselect the **[!UICONTROL Exclude System Renditions]** option.

   >[!NOTE]
   >
   >Original renditions are not downloaded using the shared link if the user who shared the assets as a link is not [authorized by the administrator to have access to the original renditions](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).

   ![](assets/download-linkshare-autoren.png)

1. Click **[!UICONTROL Download]**. The assets (and renditions if selected) are downloaded as a ZIP file to your local folder. However, no zip file is created if a single asset is downloaded without any of the renditions, thereby ensuring speedy download.

-->

## Ondersteuning voor voorvertoningen en miniaturen van asset-indelingen {#preview-thumbnail-support}

De volgende matrix geeft een overzicht van de indelingen voor elementen waarvoor Brand Portal miniaturen en voorvertoningen ondersteunt:

| Elementformaat | Ondersteuning voor miniaturen | Ondersteuning voor voorvertoningen |
|--------------|-------------------|-----------------|
| PNG | ✓ | ✓ |
| GIF | ✓ | ✓ |
| TIFF | ✓ | ✕ |
| JPEG | ✓ | ✓ |
| BMP | ✓ | ✕ |
| PNM* | NA | NA |
| PGM* | NA | NA |
| PBM* | NA | NA |
| PPM* | NA | NA |
| PSD | ✓ | ✕ |
| EPS | NA | ✕ |
| DNG | ✓ | ✕ |
| PICT | ✓ | ✕ |
| PSB* | ✓ | ✕ |
| JPG | ✓ | ✓ |
| AI | ✓ | ✕ |
| DOC | ✕ | ✕ |
| DOCX | ✕ | ✕ |
| ODT* | ✕ | ✕ |
| PDF | ✓ | ✕ |
| HTML | ✕ | ✕ |
| RTF | ✕ | ✕ |
| TXT | ✓ | ✕ |
| XLS | ✕ | ✕ |
| XLSX | ✕ | ✕ |
| ODS | ✕ | ✕ |
| PPT | ✓ | ✕ |
| PPTX | ✕ | ✕ |
| ODP | ✕ | ✕ |
| INDD | ✓ | ✕ |
| PS | ✕ | ✕ |
| QXP | ✕ | ✕ |
| ePub | ✓ | ✕ |
| AAC | ✕ | ✕ |
| MIDI | ✕ | ✕ |
| 3GP | ✕ | ✕ |
| MP3 | ✕ | ✕ |
| MP4 | ✕ | ✕ |
| OGA | ✕ | ✕ |
| OGG | ✕ | ✕ |
| RA | ✕ | ✕ |
| WAV | ✕ | ✕ |
| WMA | ✕ | ✕ |
| DVI | ✕ | ✕ |
| FLV | ✕ | ✕ |
| M4V | ✕ | ✕ |
| MPG | ✕ | ✕ |
| OGV | ✕ | ✕ |
| MOV | ✕ | ✕ |
| WMV | ✕ | ✕ |
| SWF | ✕ | ✕ |
| TGZ | NA | ✕ |
| JAR | ✓ | ✕ |
| RAR | NA | ✕ |
| TAR | NA | ✕ |
| ZIP | ✓ | ✕ |

In de volgende legenda worden de symbolen uitgelegd die in de matrix worden gebruikt:

| Symbool | Betekenis |
|---|---|
| ✓ | Deze bestandsindeling ondersteunt deze functie |
| ✕ | Deze functie wordt niet ondersteund door deze bestandsindeling |
| NA | Deze functie is niet van toepassing op deze bestandsindeling |
| &#42; | Voor deze functie is aanvullende ondersteuning voor deze bestandsindeling vereist op AEM auteurinstantie, maar niet op Brand Portal nadat elementen naar Brand Portal zijn gepubliceerd |

## Delen van elementen die worden gedeeld als koppeling opheffen {#unshare-assets-shared-as-a-link}

Ga als volgt te werk als u eerder gedeelde elementen als een koppeling wilt opheffen:

1. Wanneer u zich aanmeldt bij Brand Portal, wordt **[!UICONTROL File]** wordt standaard geopend. Als u de elementen die u als koppelingen hebt gedeeld, wilt weergeven, navigeert u naar de **[!UICONTROL Shared Links]** weergeven.

1. Controleer de koppelingen die u hebt gedeeld vanuit de weergegeven lijst.

   ![](assets/shared-links.png)

1. Als u een koppeling uit de lijst wilt verwijderen, selecteert u de koppeling en klikt u op de knop **[!UICONTROL Unshare]** van de werkbalk bovenaan.

   ![](assets/unshare-asset.png)

   >[!NOTE]
   >
   >De weergave van gedeelde koppelingen is gebruikersspecifiek. Deze eigenschap toont niet alle verbindingen die door alle gebruikers van een huurder worden gedeeld.

1. Klik in het waarschuwingsbericht op **[!UICONTROL Continue]** om te bevestigen dat u niet deelt. De vermelding voor de koppeling wordt verwijderd uit de lijst met gedeelde koppelingen.
