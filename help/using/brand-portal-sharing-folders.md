---
title: Mappen delen
seo-title: Share folders
description: Brand Portal biedt geen ondersteuning voor het opnemen van bedrijfsmiddelen, zodat middelen vanuit een vooraf geconfigureerde Experience Manager Assets Author-instantie naar Brand Portal moeten worden gepubliceerd. Gepubliceerde elementen zijn niet toegankelijk voor gebruikers die geen beheerder zijn van Brand Portal, tenzij dit is geconfigureerd tijdens het configureren van replicatie met een Experience Manager-instantie, en moeten met hen worden gedeeld.
seo-description: Brand Portal does not support asset ingestion so assets must be published to Brand Portal from a pre-configured Experience Manager Assets Author instance. Published assets are not accessible to non-admin users of Brand Portal, unless configured while configuring replication with Experience Manager instance, and need to be shared with them.
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
exl-id: d28cf927-60e8-437e-9cba-92f7e19020e7
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1054'
ht-degree: 0%

---

# Mappen delen op Brand Portal {#share-folders}

Elementen moeten vanuit een vooraf geconfigureerde instantie van Auteur van Experience Manager naar Brand Portal worden gepubliceerd, omdat Brand Portal het opnemen van elementen niet ondersteunt.

## Workflow voor het delen van mappen in Brand Portal {#folder-sharing-workflow-in-brand-portal}

Hieronder worden de workflow voor het delen van mappen en gebruikerstoegang beschreven:

* Standaard zijn alle mappen die vanuit Experience Manager Assets naar Brand Portal worden gepubliceerd, alleen zichtbaar voor de Brand Portal Administrator, tenzij ze als public zijn gemarkeerd tijdens het configureren van de replicatie.
* De beheerder gebruikt de **[!UICONTROL Folder Properties]** console om een omslag met selectieve gebruikers of groepen te delen. Alleen de gebruikers of groepen met wie de map wordt gedeeld, kunnen de map zien nadat ze zich hebben aangemeld bij Brand Portal. De map is niet zichtbaar voor andere gebruikers.
* De beheerder kan er ook voor kiezen een map openbaar te maken via de **[!UICONTROL Public Folder]** selectievakje in de **[!UICONTROL Folder Properties]** console. Alle gebruikers zien een openbare map.

* Wanneer gebruikers zich aanmelden bij Brand Portal, zien ze, ongeacht gebruikersrollen en bevoegdheden, alle openbare mappen en de mappen die rechtstreeks met hen of met een groep waartoe zij behoren worden gedeeld. Privémappen of mappen die met andere gebruikers worden gedeeld, zijn niet voor alle gebruikers zichtbaar.

### Mappen delen met gebruikersgroepen op Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

