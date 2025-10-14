---
title: Contribute-map van Experience Manager Assets naar Brand Portal configureren en publiceren
description: Meer informatie over het configureren en publiceren van een bijdragemap van Experience Manager Assets naar Brand Portal.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: 9acad588-977a-45de-b544-f2cc8874ba12
source-git-commit: 9e51048d21c5b4a34696e668309657d2091a8b04
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 0%

---

# Contribute-map in Experience Manager Assets configureren {#configure-contribution-folder}

Voor samenwerkingsactiva die, de gebruikers van Experience Manager Assets (beheerders en niet-admin gebruikers die toestemming hebben) tot omslagen van het type **Bijdrage van Activa** leiden, die ervoor zorgen dat de gecreeerde omslag open voor activavoorlegging door de gebruikers van Brand Portal is.  Deze methode brengt automatisch een werkschema in werking dat tot twee extra subomslagen leidt, genoemd **GEDEELD** en **NIEUW**, binnen de pas gecreëerde **omslag van de Bijdrage**.

De Experience Manager Assets-gebruiker definieert de elementvereisten door een korte beschrijving te uploaden van de typen elementen die moeten worden toegevoegd aan de map met Help. Ze uploaden ook een set basislijnelementen naar de map SHARED om ervoor te zorgen dat gebruikers van Brand Portal over de benodigde informatie beschikken. De beheerder kan actieve Brand Portal-gebruikers vervolgens toegang tot de map met bijdragen geven voordat ze de nieuwe Contribute-map publiceren naar Brand Portal.

In de volgende video ziet u hoe u een Contribute-map in Experience Manager Assets configureert:

