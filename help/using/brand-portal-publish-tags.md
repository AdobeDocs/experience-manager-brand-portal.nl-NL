---
title: Tags publiceren naar Brand Portal
seo-title: Tags publiceren naar Brand Portal
description: Leer hoe u tags kunt publiceren van AEM Assets naar Brand Portal.
seo-description: Leer hoe u tags kunt publiceren van AEM Assets naar Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 3%

---


# Tags publiceren naar Brand Portal {#publish-tags-to-brand-portal}

Leer hoe u tags kunt publiceren van AEM Assets naar Brand Portal.

Tags zijn handig voor het ordenen van elementen en het verbeteren van de doorzoekbaarheid van elementen waaraan ze zijn gekoppeld. Tags kunnen worden beschouwd als trefwoorden of labels (metagegevens) die zijn gekoppeld met elementen en waarmee elementen snel kunnen worden gevonden als resultaat van een zoekopdracht. Als u wilt weten hoe u tags aan elementen in AEM Assets wilt toewijzen, raadpleegt u [gebruikstags om elementen](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)te ordenen.

Tags (gekoppeld aan elementen en verzamelingen in AEM) worden automatisch naar Brand Portal gepubliceerd wanneer de elementen (en verzamelingen) met bijbehorende tags naar Brand Portal worden gepubliceerd. De gepubliceerde tags zijn handig om zoekopdrachten in staat te stellen de bijbehorende elementen te vinden.

>[!NOTE]
>
>Het wordt echter aanbevolen om uitsluitend labels naar Brand Portal te publiceren voordat de elementen (en verzamelingen) waarmee de labels zijn gekoppeld, worden gepubliceerd. Hierdoor wordt het sneller publiceren van de elementen (en verzamelingen) naar Brand Portal gegarandeerd.

## Tags beheren {#manage-tags}

U kunt de bestaande tags gebruiken om aan een element te koppelen of nieuwe tags maken vanuit de AEM Tags-console (**[!UICONTROL Tools | Tagging | AEM Tags]**). In beide scenario&#39;s moet u de labels eerst publiceren naar Brand Portal en ze vervolgens koppelen aan de juiste middelen.

Voer de volgende stappen uit om labels te maken op AEM, de labels te publiceren op Brand Portal en de tags te koppelen aan de juiste elementen (of verzamelingen):

1. **Tags** aanmelden bij AEM Author-instantie met beheerdersrechten en toegang tot **[!UICONTROL AEM Tags]** console via globale navigatie:

   1. Selecteer **[!UICONTROL Tools]**

   1. Selecteer **[!UICONTROL General]**

   1. Selecteer **[!UICONTROL Tagging]**

1. Selecteer **[!UICONTROL Create]** en selecteer de **[!UICONTROL Create Tag]** optie.
1. Opgeven:

   * **[!UICONTROL Title]**

      *(vereist)* Een weergavetoetitel voor de tag.
   * **[!UICONTROL Name]**
      *(vereist)* Een naam voor de tag. Als er geen waarde wordt opgegeven, wordt een geldige knooppuntnaam gemaakt op basis van de titel. Zie [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Beschrijving**

      *(optioneel)* Een beschrijving van de tag.
   * **Tagpad** JCR-pad van de tag.

1. Selecteer deze optie **[!UICONTROL Submit]** om de tag te maken.

   Nadat u een tag op een AEM-instantie hebt gemaakt, is de tag beschikbaar om aan een element te worden gekoppeld (met de sectie Eigenschappen of de sectie Codes beheren van dat element).

1. **Publiceer de tag naar Brand Portal**.

   Ga naar **[!UICONTROL AEM Tags]** console ([!UICONTROL Tools | Tagging | AEM Tags]), selecteer de gewenste markering en publiceer aan het Portaal van het Merk.

1. **Koppel de tag aan een element (of verzameling)**.

   Selecteer een element (of verzameling) en koppel de gewenste tag via het gedeelte Eigenschappen of het gedeelte Codes beheren van dat element. Als u meer wilt weten over het toewijzen van labels aan elementen in AEM Assets, raadpleegt u [gebruikstags om elementen](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets)te ordenen.

1. **Elementen (of verzamelingen) publiceren naar Brand Portal**.\
   Wanneer u een element (of verzameling) publiceert naar Brand Portal, is de bijgevoegde tag ook beschikbaar op Brand Portal.

   Als u de bijgevoegde tag wilt weergeven op het respectievelijke element (of verzameling) in Brand Portal, meldt u zich aan bij Brand Portal en selecteert u het element onder Eigenschappen in de sectie waaraan u de bijgevoegde tag wilt toevoegen.

## Zoeken bevorderen {#search-promote}

Met AEM Assets Brand Portal kunt u specifieke elementen als de beste resultaten maken voor zoekopdrachten op basis van een trefwoordtag.

Voer de volgende stappen uit om elementen voor een zoektrefwoord te verhogen:

1. Open de **[!UICONTROL Properties]** pagina van een element op de AEM-auteurinstantie.
1. Ga naar **[!UICONTROL Advanced]** tabblad.
1. Selecteer in **[!UICONTROL Search Promote]** de **[!UICONTROL Elevate for search keywords]** sectie **[!UICONTROL Add]** om de zoektrefwoorden of -tags toe te voegen.

   ![](assets/search-promote.png)

1. Sla de wijzigingen op.
1. Publiceer het element naar Brand Portal.
1. Meld u aan bij Brand Portal. Tabblad weergeven **[!UICONTROL Advanced]** in **[!UICONTROL Properties]** sectie van het element.
Het **[!UICONTROL Search Promote]** trefwoord is ook zichtbaar in de eigenschappen van dat element.