Toegangsrechten voor elementen van een map zijn afhankelijk van de toegangsrechten voor de bovenliggende map, ongeacht de instellingen van onderliggende mappen. Dit gedrag wordt bepaald door [ACLs](https://experienceleague.adobe.com/docs/experience-manager-65/administering/security/security.html) in AEM, aangezien de kindomslagen ACLs van hun ouderomslagen erven. Bijvoorbeeld, als een omslag A omslag B bevat die omslag C bevat, dan hebben een gebruikersgroep (of gebruikers) die toegangsrechten op omslag A hebben ook de zelfde toegangsrechten op omslag B en omslag C. De omslag B die de kindomslag van A is overerft ACLs, en de omslag C die de kindomslag van B overerft ACLs.

Op dezelfde manier hebben gebruikersgroepen (of gebruikers) met toegangsmachtigingen voor alleen map B dezelfde toegangsmachtigingen voor map C, maar niet voor map A. Daarom wordt geadviseerd dat de organisaties hun inhoud zodanig schikken dat de meeste blootgestelde activa in de kindomslag en van kinderen aan de toegang van de wortelomslag kunnen worden beperkt.

### Openbare map publiceren {#public-folder-publish}

Tenzij **[!UICONTROL Public Folder Publish]** is geselecteerd tijdens het configureren van Brand Portal-replicatie, hebben gebruikers die geen beheerder zijn (zoals Editors en Viewers) geen toegang tot de middelen die vanuit AEM Assets naar Brand Portal zijn gepubliceerd.

![](assets/assetbpreplication.png)

Als de **[!UICONTROL Public Folder Publish]** Als deze optie is uitgeschakeld, moeten beheerders deze middelen specifiek delen met gebruikers die geen beheerder zijn en gebruikmaken van de mogelijkheid om te delen.

>[!NOTE]
>
>De optie om in te schakelen **[!UICONTROL Public Folder Publish]** is beschikbaar in AEM 6.3.2.1.

## Toegang tot gedeelde mappen {#access-to-shared-folders}

In de volgende matrix worden de toegangsrechten en rechten voor het delen/ontdelen van elementen voor verschillende gebruikersrollen besproken:

|  | Toegang tot alle mappen die vanuit AEM Assets naar Brand Portal zijn gepubliceerd | Toegang tot gedeelde mappen | Maprechten delen/delen opheffen |
|---------------|-----------|-----------|------------|
| Beheerder | Ja | Ja | Ja |
| Editor | Nee* | Ja, alleen indien gedeeld met hen of met de groep waartoe zij behoren | Ja, alleen voor de mappen die met hen worden gedeeld of met de groep waartoe zij behoren |
| Viewer | Nee* | Ja, alleen indien gedeeld met hen of met de groep waartoe zij behoren | Nee |
| Gastgebruiker | Nee* | Ja, alleen indien gedeeld met hen of met de groep waartoe zij behoren | Nee |

>[!NOTE]
>
>Standaard worden de **[!UICONTROL Public Folder Publish]** is uitgeschakeld tijdens het configureren van replicatie van Brand Portal met AEM Author. Als deze optie is ingeschakeld, zijn de mappen die naar Brand Portal worden gepubliceerd standaard toegankelijk voor alle gebruikers (ook niet-beheerders).

### Toegang van gebruikers die geen beheerder zijn tot gedeelde mappen {#non-admin-user-access-to-shared-folders}

Gebruikers die geen beheerder zijn, hebben alleen toegang tot de mappen die met hen worden gedeeld op Brand Portal. Hoe deze mappen echter op het portaal worden weergegeven wanneer ze zich aanmelden, is afhankelijk van de instellingen van **[!UICONTROL Enable Folder Hierarchy]** configuratie.

**Als de configuratie is uitgeschakeld**

Niet-beheerders zien alle mappen die met hen worden gedeeld op de bestemmingspagina, bij het aanmelden bij de Brand Portal.

![](assets/disabled-folder-hierarchy1-1.png)

**Als de configuratie is ingeschakeld**

Gebruikers die geen beheerder zijn, zien de mappenstructuur (te beginnen met de hoofdmap) en de gedeelde mappen die in hun respectieve bovenliggende mappen zijn gerangschikt bij het aanmelden bij de Brand Portal.

Deze bovenliggende mappen zijn de virtuele mappen en er kunnen geen handelingen op worden uitgevoerd. U kunt deze virtuele mappen herkennen met een vergrendelingspictogram.

Er zijn geen actietaken zichtbaar bij het aanwijzen of selecteren van de taken in **[!UICONTROL Card View]**, in tegenstelling tot de gedeelde mappen. **[!UICONTROL Overview]** wordt weergegeven wanneer u een virtuele map selecteert in **[!UICONTROL Column View]** en **[!UICONTROL List View]**.

>[!NOTE]
>
>De standaardminiatuur van de virtuele mappen is de miniatuurafbeelding van de eerste gedeelde map.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Mappen delen {#how-to-share-folders}

Ga als volgt te werk als u een map wilt delen met gebruikers op Brand Portal:

1. Klik op het bedekkingspictogram aan de linkerkant en kies **[!UICONTROL Navigation]**.

   ![](assets/selectorrail.png)

1. Selecteer in de zijbalk aan de linkerkant de optie **[!UICONTROL Files]**.

   ![](assets/access_files.png)

1. Selecteer in de Brand Portal-interface de map die u wilt delen.

   ![](assets/share-folders.png)

1. Selecteer in de werkbalk bovenaan de optie **[!UICONTROL Share]**.

   ![](assets/share_icon.png)

   De [!UICONTROL Folder Properties] wordt weergegeven.

   ![](assets/folder_properties.png)

1. In de **[!UICONTROL Folder Properties]** console, specificeer de omslagtitel in **[!UICONTROL Folder Title]** als u niet wilt dat de standaardnaam aan gebruikers wordt weergegeven.
1. Van de **[!UICONTROL Add User]** selecteert u de gebruikers of groepen waarmee u de map wilt delen en klikt u op **[!UICONTROL Add]**.
Als u de map alleen met gastgebruikers en geen andere gebruikers wilt delen, selecteert u **[!UICONTROL Anonymous Users]** van de **[!UICONTROL Members]** vervolgkeuzelijst.

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Als u de map beschikbaar wilt maken voor alle gebruikers, ongeacht hun groepslidmaatschap en rol, maakt u deze openbaar door de optie **[!UICONTROL Public Folder]** selectievakje.

1. Klik indien nodig op **[!UICONTROL Change Thumbnail]** om de miniatuurafbeelding voor de map te wijzigen.
1. Klik op **[!UICONTROL Save]**.

1. Als u toegang wilt tot de gedeelde map, meldt u zich aan bij Brand Portal met de referenties van de gebruiker met wie u de map hebt gedeeld. Controleer de gedeelde map in de interface.

## Mappen delen ongedaan maken {#unshare-the-folders}

Voer de volgende stappen uit om het delen van een eerder gedeelde map op te heffen:

1. Selecteer in de Brand Portal-interface de map waarvan u het delen wilt opheffen.

   ![](assets/share-folders-1.png)

1. Van de toolbar bij de bovenkant, klik **[!UICONTROL Share]**.
1. In de **[!UICONTROL Folder Properties]** console, onder **[!UICONTROL Members]** klikt u op de knop **[!UICONTROL x]** symbool naast een gebruiker om deze te verwijderen uit de lijst met gebruikers waarmee u de map hebt gedeeld.

   ![](assets/folder_propertiesunshare.png)

1. Klik in het waarschuwingsbericht op **[!UICONTROL Confirm]** om te bevestigen dat u niet deelt.
Klik op **[!UICONTROL Save]**.

1. Meld u aan bij Brand Portal met de gegevens van de gebruiker die u uit de gedeelde lijst hebt verwijderd. De map is niet meer beschikbaar in de Brand Portal-interface voor de gebruiker.
