---
title: Mappen delen
description: Brand Portal vereist dat elementen worden gepubliceerd vanuit een vooraf geconfigureerde Experience Manager Assets Author-instantie. De gebruikers niet-admin kunnen tot gepubliceerde activa slechts toegang hebben indien gevormd tijdens replicatie opstelling met Experience Manager, en de activa moeten met hen worden gedeeld.
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: d28cf927-60e8-437e-9cba-92f7e19020e7
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1035'
ht-degree: 0%

---

# Mappen delen op Brand Portal {#share-folders}

Assets moet naar Brand Portal worden gepubliceerd vanuit een vooraf geconfigureerde Experience Manager Author-instantie, aangezien Brand Portal het opnemen van elementen niet ondersteunt.

## Workflow voor het delen van mappen in Brand Portal {#folder-sharing-workflow-in-brand-portal}

Hieronder worden de workflow voor het delen van mappen en gebruikerstoegang beschreven:

* Standaard zijn alle mappen die vanuit Experience Manager Assets naar Brand Portal worden gepubliceerd, alleen zichtbaar voor de Brand Portal Administrator, tenzij ze als public zijn gemarkeerd tijdens het configureren van de replicatie.
* De beheerder gebruikt de **[!UICONTROL Folder Properties]** -console om een map te delen met selectieve gebruikers of groepen. Alleen de gebruikers of groepen met wie de map wordt gedeeld, kunnen de map zien nadat ze zich hebben aangemeld bij Brand Portal. De map is niet zichtbaar voor andere gebruikers.
* De beheerder kan een map ook openbaar maken via het selectievakje **[!UICONTROL Public Folder]** in de **[!UICONTROL Folder Properties]** -console. Alle gebruikers zien een openbare map.

* Ongeacht gebruikersrollen en rechten, zien gebruikers die zich aanmelden bij Brand Portal, alle openbare mappen en de mappen die rechtstreeks met hen of met een groep waartoe zij behoren worden gedeeld. Privémappen of mappen die met andere gebruikers worden gedeeld, zijn niet voor alle gebruikers zichtbaar.

### Mappen delen met gebruikersgroepen op Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

Toegangsrechten voor elementen van een map zijn afhankelijk van de toegangsrechten voor de bovenliggende map, ongeacht de instellingen van onderliggende mappen. [ ACLs ](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/security/security) in AEM dit gedrag, met kindomslagen die ACLs van hun ouderomslagen erven. Stel dat map A map B bevat, die map C bevat. Dan heeft een gebruikersgroep (of gebruikers) die toegangsrechten op omslag A hebben ook de zelfde toegangsrechten op omslag B en omslag C. De omslag B die de kindomslag van A zijn ACLs erft, en de omslag C die de kindomslag van B zijn ACLs erft.

Op dezelfde manier hebben gebruikersgroepen (of gebruikers) die alleen toegang hebben tot map B dezelfde toegangsmachtigingen voor map C, maar niet voor map A. Adobe raadt aan inhoud te ordenen zodat de meest kwetsbare elementen in onderliggende mappen worden geplaatst, zodat de toegang kan worden beperkt van de onderliggende mappen tot de hoofdmap.

### Openbare map publiceren {#public-folder-publish}

Niet-beheergebruikers (zoals Editors en Viewers) hebben alleen toegang tot elementen die vanuit AEM Assets naar Brand Portal zijn gepubliceerd als de optie **[!UICONTROL Public Folder Publish]** is geselecteerd tijdens de Brand Portal-replicatieconfiguratie.

![](assets/assetbpreplication.png)

Als de optie **[!UICONTROL Public Folder Publish]** is uitgeschakeld, moeten beheerders deze elementen specifiek delen met gebruikers die geen beheerder zijn, met behulp van de deelfunctie.

>[!NOTE]
>
>De optie om **[!UICONTROL Public Folder Publish]** in te schakelen is beschikbaar in AEM 6.3.2.1 en hoger.

## Toegang tot gedeelde mappen {#access-to-shared-folders}

In de volgende matrix worden de toegangsrechten en rechten voor het delen of opheffen van elementen voor verschillende gebruikersrollen besproken:

|               | Toegang tot alle mappen die vanuit AEM Assets naar Brand Portal zijn gepubliceerd | Toegang tot gedeelde mappen | Maprechten delen of niet delen |
|---------------|-----------|-----------|------------|
| Beheerder | Ja | Ja | Ja |
| Editor | Nee* | Ja, alleen indien gedeeld met hen of met de groep waartoe zij behoren | Ja, alleen voor de mappen die met hen worden gedeeld of met de groep waartoe zij behoren |
| Viewer | Nee* | Ja, alleen indien gedeeld met hen of met de groep waartoe zij behoren | Nee |
| Gastgebruiker | Nee* | Ja, alleen indien gedeeld met hen of met de groep waartoe zij behoren | Nee |

