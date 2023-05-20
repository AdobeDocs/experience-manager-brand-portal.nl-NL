---
title: Een verzameling delen
seo-title: Share a collection
description: Experience Manager Assets Brand Portal-beheerders kunnen een verzameling of een slimme verzameling delen en het delen ervan opheffen met geautoriseerde gebruikers. Editors kunnen alleen de verzamelingen weergeven en delen die door hen zijn gemaakt, met hen zijn gedeeld en openbare verzamelingen.
seo-description: Experience Manager Assets Brand Portal Administrators can share and unshare a collection or a smart collection with authorized users. Editors can view and share only the collections created by them, shared with them, and public collections.
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: Vishabh Gupta
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
exl-id: 29b877f6-4200-4299-9b8d-81d88f4e8221
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# Verzamelingen delen {#share-collections}

Een verzameling vertegenwoordigt een groep gerelateerde elementen die samen in Adobe Experience Manager Assets Brand Portal zijn opgeslagen. De gebruikers kunnen slimme verzamelingen maken door [zoeken naar informatie of facetten toepassen om verwante elementen te filteren](brand-portal-searching.md) en samen opslaan voor eenvoudige toegang en deze verder delen met andere Brand Portal-gebruikers.

De beheerders kunnen een inzameling met de erkende gebruikers van Brand Portal delen en delen. Editors en viewers kunnen de verzamelingen die door hen zijn gemaakt, met hen worden gedeeld en openbare verzamelingen weergeven en delen.

>[!NOTE]
>
>Editors kunnen een openbare collectie niet veranderen in een niet-openbare collectie en hebben daarom niet de **[!UICONTROL Public Collection]** selectievakje beschikbaar in **[!UICONTROL Collection Settings]** .

## Een verzameling delen {#share-collection}

Hier volgen de stappen voor het delen van een verzameling met geautoriseerde Brand Portal-gebruikers:

1. Meld u aan bij uw Brand Portal-huurder. Standaard worden de **[!UICONTROL Files]** wordt geopend met alle gepubliceerde elementen en mappen.

1. Van de snelle navigatie op de bovenkant, klik **[!UICONTROL Collections]**.

1. Van de **[!UICONTROL Collections]** Voer een van de volgende handelingen uit:

   * Houd de aanwijzer boven de verzameling die u wilt delen. Klik in de snelactieminiaturen die beschikbaar zijn voor de verzameling op de knop **[!UICONTROL Settings]** pictogram.

      ![](assets/settings-icon.png)

   * Selecteer de verzameling die u wilt delen. Van de toolbar bij de bovenkant, klik **[!UICONTROL Settings]**.

      ![](assets/collection-console.png)

1. In de **[!UICONTROL Collection Settings]** selecteert u de gebruikers met wie u de verzameling wilt delen en selecteert u de rol die de gebruiker aan de algemene rol moet toewijzen. Wijs bijvoorbeeld de rol Editor toe aan een algemene editor, de rol Viewer, aan een algemene viewer.

   Als u de verzameling ook beschikbaar wilt maken voor alle gebruikers, ongeacht hun groepslidmaatschap en rol, maakt u deze openbaar door de **[!UICONTROL Public Collection]** selectievakje.

   >[!NOTE]
   >
   >Nochtans, kunnen niet-admin gebruikers van het creëren van openbare inzamelingen worden beperkt, om het hebben van talrijke openbare inzamelingen te vermijden zodat systeemruimte kan worden bewaard. Organisaties kunnen de **[!UICONTROL Allow public collections creation]** configuratie van **[!UICONTROL General]** instellingen beschikbaar in het deelvenster met beheergereedschappen.

   ![](assets/collection_sharingadduser.png)

   De editors kunnen een openbare collectie niet wijzigen in een niet-openbare collectie en hebben daarom geen **[!UICONTROL Public Collection]** selectievakje beschikbaar in **[!UICONTROL Collection Settings]** .

   ![](assets/collection-setting-editor.png)

