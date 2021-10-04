---
title: 'De map met bijdragen configureren en publiceren van Experience Manager Assets naar Brand Portal '
seo-title: Configure and publish contribution folder from Experience Manager Assets to Brand Portal
description: Krijg inzicht in het vormen en publiceren van een bijdrageomslag van de Middelen van de Experience Manager aan Brand Portal.
seo-description: Get an insight into configuring and publishing a contribution folder from Experience Manager Assets to Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 9acad588-977a-45de-b544-f2cc8874ba12
source-git-commit: e95dbff93ec4d207fe32a1752f9ccf59ee7c4e90
workflow-type: tm+mt
source-wordcount: '1090'
ht-degree: 0%

---

# Contributiemap configureren in Experience Manager Assets {#configure-contribution-folder}

Voor gezamenlijke bronnen van middelen kunnen gebruikers van Experience Manager Assets (beheerders en gebruikers zonder beheerdersrechten) nieuwe mappen van het type **Asset Contribution** maken, zodat Brand Portal-gebruikers de nieuwe map kunnen verzenden.  Dit leidt automatisch tot een werkschema dat tot twee extra subomslagen, genoemd **SHARED** en **NEW**, binnen de pas gecreëerde **Bijdrage** omslag leidt.

De gebruiker van de Activa van de Experience Manager bepaalt dan de activavereisten door een kort over de types van activa te uploaden die aan de bijdrageomslag, evenals een reeks basisactiva, aan **SHARED** omslag zouden moeten worden toegevoegd om ervoor te zorgen de gebruikers van Brand Portal de informatie hebben zij nodig. De beheerder kan actieve Brand Portal-gebruikers vervolgens toegang tot de map met bijdragen geven voordat ze de nieuwe Contribute-map publiceren naar Brand Portal.

In de volgende video ziet u hoe u een map Contribution in Experience Manager Assets configureert:

