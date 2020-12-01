---
title: Mappen delen
seo-title: Mappen delen
description: Brand Portal biedt geen ondersteuning voor het opnemen van bedrijfsmiddelen, zodat bedrijfsmiddelen via een vooraf geconfigureerde AEM-auteur naar Brand Portal moeten worden gepubliceerd. Gepubliceerde middelen zijn niet toegankelijk voor niet-admingebruikers van het Portaal van het Merk, tenzij gevormd terwijl het vormen van replicatie met AEM instantie, en moeten met hen worden gedeeld.
seo-description: Brand Portal biedt geen ondersteuning voor het opnemen van bedrijfsmiddelen, zodat bedrijfsmiddelen via een vooraf geconfigureerde AEM-auteur naar Brand Portal moeten worden gepubliceerd. Gepubliceerde middelen zijn niet toegankelijk voor niet-admingebruikers van het Portaal van het Merk, tenzij gevormd terwijl het vormen van replicatie met AEM instantie, en moeten met hen worden gedeeld.
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
translation-type: tm+mt
source-git-commit: 0ae9860e2b6beb96f53e92bb114bb5756e371ad6
workflow-type: tm+mt
source-wordcount: '1099'
ht-degree: 0%

---


# Mappen delen op Brand Portal {#share-folders}

Middelen moeten via een vooraf geconfigureerde AEM Author-instantie naar Brand Portal worden gepubliceerd, omdat het Brand Portal geen ondersteuning biedt voor het opnemen van bedrijfsmiddelen.

## Workflow voor het delen van mappen in Brand Portal {#folder-sharing-workflow-in-brand-portal}

Hieronder worden de workflow voor het delen van mappen en gebruikerstoegang beschreven:

* Door gebrek, zijn alle omslagen die van AEM Assets aan het Portaal van het Merk worden gepubliceerd zichtbaar slechts aan de Beheerder van het Portaal van het Merk, tenzij duidelijk als openbaar terwijl het vormen van replicatie.
* De beheerder gebruikt de **[!UICONTROL Folder Properties]** console om een omslag met selectieve gebruikers of groepen te delen. Alleen die gebruikers of groepen met wie de map wordt gedeeld, kunnen de map zien nadat ze zich hebben aangemeld bij Brand Portal. De map is niet zichtbaar voor andere gebruikers.
* De beheerder kan er ook voor kiezen een map openbaar te maken via het selectievakje **[!UICONTROL Public Folder]** in de console **[!UICONTROL Folder Properties]**. Alle gebruikers zien een openbare map.

* Ongeacht gebruikersrollen en voorrechten, wanneer de gebruikers login aan het Portaal van het Merk, zien zij alle openbare omslagen, en de omslagen die direct met hen of met een groep worden gedeeld waartoe zij behoren. Privémappen of mappen die met andere gebruikers worden gedeeld, zijn niet voor alle gebruikers zichtbaar.

### Mappen delen met gebruikersgroepen op Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

