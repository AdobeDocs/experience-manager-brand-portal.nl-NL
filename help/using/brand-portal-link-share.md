---
title: Elementen delen als koppeling
seo-title: Elementen delen als koppeling
description: Beheerders van AEM Assets Brand Portal kunnen koppelingen van meerdere middelen delen met geautoriseerde interne gebruikers en externe entiteiten, waaronder partners en leveranciers. Editors kunnen alleen de elementen weergeven en delen die met hen worden gedeeld.
seo-description: Beheerders van AEM Assets Brand Portal kunnen koppelingen van meerdere middelen delen met geautoriseerde interne gebruikers en externe entiteiten, waaronder partners en leveranciers. Editors kunnen alleen de elementen weergeven en delen die met hen worden gedeeld.
uuid: 8889ac24-c56d-4a47-b792-80c34ffb5c3f
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f3573219-3c58-47ba-90db-62b003d8b9aa
translation-type: tm+mt
source-git-commit: 9c937603cf325919cb49d3418b06266fa1b93cf1
workflow-type: tm+mt
source-wordcount: '1078'
ht-degree: 1%

---


# Elementen delen als een koppeling {#share-assets-as-a-link}

Beheerders van AEM Assets Brand Portal kunnen koppelingen van meerdere middelen delen met geautoriseerde interne gebruikers en externe entiteiten, waaronder partners en leveranciers. Editors kunnen alleen de elementen weergeven en delen die met hen worden gedeeld.

Het delen van elementen via een koppeling is een handige manier om deze beschikbaar te maken voor externe partijen, aangezien de ontvangers zich niet hoeven aan te melden bij Brand Portal voor toegang tot de middelen.

De verbinding die toegang deelt is beperkt tot editors en beheerders.

