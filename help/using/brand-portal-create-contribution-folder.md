---
title: Map voor bijdrage maken
seo-title: Map voor bijdrage maken
description: 'Krijg inzicht in hoe te om een bijdrageomslag in AEM Assets tot stand te brengen. '
seo-description: Krijg inzicht in hoe te om een bijdrageomslag in AEM Assets tot stand te brengen.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 92961850279ad5a676ec0bc655d3a16f0497b024
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---


# Map voor bijdragen maken {#create-contribution-folder}

AEM-beheerders en gebruikers die geen beheerder zijn, die toestemming hebben om een nieuwe map te maken, kunnen een **Contribute** -map in AEM Assets maken.
Als u een map **Contribution** wilt maken, maakt u een nieuwe map van het type **Asset Contribution**. Zo zorgt u ervoor dat de nieuwe map die u maakt, kan worden verzonden door gebruikers van Brand Portal.  Dit leidt automatisch tot een werkschema dat tot twee extra subomslagen, genoemd **GEDEELD** en **NIEUW**, binnen de pas gecreëerde omslag van de **Bijdrage** leidt.

**Een nieuwe map voor bijdragen maken:**
1. Meld u aan bij de instantie van uw AEM-auteurStandaard-URL: http:// localhost:4502/aem/start.html
1. Navigeer naar **[!UICONTROL Assets > Files]** Deze lijst bevat alle bestaande mappen in de gegevensopslagruimte AEM Assets.
1. Klik **[!UICONTROL Create]** om een nieuwe map te maken. Het pop-upvenster Map maken wordt geopend.
1. Voer **[!UICONTROL Title]** de map in, typ **[!UICONTROL Name]** de map en markeer het selectievakje **[!UICONTROL Asset Contribution]**.
U wordt aangeraden kleine alfabeten zonder spatie te gebruiken om de map een naam te geven.
1. Klik op **[!UICONTROL Create]**.
   ![](assets/create-contribution-folder.png)
1. U kunt de nieuwe bijdragemap zien in de opslagplaats van AEM Assets.
1. Klik om de map met bijdragen te openen. Er worden twee submappen **[!UICONTROL SHARED]** weergegeven en deze **[!UICONTROL NEW]** worden automatisch gemaakt in de map met bijdragen.\
   ![](assets/contribution-folder.png)

U kunt nu de eigenschappen van de map Contribution configureren. Zie [Eigenschappen](brand-portal-configure-contribution-folder-properties.md)voor Contribute-mappen configureren.

>[!NOTE]
>
>Een gebruiker die geen beheerder is, kan alleen een bronnenbijdragemap maken en delen. Wanneer de bijdragemap is gemaakt, kan een niet-beheerder deze niet wijzigen of verwijderen.
>
>Het nesten van de map voor middelenbijdragen wordt niet ondersteund. U kunt mappen voor meerdere bijdragen maken in een map, maar u mag geen bijdragemap maken in een andere bijdragemap.

