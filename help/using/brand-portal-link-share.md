---
title: Elementen delen als koppeling
description: Leer hoe Adobe Experience Manager Assets Brand Portal-beheerders koppelingen van meerdere middelen kunnen delen met geautoriseerde interne gebruikers en externe entiteiten, waaronder partners en leveranciers. Editors kunnen alleen de elementen weergeven en delen die met hen worden gedeeld.
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
exl-id: 9d254e95-a4fc-468d-ae1f-9690ddd3b4a1
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1028'
ht-degree: 0%

---

# Elementen delen als koppeling {#share-assets-as-a-link}

Adobe Experience Manager Assets Brand Portal-beheerders kunnen koppelingen van meerdere middelen delen met geautoriseerde interne gebruikers en externe entiteiten, waaronder partners en leveranciers. Editors kunnen alleen de elementen weergeven en delen die met hen worden gedeeld.

Het delen van elementen via een koppeling is een handige manier om deze beschikbaar te maken voor externe partijen, aangezien de ontvangers zich niet hoeven aan te melden bij Brand Portal om toegang te krijgen tot de middelen.

<!-- Link sharing access is restricted to editors and administrators. 
-->

Voor meer informatie, zie [ het Leiden gebruikers, groepen, en gebruikersrollen ](../using/brand-portal-adding-users.md#manage-user-roles).


Hier volgen de stappen om elementen als een koppeling te delen:

1. Meld u aan bij uw Brand Portal-huurder. Standaard wordt de weergave **[!UICONTROL Files]** geopend die alle gepubliceerde elementen en mappen bevat.

1. Selecteer de elementen of mappen die u wilt delen, of navigeer naar de **[!UICONTROL Collections]** -weergave om de gemaakte verzamelingen te delen.

   ![ selecteren-veelvoud-activa ](assets/select-assets-new.png)

1. Klik op het pictogram **[!UICONTROL Share Link]** op de werkbalk boven in het scherm.

   Het dialoogvenster **[!UICONTROL Link Sharing]** wordt weergegeven.

   ![](assets/link-sharing.png)

   * Typ in het vak E-mailadres de e-mailadres van de gebruiker met wie u de koppeling wilt delen. U kunt de koppeling delen met meerdere gebruikers. Als de gebruiker lid is van uw organisatie, selecteert u de desbetreffende e-mailadres in de suggesties in de vervolgkeuzelijst. Als de gebruiker een externe gebruiker is, typt u de volledige e-mailid en drukt u op **[!UICONTROL Enter]** . De e-mailid wordt dan toegevoegd aan de lijst met gebruikers.

     ![](assets/link-sharing-text.png)

   * Typ in het vak **[!UICONTROL Subject]** een onderwerp voor het element dat u wilt delen.
   * Typ desgewenst een bericht in het vak **[!UICONTROL Message]** .
   * Gebruik in het veld **[!UICONTROL Expiration]** de datumkiezer om een vervaldatum en -tijd voor de koppeling op te geven. De vervaldatum is standaard ingesteld op 7 dagen vanaf de datum waarop u de koppeling deelt.
   * Schakel het selectievakje **[!UICONTROL Allow download of the original file]** in zodat de ontvangers de oorspronkelijke vertoning kunnen downloaden.

   De elementen die via de koppeling worden gedeeld, verlopen na het overschrijden van de datum en tijd die in het veld **[!UICONTROL Expiration]** zijn opgegeven. Voor details op verlopen activa en op rol-gebaseerde activiteitenveranderingen in Brand Portal, zie [ digitale rechten van activa beheren ](../using/manage-digital-rights-of-assets.md#asset-expiration).

   >[!NOTE]
   >
   >De standaardvervaltijd voor de verbinding is 7 dagen. De koppeling moet naar de gebruikers worden gemaild via het dialoogvenster **[!UICONTROL Link Sharing]** . Kopieer en deel de koppeling niet afzonderlijk.

1. Klik op **[!UICONTROL Share]**. Een bericht bevestigt dat de koppeling wordt gedeeld met de gebruikers. Gebruikers ontvangen een e-mail met de gedeelde koppeling.

   ![](assets/link-share-email.png)

   >[!NOTE]
   >
   >De beheerders kunnen het e-mailoverseinen aanpassen, dat het aanpassen van embleem, beschrijving, en footer met [ Brandend ](../using/brand-portal-branding.md) eigenschap omvat.

## Elementen downloaden van gedeelde koppelingen {#download-assets-from-shared-links}

Klik op de koppeling in de e-mail om het gedeelde element te openen. De pagina AEM delen van koppeling wordt geopend.

De gedeelde elementen downloaden:

1. Klik op de elementen of mappen en klik vervolgens op het pictogram **[!UICONTROL Download]** op de werkbalk.

   ![](assets/download-share-link.png)

   >[!NOTE]
   >
   >Op dit moment kunt u, afhankelijk van de bestandsindeling, alleen voor bepaalde elementen een voorvertoning en miniatuur genereren. Voor meer informatie over de gesteunde dossierformaten, zie [ Voorproef en duimnagelsteun voor activa formaten ](#preview-thumbnail-support).

1. Het dialoogvenster **[!UICONTROL Download]** wordt weergegeven.

   ![ download-dialoog ](assets/download-dialog-box-new.png)

1. De instelling **[!UICONTROL Fast Download]** wordt standaard ingeschakeld in **[!UICONTROL Download Settings]** . Daarom wordt een bevestigingsvenster weergegeven waarin het downloaden met IBM® Aspera Connect wordt voortgezet.

   Klik op **[!UICONTROL Allow]** als u **[!UICONTROL Fast Download]** wilt blijven gebruiken.

   Alle geselecteerde uitvoeringen worden gedownload in een ZIP-map met een aparte map voor elk element.

   >[!NOTE]
   >
   >Voor elk element wordt een aparte map gemaakt terwijl de elementen worden gedownload van een gedeelde koppeling.
   >
   >Als een map, verzameling of meer dan 20 elementen zijn geselecteerd, wordt het dialoogvenster **[!UICONTROL Download]** overgeslagen. Bovendien worden alle toegankelijke elementuitvoeringen (behalve dynamische) gedownload in een ZIP-map met aparte mappen voor elk element.

   >[!NOTE]
   >
   >Als de beheerder de gebruiker die de elementen heeft gedeeld niet heeft geautoriseerd, downloadt de gedeelde koppeling de oorspronkelijke vertoningen niet. Zie ook [ die door de beheerder wordt gemachtigd om toegang tot de originele vertoningen ](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges) te hebben.


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

| Elementformaat | Ondersteuning voor miniaturen | Ondersteuning voor voorvertoning |
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
| EPUB | ✓ | ✕ |
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
| NA | Deze functie geldt niet voor deze bestandsindeling |
| &#42; | Voor deze functie is aanvullende ondersteuning voor deze bestandsindeling vereist op AEM auteurinstantie, maar niet op Brand Portal nadat elementen naar Brand Portal zijn gepubliceerd |

## Delen van elementen die worden gedeeld als koppeling opheffen {#unshare-assets-shared-as-a-link}

Ga als volgt te werk als u eerder gedeelde elementen als een koppeling wilt opheffen:

1. Wanneer u zich aanmeldt bij Brand Portal, wordt de weergave **[!UICONTROL File]** standaard geopend. Navigeer naar de **[!UICONTROL Shared Links]** -weergave om de elementen die u als koppelingen hebt gedeeld, weer te geven.

1. Controleer de koppelingen die u vanuit de weergegeven lijst hebt gedeeld.

   ![](assets/shared-links.png)

1. Als u een koppeling niet meer wilt delen in de lijst, selecteert u de koppeling en klikt u op het pictogram **[!UICONTROL Unshare]** op de werkbalk boven in het scherm.

   ![](assets/unshare-asset.png)

   >[!NOTE]
   >
   >De weergave van gedeelde koppelingen is gebruikersspecifiek. Deze eigenschap toont niet alle verbindingen die door alle gebruikers van een huurder worden gedeeld.

1. Klik in het waarschuwingsbericht op **[!UICONTROL Continue]** om te bevestigen dat u het document niet deelt. De vermelding voor de koppeling wordt verwijderd uit de lijst met gedeelde koppelingen.