>[!VIDEO](https://video.tv.adobe.com/v/30547)

Experience Manager Assets-gebruiker voert de volgende activiteiten uit tijdens het configureren van een bijdragemap:

* [Een bijdragemap maken](#create-contribution-folder)
* [Elementvereisten uploaden en contribuanten toewijzen](#configure-contribution-folder-properties)
* [Basiselementen uploaden](#uplad-new-assets-to-contribution-folder)
* [Publish Contributiemap van Experience Manager Assets naar Brand Portal](#publish-contribution-folder-to-brand-portal)

## Map voor bijdragen maken {#create-contribution-folder}

Experience Manager Assets-beheerders en gebruikers die geen beheerder zijn en toestemming hebben om een nieuwe map te maken, kunnen een bijdragemap maken in Experience Manager Assets.
Als u een map met bijdragen wilt maken, maakt u een map met het type middelenbijdrage. Zo zorgt u ervoor dat de gemaakte map openstaat voor verzending van middelen door Brand Portal-gebruikers. Deze methode brengt automatisch een werkschema teweeg dat tot twee extra subomslagen, genoemd GEDEELD en NIEUW, binnen de bijdrageomslag leidt.

>[!NOTE]
>
>De beheerders kunnen meerdere mappen voor middelenbijdragen maken in een map.
>
>Een map met middelenbijdragen bevat de mappen NEW en SHARED voor de distributie en bijdrage van de elementen. Maak geen middelenmap of bijdragemap in een bijdragemap.


U kunt de eigenschappen van de bijdragemap afzonderlijk configureren, maar ook tijdens het maken van de bijdragemap. In dit voorbeeld worden de eigenschappen afzonderlijk geconfigureerd.

**om een bijdrageomslag tot stand te brengen:**

1. Meld u aan bij uw Experience Manager Assets-exemplaar.

1. Navigeer naar **[!UICONTROL Assets]** > **[!UICONTROL Files]** . Hier worden alle bestaande mappen in de Experience Manager Assets-opslagplaats vermeld.

1. Klik op **[!UICONTROL Create]** om een nieuwe map te maken. **[!UICONTROL Create Folder]** wordt geopend.

1. Voer de **[!UICONTROL Title]** en **[!UICONTROL Name]** van de map in en selecteer het selectievakje **[!UICONTROL Asset Contribution]** .
Adobe raadt u aan kleine letters te gebruiken zonder ruimte om de map een naam te geven.

1. Klik op **[!UICONTROL Create]**. U kunt de bijdragemap weergeven in de Experience Manager Assets-opslagplaats.

   >[!NOTE]
   >
   >Een gebruiker die geen beheerder is, kan een map voor middelenbijdragen maken en delen, maar kan deze niet wijzigen of verwijderen.


   ![](assets/create-contribution-folder.png)

1. Open de map met bijdragen. U kunt twee submappen zien - **[!UICONTROL SHARED]** en **[!UICONTROL NEW]** - die automatisch worden gemaakt in de bijdragemap.

   ![](assets/contribution-folder.png)


## Eigenschappen voor bijdragemappen configureren {#configure-contribution-folder-properties}

De beheerder van Experience Manager Assets voert de volgende activiteiten uit terwijl het vormen van de eigenschappen van een bijdrageomslag.

* **voeg beschrijving** toe: verstrek een beschrijving op hoog niveau van de bijdrageomslag.
* **uploadsamenvatting**: Upload een document van de activavereiste die activa op verwante informatie bevatten.
* **voegt contribuanten** toe: Voeg de gebruikers van Brand Portal toe om hen toegang tot de bijdrageomslag te verlenen.

Het vereiste van activa verwijst naar de details die door beheerders worden verstrekt om contribuanten (gebruikers van Brand Portal) te helpen de behoefte en de vereisten van de bijdrageomslag begrijpen. De beheerder uploadt een document met elementvereisten waarin de typen elementen voor de bijdragemap worden beschreven, zoals het doel, de afbeeldingstypen en de maximumgrootte.

**om de eigenschappen van de bijdrageomslag te vormen:**

1. Meld u aan bij uw Experience Manager Assets-exemplaar.

1. Navigeer naar **[!UICONTROL Assets > Files]** en zoek de map met Help.
1. Selecteer de map met bijdragen en klik op **[!UICONTROL Properties]** om het venster Eigenschappen van map te openen.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. Ga naar het tabblad **[!UICONTROL Asset Contribution]**.
1. Voer een eersteklas **[!UICONTROL Description]** van de map met Help in.
1. Klik **[!UICONTROL Upload Brief]** om van uw lokale machine te doorbladeren en een **Document van de Vereiste van Activa** te uploaden.

   ![](assets/upload.png)

1. Voeg in het veld **[!UICONTROL Add User]** Brand Portal-gebruikers toe met wie u de bijdraatiemap wilt delen. Deze gebruikers kunnen met de Brand Portal-interface toegang krijgen tot inhoud en deze uploaden naar de map met bijdragen.
1. Klik op **[!UICONTROL Save]**.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>De zoekresultaten zijn gebaseerd op de Brand Portal-gebruikerslijst die in Experience Manager Assets is geconfigureerd. Controleer of u de bijgewerkte gebruikerslijst van Brand Portal hebt.

De beheerders kunnen het `user.csv` -bestand downloaden van [!DNL Admin Console] en het gebruiken als de basissjabloon voor het toevoegen van Brand Portal-gebruikers. Ga naar [!UICONTROL Users] en klik op de optie [!UICONTROL Export users list to csv] om het `users.csv` -bestand te downloaden. De volgende voorbeeldgebruikers geven een overzicht van de kenmerken die vereist zijn voor het toevoegen van de gebruikers. Het enige verplichte kenmerk voor een gebruikersinvoer is `Email` en alle andere kenmerken zijn optioneel.

[Bestand ophalen](assets/users.csv)

## Elementen uploaden naar de bijdragemap {#uplad-new-assets-to-contribution-folder}

De gebruiker van Experience Manager Assets uploadt een reeks basislijnactiva aan de **GEDEELDE** omslag om ervoor te zorgen dat de gebruikers van Brand Portal de informatie hebben zij nodig.

**om basislijnactiva te uploaden:**

1. Meld u aan bij uw Experience Manager Assets-exemplaar.

1. Navigeer naar **[!UICONTROL Assets > Files]** en zoek de map met Help.

1. Selecteer de map met de bijdrage en klik om deze te openen.

1. Klik op de map **[!UICONTROL NEW]** .

   ![](assets/upload-new-assets1.png)

1. Klik op **[!UICONTROL Create]** > **[!UICONTROL Files]** om afzonderlijke bestanden of mappen (.zip) met meerdere elementen te uploaden.

   ![](assets/upload-new-assets2.png)

1. Blader naar en upload elementen (bestanden of mappen) naar de map **[!UICONTROL NEW]** .

   ![](assets/upload-asset4.png)

Nadat u alle elementen of mappen naar de map NEW hebt geüpload, publiceert u de map met bijdragen naar Experience Manager Assets.


## Publish Contributiemap naar Brand Portal {#publish-contribution-folder-to-brand-portal}

Als de map met bijdragen is geconfigureerd, kan Experience Manager Assets-gebruiker (beheerder/niet-beheerder) de map met bijdragen publiceren van Experience Manager Assets naar Brand Portal. Brand Portal-gebruikers die toegang hebben tot de map met bijdragen, ontvangen een e-mail- of pulsmelding wanneer de publicatieactie is voltooid.


**om een bijdrageomslag te publiceren:**

1. Meld u aan bij uw Experience Manager Assets-exemplaar.

1. Navigeer naar **[!UICONTROL Assets > Files]** en zoek de map met Help waarin u naar Brand Portal wilt publiceren.
1. Selecteer een map met bijdragen en klik op **[!UICONTROL Quick Publish]** > **[!UICONTROL Publish to Brand Portal]** .

   ![](assets/publish-contribution-folder-to-bp.png)

   U ontvangt een succesbericht nadat de map met bijdragen naar Brand Portal is gepubliceerd.

Er wordt een e-mail-/pulsmelding verzonden naar de Brand Portal-gebruikers die zijn toegewezen aan de bijdragemap. De Brand Portal-gebruikers hebben toegang tot de map met bijdragen en kunnen een bijdrage starten. Zie, [&#x200B; activa aan de bijdrageomslag uploaden en aan Experience Manager Assets &#x200B;](brand-portal-publish-contribution-folder-to-aem-assets.md) publiceren.