>[!VIDEO](https://video.tv.adobe.com/v/30547)

De gebruiker van de Activa van de Experience Manager voert de volgende activiteiten terwijl het vormen van een bijdrageomslag uit:

* [Map voor bijdragen maken](#create-contribution-folder)
* [Elementvereisten uploaden en contribuanten toewijzen](#configure-contribution-folder-properties)
* [Basiselementen uploaden](#uplad-new-assets-to-contribution-folder)
* [Map met bijdragen publiceren van Experience Manager Assets naar Brand Portal](#publish-contribution-folder-to-brand-portal)

## Map voor bijdragen maken {#create-contribution-folder}


Beheerders van middelen van de Experience Manager en gebruikers niet-admin die toestemming hebben om een nieuwe omslag tot stand te brengen, kunnen een bijdrageomslag in de Middelen van de Experience Manager tot stand brengen.
Als u een map met bijdragen wilt maken, maakt u een nieuwe map van het type Asset Contribution. Zo zorgt u ervoor dat de nieuwe map die u maakt, kan worden verzonden door Brand Portal-gebruikers.  Dit leidt automatisch tot een werkschema dat tot twee extra subomslagen, genoemd GEDEELD en NIEUW, binnen de bijdrageomslag leidt.


>[!NOTE]
>
>U kunt meerdere mappen voor bijdragen maken in een map. Maak geen bijdragemap in een andere bijdragemap.

U kunt de eigenschappen van de bijdragemap afzonderlijk configureren en de bijdragemap maken. In dit voorbeeld configureren we de eigenschappen afzonderlijk.

**Een bijdragemap maken:**

1. Meld u aan bij de Experience Manager Assets-instantie.

1. Ga naar **[!UICONTROL Assets]** > **[!UICONTROL Files]**. Alle bestaande mappen in de gegevensopslagruimte van Experience Manager Assets worden weergegeven.

1. Klik **[!UICONTROL Create]** om een nieuwe omslag tot stand te brengen. **[!UICONTROL Create Folder]** wordt geopend.

1. Voer **[!UICONTROL Title]** en **[!UICONTROL Name]** van de map in en selecteer het selectievakje **[!UICONTROL Asset Contribution]**.
Het wordt aanbevolen kleine letters zonder ruimte te gebruiken om de map een naam te geven.

1. Klik op **[!UICONTROL Create]**. U kunt de bijdragemap zien in de gegevensopslagruimte van de Experience Manager Assets.

   >[!NOTE]
   >
   >Een gebruiker die geen beheerder is, kan een map voor middelenbijdragen maken en delen, maar kan deze niet wijzigen of verwijderen.


   ![](assets/create-contribution-folder.png)

1. Klik om de bijdragemap te openen. Er worden twee submappen weergegeven.-**[!UICONTROL SHARED]** en **[!UICONTROL NEW]** worden automatisch gemaakt in de bijdragemap.

   ![](assets/contribution-folder.png)


## Eigenschappen voor bijdragemappen configureren {#configure-contribution-folder-properties}

De beheerder van de Middelen van de Experience Manager voert de volgende activiteiten uit terwijl het vormen van de eigenschappen van een bijdrageomslag.

* **Beschrijving** toevoegen: Geef een beschrijving op hoog niveau van de map met bijdragen.
* **Uploadinstructie**: Document voor vereist element uploaden dat informatie over elementen bevat.
* **Medewerkers** toevoegen: Voeg Brand Portal-gebruikers toe om ze toegang te verlenen tot de map met bijdragen.

Het vereiste van activa verwijst naar de details die door beheerders worden verstrekt om contribuanten (gebruikers van Brand Portal) te helpen de behoefte en de vereisten van de bijdrageomslag begrijpen. De beheerder uploadt een document met middelenvereisten dat een korte beschrijving bevat van het type activa dat aan de bijdrageomslag en activa verwante informatie, bijvoorbeeld, doel, type van beelden, maximumgrootte, enz. zou moeten worden toegevoegd.

**Eigenschappen voor bijdragemappen configureren:**

1. Meld u aan bij de Experience Manager Assets-instantie.

1. Navigeer naar **[!UICONTROL Assets > Files]** en zoek de map met de bijdrage.
1. Selecteer de map met bijdragen en klik op **[!UICONTROL Properties]** om het venster Eigenschappen van map te openen.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. Navigeer naar het tabblad **[!UICONTROL Asset Contribution]**.
1. Voer op hoog niveau **[!UICONTROL Description]** van de bijdragemap in.
1. Klik **[!UICONTROL Upload Brief]** om van uw lokale machine te doorbladeren en **Document van de Vereiste van Activa te uploaden**.

   ![](assets/upload.png)

1. Voeg in het veld **[!UICONTROL Add User]** Brand Portal-gebruikers toe met wie u de bijdraamap wilt delen. Deze gebruikers kunnen met de Brand Portal-interface toegang krijgen tot inhoud en deze uploaden naar de map met bijdragen.
1. Klik op **[!UICONTROL Save]**.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>De zoekresultaten zijn gebaseerd op de Brand Portal-gebruikerslijst die is geconfigureerd in Experience Manager Assets. Controleer of u de bijgewerkte gebruikerslijst van Brand Portal hebt.

## Elementen uploaden naar de bijdragemap {#uplad-new-assets-to-contribution-folder}

De Brand Portal-gebruikers kunnen de vereisten voor middelen downloaden om te begrijpen of een bijdrage nodig is.
Vervolgens kunnen ze nieuwe middelen maken voor de bijdrage en deze uploaden naar de map NEW in de map met de bijdrage.

>[!NOTE]
>
>De Brand Portal-gebruikers kunnen alleen elementen uploaden naar de map NEW.
>
>De maximale uploadlimiet voor elke Brand Portal-huurder is **10** GB, die cumulatief wordt toegepast op alle mappen voor de bijdrage.


Na publicatie van de zojuist gemaakte elementen naar Experience Manager Assets kunnen de Brand Portal-gebruikers deze verwijderen uit de map NEW. De Brand Portal-beheerder kan de elementen echter verwijderen uit zowel de map NEW als de map SHARED.

Zodra het doel om de bijdrageomslag tot stand te brengen wordt bereikt, kan de beheerder van Brand Portal de bijdrageomslag schrappen om uploadruimte voor andere gebruikers vrij te geven.

>[!NOTE]
>
>U wordt aangeraden de uploadruimte vrij te geven nadat u de map met bijdragen hebt gepubliceerd naar Experience Manager Assets, zodat deze beschikbaar is voor de andere Brand Portal-gebruikers voor een bijdrage.
>
>Als het nodig is om de uploadlimiet van uw Brand Portal-huurder te verhogen tot meer dan **10** GB, neemt u contact op met de Klantenondersteuning om de vereiste op te geven.


**Nieuwe elementen uploaden:**

1. Meld u aan bij uw Brand Portal-exemplaar.
Het Brand Portal-dashboard weerspiegelt alle bestaande mappen die aan de Brand Portal-gebruiker zijn toegestaan, samen met de nieuw gedeelde bijdragemap.

1. Selecteer de map met de bijdrage en klik om deze te openen. De map voor bijdragen bevat twee submappen: **[!UICONTROL SHARED]** en **[!UICONTROL NEW]**.

1. Klik op de **[!UICONTROL NEW]** omslag.

   ![](assets/upload-new-assets1.png)

1. Klik op **[!UICONTROL Create]** > **[!UICONTROL Files]** om afzonderlijke bestanden of mappen (.zip) met meerdere elementen te uploaden.

   ![](assets/upload-new-assets2.png)

1. Blader naar elementen (bestanden of mappen) en upload deze naar de map **[!UICONTROL NEW]**.

   ![](assets/upload-new-assets3.png)

Nadat u alle elementen of mappen naar de map NEW hebt geüpload, publiceert u de map met bijdragen naar Experience Manager Assets.


## Bijdragemap publiceren naar Brand Portal {#publish-contribution-folder-to-brand-portal}

Zodra de bijdrageomslag wordt gevormd, kan de gebruiker van de Middelen van de Experience Manager (beheerder/niet-admin gebruiker) de bijdrageomslag van de Middelen van de Experience Manager aan Brand Portal publiceren. Brand Portal-gebruikers die toegang hebben tot de map met bijdragen, ontvangen een e-mail-/pulsmelding wanneer de publicatieactie is voltooid.


**Map met bijdragen publiceren:**

1. Meld u aan bij de Experience Manager Assets-instantie.

1. Navigeer naar **[!UICONTROL Assets > Files]** en zoek de map met bijdragen waarin u wilt publiceren naar Brand Portal.
1. Selecteer de map met bijdragen en klik op **[!UICONTROL Quick Publish]** > **[!UICONTROL Publish to Brand Portal]**.

   ![](assets/publish-contribution-folder-to-bp.png)

   U ontvangt een succesbericht zodra de map met bijdragen naar Brand Portal is gepubliceerd.

Er wordt een e-mail-/pulsmelding verzonden naar de Brand Portal-gebruikers die zijn toegewezen aan de bijdragemap. De Brand Portal-gebruikers hebben toegang tot de map met bijdragen en kunnen hun bijdrage starten. Zie [Elementen uploaden naar de bijdragemap en publiceren naar Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md).
