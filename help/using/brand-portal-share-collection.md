---
title: Een verzameling delen
seo-title: Een verzameling delen
description: Beheerders van AEM Assets Brand Portal kunnen een verzameling of een slimme verzameling delen en delen met geautoriseerde gebruikers. Editors kunnen alleen de verzamelingen weergeven en delen die door hen zijn gemaakt, met hen zijn gedeeld en openbare verzamelingen.
seo-description: Beheerders van AEM Assets Brand Portal kunnen een verzameling of een slimme verzameling delen en delen met geautoriseerde gebruikers. Editors kunnen alleen de verzamelingen weergeven en delen die door hen zijn gemaakt, met hen zijn gedeeld en openbare verzamelingen.
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: Vishabh Gupta
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
translation-type: tm+mt
source-git-commit: a587061bc8afe250a88b4a02b42b6acd9ef6bbeb
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---


# Verzamelingen delen {#share-collections}

Een verzameling vertegenwoordigt een groep gerelateerde elementen die samen zijn opgeslagen in Adobe Experience Manager Assets Brand Portal. Gebruikers kunnen slimme verzamelingen maken door [zoekopdrachten in de vorm van zoekopdrachten of facetten toe te passen om gerelateerde elementen](brand-portal-searching.md) te filteren en ze samen op te slaan, zodat ze gemakkelijk toegankelijk zijn en ze verder kunnen delen met andere gebruikers van het Brand Portal.

De beheerders kunnen een inzameling met de erkende gebruikers van het Portaal van het Merk delen en unshare. Editors en viewers kunnen de verzamelingen die door hen zijn gemaakt, met hen worden gedeeld en openbare verzamelingen weergeven en delen.

>[!NOTE]
>
>Editors kunnen een openbare verzameling niet wijzigen in een verzameling die niet openbaar is en beschikken daarom niet over het **[!UICONTROL Public Collection]** selectievakje dat beschikbaar is in het **[!UICONTROL Collection Settings]** dialoogvenster.

## Een verzameling delen {#share-collection}

Hier volgen de stappen voor het delen van een verzameling met de geautoriseerde gebruikers van het Brand Portal:

1. Meld u aan bij uw Brand Portal-huurder. Standaard wordt de **[!UICONTROL Files]** weergave geopend met alle gepubliceerde elementen en mappen.

1. Klik op de snelle navigaties bovenaan **[!UICONTROL Collections]**.

1. Voer vanuit de **[!UICONTROL Collections]** console een van de volgende handelingen uit:

   * Houd de aanwijzer boven de verzameling die u wilt delen. Klik op het **[!UICONTROL Settings]** pictogram in de snelactieminiaturen die beschikbaar zijn voor de verzameling.

      ![](assets/settings-icon.png)

   * Selecteer de verzameling die u wilt delen. Klik op de werkbalk boven in het scherm **[!UICONTROL Settings]**.

      ![](assets/collection-console.png)

1. Selecteer in het **[!UICONTROL Collection Settings]** dialoogvenster de gebruikers met wie u de verzameling wilt delen en selecteer de rol die de gebruiker aan de algemene rol moet toekennen. Wijs bijvoorbeeld de rol Editor toe aan een algemene editor, de rol Viewer, aan een algemene viewer.

   U kunt de verzameling ook beschikbaar maken voor alle gebruikers, ongeacht hun groepslidmaatschap en rol, door het **[!UICONTROL Public Collection]** selectievakje in te schakelen.

   >[!NOTE]
   >
   >Nochtans, kunnen niet-admin gebruikers van het creëren van openbare inzamelingen worden beperkt, om het hebben van talrijke openbare inzamelingen te vermijden zodat systeemruimte kan worden bewaard. Organisaties kunnen de **[!UICONTROL Allow public collections creation]** configuratie uitschakelen op basis van de **[!UICONTROL General]** instellingen in het deelvenster met beheergereedschappen.

   ![](assets/collection_sharingadduser.png)

   De editors kunnen een openbare verzameling niet wijzigen in een niet-openbare verzameling en beschikken daarom niet over een **[!UICONTROL Public Collection]** selectievakje dat beschikbaar is in het **[!UICONTROL Collection Settings]** dialoogvenster.

   ![](assets/collection-setting-editor.png)

1. Klik op de **[!UICONTROL Add]** knop om de gebruiker toe te voegen en klik vervolgens **[!UICONTROL Save]**. De verzameling wordt gedeeld met de gebruikers.

   >[!NOTE]
   >
   >De rol van een gebruiker bepaalt de toegang tot de elementen en mappen in een verzameling. Als een gebruiker geen toegang heeft tot elementen, wordt een lege verzameling gedeeld met de gebruiker. De rol van een gebruiker bepaalt ook de acties die beschikbaar zijn voor verzamelingen.

## Delen van een verzameling opheffen {#unshare-a-collection}

Ga als volgt te werk om het delen van een eerder gedeelde verzameling op te heffen:

1. Selecteer in de **[!UICONTROL Collections]** console de verzameling waarvan u het delen wilt opheffen.

   Klik op de werkbalk boven in het scherm **[!UICONTROL Settings]**.

   ![](assets/collection_settings.png)

1. Klik in het **[!UICONTROL Collection Settings]** dialoogvenster onder de **[!UICONTROL Members]** sectie op het **[!UICONTROL x]** symbool naast gebruikers om deze te verwijderen uit de lijst met gebruikers die toegang hebben tot de verzameling.

   ![](assets/unshare_collection.png)

1. Er verschijnt een waarschuwingsbericht. Klik **[!UICONTROL Confirm]** om het delen van de verzameling op te heffen.

1. Klik **[!UICONTROL Save]** om de wijzigingen toe te passen.

   Zodra de gebruiker uit de gedeelde lijst wordt verwijderd, wordt de niet gedeelde inzameling verwijderd uit de **[!UICONTROL Collections]** console van de gebruiker.

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