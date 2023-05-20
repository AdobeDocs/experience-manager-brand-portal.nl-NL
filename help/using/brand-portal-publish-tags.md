---
title: Tags publiceren naar Brand Portal
seo-title: Publish tags to Brand Portal
description: Leer hoe u tags kunt publiceren van Experience Manager Assets naar Brand Portal.
seo-description: Learn how to publish tags from Experience Manager Assets to Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 3%

---

# Tags publiceren naar Brand Portal {#publish-tags-to-brand-portal}

Leer hoe u tags kunt publiceren van Experience Manager Assets naar Brand Portal.

Tags zijn handig voor het ordenen van elementen en het verbeteren van de doorzoekbaarheid van elementen waaraan ze zijn gekoppeld. Tags kunnen worden beschouwd als trefwoorden of labels (metagegevens) die zijn gekoppeld met elementen en waarmee elementen snel kunnen worden gevonden als resultaat van een zoekopdracht. Zie voor informatie over het toewijzen van labels aan elementen in Experience Manager Assets [tags gebruiken om elementen te ordenen](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

Tags (gekoppeld aan elementen en verzamelingen in AEM) worden automatisch naar Brand Portal gepubliceerd wanneer de elementen (en verzamelingen) met de bijbehorende tags naar Brand Portal worden gepubliceerd. De gepubliceerde tags zijn handig om zoekopdrachten in staat te stellen de bijbehorende elementen te vinden.

>[!NOTE]
>
>Het wordt echter aanbevolen alleen labels naar Brand Portal te publiceren voordat u de elementen (en verzamelingen) publiceert waaraan de tags zijn gekoppeld. Zo zorgt u ervoor dat de elementen (en verzamelingen) sneller naar Brand Portal worden gepubliceerd.

## Tags beheren {#manage-tags}

U kunt de bestaande tags gebruiken om aan een element te koppelen of om nieuwe tags te maken via de AEM Tags-console (**[!UICONTROL Tools | Tagging | AEM Tags]**). In beide scenario&#39;s moet u de tags eerst publiceren naar Brand Portal en vervolgens koppelen aan de juiste elementen.

Ga als volgt te werk als u tags wilt maken bij AEM, de tags op Brand Portal wilt publiceren en de tags aan de juiste elementen (of verzamelingen) wilt koppelen:

1. **Tags maken**
Meld u aan bij de instantie AEM-auteur met beheerdersrechten en toegang **[!UICONTROL AEM Tags]** console van globale navigatie:

   1. Selecteer **[!UICONTROL Tools]**

   1. Selecteer **[!UICONTROL General]**

   1. Selecteer **[!UICONTROL Tagging]**

1. Selecteren **[!UICONTROL Create]** en selecteer vervolgens **[!UICONTROL Create Tag]** optie.
1. Geef het volgende op:

   * **[!UICONTROL Title]**

      *(vereist)* Een titel voor het weergeven van de tag.
   * **[!UICONTROL Name]**
      *(vereist)* Een naam voor de tag. Als er geen waarde wordt opgegeven, wordt een geldige knooppuntnaam gemaakt op basis van de titel. Zie [TagID](https://experienceleague.adobe.com/docs/experience-manager-65/developing/platform/tagging/framework.html).
   * **Beschrijving**

      *(optioneel)* Een beschrijving van de tag.
   * **Labelpad**
JCR-pad van de tag.

1. Selecteren **[!UICONTROL Submit]** om de tag te maken.

   Nadat u een tag hebt gemaakt op AEM instantie, is de tag beschikbaar om aan een element te worden gekoppeld (met de sectie Eigenschappen of de sectie Codes van dat element beheren).

1. **De tag publiceren naar Brand Portal**.

   Ga naar **[!UICONTROL AEM Tags]** console ([!UICONTROL Tools | Tagging | AEM Tags]), selecteert u de gewenste tag en publiceert u naar Brand Portal.

1. **De tag aan een element (of verzameling) koppelen**.

   Selecteer een element (of verzameling) en koppel de gewenste tag via het gedeelte Eigenschappen of het gedeelte Codes beheren van dat element. Raadpleeg voor meer informatie over het toewijzen van labels aan elementen in AEM Assets [tags gebruiken om elementen te ordenen](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

1. **Elementen (of verzamelingen) publiceren naar Brand Portal**.\
   Als u een element (of verzameling) publiceert naar Brand Portal, is de bijgevoegde tag ook beschikbaar op Brand Portal.

   Als u de bijgevoegde tag wilt weergeven op het respectievelijke element (of de desbetreffende verzameling) in Brand Portal, meldt u zich aan bij Brand Portal en selecteert u het element. In het gedeelte Eigenschappen ziet u de bijgevoegde tag.

## Zoeken bevorderen {#search-promote}

Met AEM Assets Brand Portal kunt u specifieke elementen gebruiken als de beste resultaten voor zoekopdrachten op basis van een trefwoordtag.

Voer de volgende stappen uit om elementen voor een zoektrefwoord te verhogen:

1. Open de **[!UICONTROL Properties]** pagina van een element op AEM instantie van de auteur.
1. Ga naar **[!UICONTROL Advanced]** tab.
1. In **[!UICONTROL Search Promote]** binnen **[!UICONTROL Elevate for search keywords]** sectie, selecteert u **[!UICONTROL Add]** om de zoektrefwoorden of -tags toe te voegen.

   ![](assets/search-promote.png)

1. Sla de wijzigingen op.
1. Publiceer het element naar Brand Portal.
1. Meld u aan bij Brand Portal. Weergave **[!UICONTROL Advanced]** tab in **[!UICONTROL Properties]** van het element.
De **[!UICONTROL Search Promote]** trefwoord is ook zichtbaar in de eigenschappen van dat element.