>[!NOTE]
>
>Standaard is de optie **[!UICONTROL Public Folder Publish]** uitgeschakeld tijdens het configureren van replicatie van Brand Portal met AEM auteur. Als deze optie is ingeschakeld, zijn de mappen die naar Brand Portal worden gepubliceerd standaard toegankelijk voor alle gebruikers (ook niet-beheerders).

### Toegang van gebruikers die geen beheerder zijn tot gedeelde mappen {#non-admin-user-access-to-shared-folders}

Gebruikers die geen beheerder zijn, hebben alleen toegang tot de mappen die met hen worden gedeeld op Brand Portal. Hoe deze mappen echter worden weergegeven op het portaal wanneer ze zich aanmelden, is afhankelijk van de instellingen van de **[!UICONTROL Enable Folder Hierarchy]** -configuratie.

**als de configuratie gehandicapt** is

Gebruikers die geen beheerder zijn, kunnen alle mappen zien die met hen worden gedeeld op de bestemmingspagina en zich aanmelden bij de Brand Portal.

![](assets/disabled-folder-hierarchy1-1.png)

**als de configuratie** wordt toegelaten

Gebruikers die geen beheerder zijn, zien de mappenstructuur (te beginnen met de hoofdmap) en de gedeelde mappen die in hun respectieve bovenliggende mappen zijn gerangschikt bij het aanmelden bij de Brand Portal.

Deze bovenliggende mappen zijn virtuele mappen en er kunnen geen handelingen op worden uitgevoerd. U kunt deze virtuele mappen herkennen met een vergrendelingspictogram.

In tegenstelling tot de gedeelde mappen zijn er geen actietaken zichtbaar wanneer u deze in **[!UICONTROL Card View]** aanwijst of selecteert. De knop **[!UICONTROL Overview]** wordt weergegeven bij het selecteren van een virtuele map in **[!UICONTROL Column View]** en **[!UICONTROL List View]** .

>[!NOTE]
>
>De standaardminiatuur van de virtuele mappen is de miniatuurafbeelding van de eerste gedeelde map.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Mappen delen {#how-to-share-folders}

Ga als volgt te werk als u een map wilt delen met gebruikers op Brand Portal:

1. Klik op het bedekkingspictogram aan de linkerkant en kies **[!UICONTROL Navigation]** .

   ![](assets/selectorrail.png)

1. Selecteer **[!UICONTROL Files]** in de zijbalk aan de linkerkant.

   ![](assets/access_files.png)

1. Selecteer in de Brand Portal-interface de map die u wilt delen.

   ![](assets/share-folders.png)

1. Selecteer **[!UICONTROL Share]** in de werkbalk boven in het scherm.

   ![](assets/share_icon.png)

   De [!UICONTROL Folder Properties] -console wordt weergegeven.

   ![](assets/folder_properties.png)

1. Geef in de **[!UICONTROL Folder Properties]** -console de maptitel op in het veld **[!UICONTROL Folder Title]** als u niet wilt dat de standaardnaam wordt weergegeven aan gebruikers.
1. Selecteer in de lijst **[!UICONTROL Add User]** de gebruikers of groepen waarmee u de map wilt delen en klik op **[!UICONTROL Add]** .
Als u de map alleen met gastgebruikers en geen andere gebruikers wilt delen, selecteert u **[!UICONTROL Anonymous Users]** in de vervolgkeuzelijst **[!UICONTROL Members]** .

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Als u de map beschikbaar wilt maken voor alle gebruikers, ongeacht hun groepslidmaatschap en rol, schakelt u het selectievakje **[!UICONTROL Public Folder]** in om deze openbaar te maken.

1. Klik indien nodig op **[!UICONTROL Change Thumbnail]** om de miniatuurafbeelding voor de map te wijzigen.
1. Klik op **[!UICONTROL Save]**.

1. Als u toegang wilt tot de gedeelde map, meldt u zich aan bij Brand Portal met de referenties van de gebruiker met wie u de map hebt gedeeld. Controleer de gedeelde map in de interface.

## Mappen delen ongedaan maken {#unshare-the-folders}

Voer de volgende stappen uit om het delen van een eerder gedeelde map op te heffen:

1. Selecteer in de Brand Portal-interface de map waarvan u het delen wilt opheffen.

   ![](assets/share-folders-1.png)

1. Klik in de werkbalk boven in het scherm op **[!UICONTROL Share]** .
1. Klik in de **[!UICONTROL Folder Properties]** -console onder **[!UICONTROL Members]** op het **[!UICONTROL x]** -symbool naast een gebruiker om deze te verwijderen uit de lijst met gebruikers waarmee u de map hebt gedeeld.

   ![](assets/folder_propertiesunshare.png)

1. Klik in het waarschuwingsbericht op **[!UICONTROL Confirm]** om te bevestigen dat u het document niet deelt.
Klik op **[!UICONTROL Save]**.

1. Meld u aan bij Brand Portal met de gegevens van de gebruiker die u uit de gedeelde lijst hebt verwijderd. De map is niet meer beschikbaar in de Brand Portal-interface voor de gebruiker.