1. Klik op de knop **[!UICONTROL Add]** om de gebruiker toe te voegen, en klik dan **[!UICONTROL Save]**. De verzameling wordt gedeeld met de gebruikers.

   >[!NOTE]
   >
   >De rol van een gebruiker bepaalt de toegang tot de elementen en mappen in een verzameling. Als een gebruiker geen toegang heeft tot elementen, wordt een lege verzameling gedeeld met de gebruiker. De rol van een gebruiker bepaalt ook de acties die beschikbaar zijn voor verzamelingen.

## Delen van een verzameling opheffen {#unshare-a-collection}

Ga als volgt te werk om het delen van een eerder gedeelde verzameling op te heffen:

1. Van de **[!UICONTROL Collections]** -console, selecteert u de verzameling waarvan u het delen wilt opheffen.

   Van de toolbar bij de bovenkant, klik **[!UICONTROL Settings]**.

   ![](assets/collection_settings.png)

1. In de **[!UICONTROL Collection Settings]** onder de **[!UICONTROL Members]** klikt u op de **[!UICONTROL x]** symbool naast gebruikers om hen uit de lijst van gebruikers te verwijderen die tot de inzameling toegang hebben.

   ![](assets/unshare_collection.png)

1. Er verschijnt een waarschuwingsbericht. Klikken **[!UICONTROL Confirm]** om het delen van de verzameling op te heffen.

1. Klikken **[!UICONTROL Save]** om de wijzigingen toe te passen.

   Wanneer de gebruiker uit de gedeelde lijst is verwijderd, wordt de niet-gedeelde verzameling verwijderd uit de **[!UICONTROL Collections]** console.

<!--
1. Click the overlay icon on the left, and choose **[!UICONTROL Navigation]**.

   ![](assets/contenttree-1.png)

1. From the siderail on the left, click **[!UICONTROL Collections]**.

   ![](assets/access_collections.png)

1. From the **[!UICONTROL Collections]** console, do one of the following:

    * Hover the pointer over the collection you want to share. From the quick action thumbnails available for the collection, click the **[!UICONTROL Settings]** icon.

   ![](assets/settings_thumbnail.png)

    * Select the collection you want to share. From the toolbar at the top, click **[!UICONTROL Settings]**.
    
   ![](assets/collection-sharing.png)

1. In the [!UICONTROL Collection Settings] dialog box, select the users or groups with whom you want to share the collection and select the role for a user or a group to match their global role. For example, assign the Editor role to a global editor, the Viewer role to a global viewer.

   Alternatively, to make the collection available to all users irrespective of their group membership and role, make it public by selecting the **[!UICONTROL Public Collection]** check-box.

   >[!NOTE]
   >
   >However, non-admin users can be restricted from creating public collections, to avoid having numerous public collections so that system space can be saved. Organizations can disable the **[!UICONTROL Allow public collections creation]** configuration from [!UICONTROL General] settings available in admin tools panel.

   ![](assets/collection_sharingadduser.png)

   Editors cannot change a public collection to a non-public collection and, therefore, do not have **[!UICONTROL Public Collection]** check-box available in **[!UICONTROL Collection Settings]** dialog.

   ![](assets/collection-setting-editor.png)

1. Select **[!UICONTROL Add]**, and then **[!UICONTROL Save]**. The collection is shared with the chosen users.

   >[!NOTE]
   >
   >A user's role governs access to the assets and folders inside a collection. If a user does not have access to assets, an empty collection is shared with the user. Also, a user's role governs the actions available for collections.

## Unshare a collection {#unshare-a-collection}

To unshare a previously shared collection, do the following:

1. From the **[!UICONTROL Collections]** console, select the collection you want to unshare.

   In the toolbar, click **[!UICONTROL Settings]**.

   ![](assets/collection_settings.png)

1. On the **[!UICONTROL Collection Settings]** dialog box, under **[!UICONTROL Members]**, click the **[!UICONTROL x]** symbol next to users or groups to remove them from the list of users you shared the collection with.

   ![](assets/unshare_collection.png)

1. In the warning message box, click **[!UICONTROL Confirm]** to confirm unshare.

   Click **[!UICONTROL Save]**.

1. Log in to Brand Portal with the credentials of the user you removed from the shared list. The collection is removed from the **[!UICONTROL Collections]** console.
-->