Toegangsrechten voor elementen van een map zijn afhankelijk van de toegangsrechten voor de bovenliggende map, ongeacht de instellingen van onderliggende mappen. Dit gedrag wordt geregeerd door [ACLs](https://helpx.adobe.com/experience-manager/6-5/sites/administering/using/security.html#PermissionsinAEM) in AEM, aangezien de kindomslagen ACLs van hun ouderomslagen erven. Bijvoorbeeld, als een omslag A omslag B bevat die omslag C bevat, dan hebben een gebruikersgroep (of gebruikers) die toegangsrechten op omslag A hebben ook de zelfde toegangsrechten op omslag B en omslag C. De omslag B die de kindomslag van A is overerft ACLs, en de omslag C die de kindomslag van B overerft ACLs.

Op dezelfde manier hebben gebruikersgroepen (of gebruikers) met toegangsmachtigingen voor alleen map B dezelfde toegangsmachtigingen voor map C, maar niet voor map A. Daarom wordt geadviseerd dat de organisaties hun inhoud zodanig schikken dat de meeste blootgestelde activa in de kindomslag en van kinderen aan de toegang van de wortelomslag kunnen worden beperkt.

### Openbare map publiceren {#public-folder-publish}

Tenzij de optie **[!UICONTROL Public Folder Publish]** is geselecteerd tijdens het configureren van de replicatie van het Brand Portal, hebben gebruikers zonder beheerdersrechten (zoals Editors en Viewers) geen toegang tot de middelen die van AEM Assets naar Brand Portal zijn gepubliceerd.

![](assets/assetbpreplication.png)

Als de optie **[!UICONTROL Public Folder Publish]** is uitgeschakeld, moeten beheerders deze elementen specifiek delen met gebruikers die geen beheerder zijn en gebruikmaken van de mogelijkheid om bestanden te delen.

>[!NOTE]
>
>De optie om **[!UICONTROL Public Folder Publish]** in te schakelen is beschikbaar in AEM 6.3.2.1 vanaf.

## Toegang tot gedeelde mappen {#access-to-shared-folders}

In de volgende matrix worden de toegangsrechten en rechten voor het delen/ontdelen van elementen voor verschillende gebruikersrollen besproken:

|  | Toegang tot alle mappen die van AEM Assets naar Brand Portal zijn gepubliceerd | Toegang tot gedeelde mappen | Maprechten delen/delen opheffen |
|---------------|-----------|-----------|------------|
| Beheerder | Ja | Ja | Ja |
| Editor | Nee* | Ja, alleen indien gedeeld met hen of met de groep waartoe zij behoren | Ja, alleen voor de mappen die met hen worden gedeeld of met de groep waartoe zij behoren |
| Viewer | Nee* | Ja, alleen indien gedeeld met hen of met de groep waartoe zij behoren | Nee |
| Gastgebruiker | Nee* | Ja, alleen indien gedeeld met hen of met de groep waartoe zij behoren | Nee |

>[!NOTE]
>
>Standaard is de optie **[!UICONTROL Public Folder Publish]** uitgeschakeld tijdens het configureren van replicatie van Brand Portal met AEM-auteur. Als de optie is ingeschakeld, zijn de mappen die naar het Brand Portal worden gepubliceerd standaard toegankelijk voor alle gebruikers (ook niet-beheerders).

### Toegang van gebruikers die geen beheerder zijn tot gedeelde mappen {#non-admin-user-access-to-shared-folders}

Gebruikers die geen beheerder zijn, hebben alleen toegang tot de mappen die met hen worden gedeeld op Brand Portal. Hoe deze mappen echter op het portaal worden weergegeven wanneer deze zich aanmelden, is afhankelijk van de instellingen van de configuratie **[!UICONTROL Enable Folder Hierarchy]**.

**Als de configuratie is uitgeschakeld**

Niet-admin-gebruikers zien alle mappen die met hen worden gedeeld op de bestemmingspagina, bij het aanmelden bij het Brand Portal.

![](assets/disabled-folder-hierarchy1-1.png)

**Als de configuratie is ingeschakeld**

Gebruikers die geen beheerder zijn, zien de mapstructuur (te beginnen met de hoofdmap) en de gedeelde mappen die in hun respectieve bovenliggende mappen zijn gerangschikt, bij het aanmelden bij de Brand Portal.

Deze bovenliggende mappen zijn de virtuele mappen en er kunnen geen handelingen op worden uitgevoerd. U kunt deze virtuele mappen herkennen met een vergrendelingspictogram.

In tegenstelling tot de gedeelde mappen zijn er geen actietaken zichtbaar bij het aanwijzen of selecteren van deze taken in **[!UICONTROL Card View]**. **[!UICONTROL Overview]** wordt weergegeven bij het selecteren van een virtuele map in  **[!UICONTROL Column View]** en  **[!UICONTROL List View]**.

>[!NOTE]
>
>De standaardminiatuur van de virtuele mappen is de miniatuurafbeelding van de eerste gedeelde map.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Mappen {#how-to-share-folders} delen

Ga als volgt te werk als u een map wilt delen met gebruikers op Brand Portal:

1. Klik op het bedekkingspictogram aan de linkerkant en kies **[!UICONTROL Navigation]**.

   ![](assets/selectorrail.png)

1. Selecteer **[!UICONTROL Files]** in de zijlijn aan de linkerkant.

   ![](assets/access_files.png)

1. Selecteer in de interface Brand Portal de map die u wilt delen.

   ![](assets/share-folders.png)

1. Selecteer **[!UICONTROL Share]** op de werkbalk boven in het scherm.

   ![](assets/share_icon.png)

   De [!UICONTROL Folder Properties] console verschijnt.

   ![](assets/folder_properties.png)

1. Geef in de **[!UICONTROL Folder Properties]**-console de maptitel op in het veld **[!UICONTROL Folder Title]** als u niet wilt dat de standaardnaam wordt weergegeven aan gebruikers.
1. Selecteer in de lijst **[!UICONTROL Add User]** de gebruikers of groepen waarmee u de map wilt delen en klik op **[!UICONTROL Add]**.
Als u de map alleen met gastgebruikers en geen andere gebruikers wilt delen, selecteert u **[!UICONTROL Anonymous Users]** in het vervolgkeuzemenu **[!UICONTROL Members]**.

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Als u de map beschikbaar wilt maken voor alle gebruikers, ongeacht hun groepslidmaatschap en rol, schakelt u het selectievakje **[!UICONTROL Public Folder]** in om deze openbaar te maken.

1. Klik zo nodig op **[!UICONTROL Change Thumbnail]** om de miniatuurafbeelding voor de map te wijzigen.
1. Klik op **[!UICONTROL Save]**.

1. Als u toegang wilt tot de gedeelde map, meldt u zich aan bij Brand Portal met de referenties van de gebruiker met wie u de map hebt gedeeld. Controleer de gedeelde map in de interface.

## Mappen {#unshare-the-folders} opheffen

Voer de volgende stappen uit om het delen van een eerder gedeelde map op te heffen:

1. Selecteer in de interface Brand Portal de map waarvan u het delen wilt opheffen.

   ![](assets/share-folders-1.png)

1. Klik op **[!UICONTROL Share]** op de werkbalk boven in het scherm.
1. Klik in de **[!UICONTROL Folder Properties]**-console onder **[!UICONTROL Members]** op het **[!UICONTROL x]**-symbool naast een gebruiker om deze te verwijderen uit de lijst met gebruikers waarmee u de map hebt gedeeld.

   ![](assets/folder_propertiesunshare.png)

1. Klik in het waarschuwingsbericht op **[!UICONTROL Confirm]** om het delen te bevestigen.
Klik op **[!UICONTROL Save]**.

1. Meld u aan bij Brand Portal met de referenties van de gebruiker die u uit de gedeelde lijst hebt verwijderd. De map is niet meer beschikbaar in de interface Brand Portal voor de gebruiker.