Zie [Gebruikers, groepen en gebruikersrollen beheren](../using/brand-portal-adding-users.md#manage-user-roles) voor meer informatie.

>[!NOTE]
>
>Maximaal 5 GB ZIP-download is toegestaan met de functie voor delen van koppelingen op Brand Portal.


Hieronder vindt u de stappen voor het delen van elementen als een koppeling:

1. Klik op het bedekkingspictogram aan de linkerkant en kies **[!UICONTROL Navigation]**.

   ![](assets/siderail.png)

1. Klik in de handleiding aan de linkerkant op **[!UICONTROL Files]** om mappen of afbeeldingen te delen. Als u verzamelingen wilt delen, klikt u op **[!UICONTROL Collections]**.

   ![](assets/navigationrail.png)

1. Selecteer de mappen of verzamelingen die u als koppeling wilt delen.

   ![](assets/asset-link-share.png)

1. Klik op het pictogram **[!UICONTROL Share Link]** op de werkbalk boven in het scherm.

   Het dialoogvenster **[!UICONTROL Link Sharing]** wordt weergegeven.

   ![](assets/link-sharing.png)

   >[!NOTE]
   >
   >In het veld **[!UICONTROL Share Link]** wordt een automatisch gemaakte elementkoppeling weergegeven. De standaardvervaltijd voor deze koppeling is 7 dagen. U kunt de koppeling kopiëren en afzonderlijk met gebruikers delen of deze delen vanuit het dialoogvenster **[!UICONTROL Link Sharing]**.

1. Typ in het vak E-mailadres de e-mailadres van de gebruiker met wie u de koppeling wilt delen. U kunt de koppeling delen met meerdere gebruikers.

   Als de gebruiker lid is van uw organisatie, selecteert u de desbetreffende e-mailadres in de suggesties in de vervolgkeuzelijst. Als de gebruiker extern is, typt u de volledige e-mailid en drukt u op **[!UICONTROL Enter]**; e-mailadres wordt toegevoegd aan de lijst met gebruikers.

   ![](assets/link-sharing-text.png)

1. Typ in het tekstvak **[!UICONTROL Subject]** een onderwerp voor het element dat u wilt delen.
1. Typ desgewenst een bericht in het tekstvak **[!UICONTROL Message]**.
1. Gebruik in het veld **[!UICONTROL Expiration]** de datumkiezer om een vervaldatum en -tijd voor de koppeling op te geven. De vervaldatum is standaard ingesteld op 7 dagen vanaf de datum waarop u de koppeling deelt.

   De elementen die via de koppeling worden gedeeld, verlopen na het overschrijden van de datum en tijd die in het veld **[!UICONTROL Expiration]** zijn opgegeven. Zie [Digitale rechten van middelen beheren](../using/manage-digital-rights-of-assets.md#asset-expiration) voor informatie over het gedrag van verlopen elementen en wijzigingen in de toegestane activiteiten op basis van gebruikersrollen in Brand Portal.

1. Klik op **[!UICONTROL Share]**. Een bericht bevestigt dat de koppeling wordt gedeeld met de gebruikers. Gebruikers ontvangen een e-mail met de koppeling.

   ![](assets/link-sharing-email.png)

   >[!NOTE]
   >
   >Beheerders kunnen het e-mailbericht aanpassen. Dit omvat het aanpassen van het logo, de beschrijving en de voettekst met de functie [Branding](../using/brand-portal-branding.md).

## Elementen downloaden van gedeelde koppelingen {#download-assets-from-shared-links}

Klik op de koppeling in de e-mail om het gedeelde element weer te geven. De pagina AEM delen van koppeling wordt geopend.

De gedeelde elementen downloaden:

1. Klik op de elementen en klik vervolgens op het pictogram **[!UICONTROL Download]** op de werkbalk.

   ![](assets/assets-shared-link.png)

   >[!NOTE]
   >
   >Op dit moment kunt u, afhankelijk van de bestandsindeling, alleen voor bepaalde elementen een voorvertoning en miniatuur genereren. Zie [Ondersteuning van voorvertoningen en miniaturen voor asset-indelingen](#preview-thumbnail-support) voor meer informatie over de ondersteunde bestandsindelingen.

   >[!NOTE]
   >
   >Als de elementen die u downloadt ook gelicentieerde elementen bevatten, wordt u doorgestuurd naar de pagina **[!UICONTROL Copyright Management]**. Selecteer op deze pagina de gelicentieerde elementen, klik op **[!UICONTROL Agree]** en klik vervolgens op **[!UICONTROL Download]**. Als u het niet eens bent, worden alleen de middelen zonder licentie gedownload.\
   >Voor met licentie beveiligde elementen is [licentieovereenkomst gekoppeld](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets). Dit gebeurt door de [metagegevenseigenschap](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) van het element in [!DNL AEM Assets] in te stellen.

   ![](assets/licensed-asset-download.png)

   Het dialoogvenster **[!UICONTROL Download]** wordt weergegeven.

   ![](assets/download-linkshare.png)

   * Selecteer **[!UICONTROL Enable download acceleration]** en [volg de wizard](../using/accelerated-download.md#download-workflow-using-file-accelerator) om het downloaden van bestanden die als de koppeling worden gedeeld, te versnellen. Raadpleeg [Handleiding voor het versnellen van downloads vanaf Brand Portal](../using/accelerated-download.md) voor meer informatie over het snel downloaden van middelen op Brand Portal.

1. Selecteer **[!UICONTROL Rendition(s)]** als u de vertoningen van elementen wilt downloaden naast de elementen van de gedeelde koppeling. Als u dat doet, wordt de optie **[!UICONTROL Exclude System Renditions]** standaard geselecteerd. Zo voorkomt u dat uitvoeringen buiten de box samen met goedgekeurde elementen of aangepaste uitvoeringen worden gedownload.

   Als u echter wilt dat automatisch gegenereerde uitvoeringen samen met aangepaste uitvoeringen kunnen worden gedownload, schakelt u de optie **[!UICONTROL Exclude System Renditions]** uit.

   >[!NOTE]
   >
   >Oorspronkelijke uitvoeringen worden niet gedownload via de gedeelde koppeling als de gebruiker die de elementen als een koppeling heeft gedeeld, niet [gemachtigd is door de beheerder om toegang te hebben tot de oorspronkelijke uitvoeringen](../using/brand-portal-adding-users.md#manage-group-roles-and-privileges).

   ![](assets/download-linkshare-autoren.png)

1. Tik of klik op **[!UICONTROL Download]**. De elementen (en de vertoningen als geselecteerd) worden gedownload als dossier van het PIT aan uw lokale omslag. Er wordt echter geen .zip-bestand gemaakt als één element zonder de uitvoeringen wordt gedownload, zodat het snel kan worden gedownload.

>[!NOTE]
>
>Brand Portal beperkt het downloaden van elementen die groter zijn dan 5 GB per bestandsgrootte.

## Ondersteuning voor voorvertoningen en miniaturen van asset-indelingen {#preview-thumbnail-support}

De volgende matrix geeft een overzicht van de indelingen voor elementen waarvoor Brand Portal miniatuur en voorvertoning ondersteunt:

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
| TTF | ✕ | ✕ |
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
| NA | Deze functie is niet van toepassing op deze bestandsindeling |
| * | Voor deze functie is add-on ondersteuning voor deze bestandsindeling vereist op AEM auteurinstantie, maar niet op Brand Portal nadat de middelen naar Brand Portal zijn gepubliceerd |

## Delen van elementen die worden gedeeld als een koppeling {#unshare-assets-shared-as-a-link} opheffen

Ga als volgt te werk als u eerder gedeelde elementen als een koppeling wilt opheffen:

1. Als u de elementen die u als koppelingen hebt gedeeld, wilt weergeven, klikt u op het bedekkingspictogram aan de linkerkant en kiest u **[!UICONTROL Navigation]**.

   ![](assets/siderail.png)

1. Van de siderail, klik **[!UICONTROL Shared Links]**.

   ![](assets/navigationrail.png)

1. Controleer de koppelingen die u hebt gedeeld vanuit de weergegeven lijst.
1. Als u een koppeling niet meer wilt delen in de lijst, selecteert u de koppeling en klikt u op het binpictogram naast de koppelingsingang of op het pictogram **[!UICONTROL Unshare]** op de werkbalk bovenaan.

   ![](assets/unshare-links.jpg)

   >[!NOTE]
   >
   >De weergave van gedeelde koppelingen is gebruikersspecifiek. Deze eigenschap toont niet alle verbindingen die door alle gebruikers van een huurder worden gedeeld.

1. Klik in het waarschuwingsbericht op **[!UICONTROL Continue]** om het delen te bevestigen. De vermelding voor de koppeling wordt verwijderd uit de lijst met gedeelde koppelingen.
