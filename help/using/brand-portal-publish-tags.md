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

Tags zijn handig voor het ordenen van elementen en het verbeteren van de doorzoekbaarheid van elementen waaraan ze zijn gekoppeld. Tags kunnen worden beschouwd als trefwoorden of labels (metagegevens) die zijn gekoppeld met elementen en waarmee elementen snel kunnen worden gevonden als resultaat van een zoekopdracht. Als u wilt weten hoe tags aan elementen in AEM Assets moeten worden toegewezen, raadpleegt u [tags gebruiken om elementen te ordenen](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

Tags (gekoppeld aan elementen en verzamelingen in AEM) worden automatisch naar Brand Portal gepubliceerd wanneer de elementen (en verzamelingen) met bijbehorende tags naar Brand Portal worden gepubliceerd. De gepubliceerde tags zijn handig om zoekopdrachten in staat te stellen de bijbehorende elementen te vinden.

>[!NOTE]
>
>Het wordt echter aanbevolen om uitsluitend labels naar Brand Portal te publiceren voordat de elementen (en verzamelingen) waarmee de labels zijn gekoppeld, worden gepubliceerd. Hierdoor wordt het sneller publiceren van de elementen (en verzamelingen) naar Brand Portal gegarandeerd.

## Tags {#manage-tags} beheren

U kunt de reeds bestaande markeringen gebruiken om aan activa vast te maken of nieuwe markeringen van AEM console van Markeringen tot stand te brengen (**[!UICONTROL Tools | Tagging | AEM Tags]**). In beide scenario&#39;s moet u de labels eerst publiceren naar Brand Portal en ze vervolgens koppelen aan de juiste middelen.

Als u tags wilt maken op AEM, de tags wilt publiceren op Brand Portal en de tags wilt koppelen aan de juiste elementen (of verzamelingen), voert u de volgende stappen uit:

1. **Maak**
TagsAanmelden bij de instantie AEM-auteur met beheerdersrechten en open  **[!UICONTROL AEM Tags]** console via globale navigatie:

   1. Selecteer **[!UICONTROL Tools]**

   1. Selecteer **[!UICONTROL General]**

   1. Selecteer **[!UICONTROL Tagging]**

1. Selecteer **[!UICONTROL Create]** en selecteer vervolgens **[!UICONTROL Create Tag]** optie.
1. Geef het volgende op:

   * **[!UICONTROL Title]**

      *(vereist)* Een weergavetoetitel voor de tag.
   * **[!UICONTROL Name]**
      *(vereist)* Een naam voor de tag. Als er geen waarde wordt opgegeven, wordt een geldige knooppuntnaam gemaakt op basis van de titel. Zie [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Beschrijving**

      *(optioneel)* Een beschrijving van de tag.
   * **Label het**
pad PathJCR van de tag.

1. Selecteer **[!UICONTROL Submit]** om de tag te maken.

   Nadat u een tag hebt gemaakt op AEM instantie, is de tag beschikbaar om aan een element te worden gekoppeld (met de sectie Eigenschappen of de sectie Codes van dat element beheren).

1. **Publiceer de tag naar Brand Portal**.

   Ga naar **[!UICONTROL AEM Tags]** console ([!UICONTROL Tools | Tagging | AEM Tags]), selecteer de gewenste markering en publiceer aan het Portaal van het Merk.

1. **Koppel de tag aan een element (of verzameling)**.

   Selecteer een element (of verzameling) en koppel de gewenste tag via het gedeelte Eigenschappen of het gedeelte Codes beheren van dat element. Raadpleeg [Tags gebruiken om elementen te ordenen](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets) voor meer informatie over het toewijzen van tags aan elementen in AEM Assets.

1. **Elementen (of verzamelingen) publiceren naar Brand Portal**.\
   Wanneer u een element (of verzameling) publiceert naar Brand Portal, is de bijgevoegde tag ook beschikbaar op Brand Portal.

   Als u de bijgevoegde tag wilt weergeven op het respectievelijke element (of verzameling) in Brand Portal, meldt u zich aan bij Brand Portal en selecteert u het element onder Eigenschappen in de sectie waaraan u de bijgevoegde tag wilt toevoegen.

## Zoeken bevorderen {#search-promote}

Met AEM Assets Brand Portal kunt u specifieke elementen gebruiken als de beste resultaten voor zoekopdrachten op basis van een trefwoordtag.

Voer de volgende stappen uit om elementen voor een zoektrefwoord te verhogen:

1. Open de pagina **[!UICONTROL Properties]** van een element op AEM auteurinstantie.
1. Ga naar **[!UICONTROL Advanced]** tabblad.
1. Selecteer **[!UICONTROL Add]** in **[!UICONTROL Search Promote]** in **[!UICONTROL Elevate for search keywords]** sectie om de zoektrefwoorden of -tags toe te voegen.

   ![](assets/search-promote.png)

1. Sla de wijzigingen op.
1. Publiceer het element naar Brand Portal.
1. Meld u aan bij Brand Portal. Tabblad **[!UICONTROL Advanced]** weergeven in sectie **[!UICONTROL Properties]** van het element.
Het trefwoord **[!UICONTROL Search Promote]** is ook zichtbaar in de eigenschappen van dat element.
