---
title: Publish-tags naar Brand Portal
description: Leer hoe u tags kunt publiceren van Experience Manager Assets naar Brand Portal.
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Publish-tags naar Brand Portal {#publish-tags-to-brand-portal}

Leer hoe u tags kunt publiceren van Experience Manager Assets naar Brand Portal.

Tags zijn handig voor het ordenen van elementen en het verbeteren van de doorzoekbaarheid van elementen waaraan ze zijn gekoppeld. Tags kunnen worden beschouwd als trefwoorden of labels (metagegevens) die zijn gekoppeld met elementen en waarmee elementen snel kunnen worden gevonden als resultaat van een zoekopdracht. Om te weten hoe te om markeringen aan activa in Experience Manager Assets toe te wijzen, verwijs [&#x200B; gebruiksmarkeringen om activa &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-manager-65/content/assets/managing/organize-assets) te organiseren.

Tags (gekoppeld aan elementen en verzamelingen in AEM) worden automatisch naar Brand Portal gepubliceerd wanneer de elementen (en verzamelingen) met de bijbehorende tags naar Brand Portal worden gepubliceerd. De gepubliceerde tags zijn handig om zoekopdrachten in staat te stellen de bijbehorende elementen te vinden.

>[!NOTE]
>
>Adobe raadt u aan alleen labels naar Brand Portal te publiceren voordat u de elementen (en verzamelingen) publiceert waaraan de labels zijn gekoppeld. Deze aanpak zorgt ervoor dat de middelen (en verzamelingen) sneller naar Brand Portal worden gepubliceerd.

## Tags beheren {#manage-tags}

U kunt de reeds bestaande markeringen gebruiken om aan activa vast te maken of nieuwe markeringen van de console van de Markeringen van de AEM tot stand te brengen (**[!UICONTROL Tools | Tagging | AEM Tags]**). In beide scenario&#39;s moet u de tags eerst publiceren naar Brand Portal en vervolgens koppelen aan de juiste elementen.

Ga als volgt te werk als u tags wilt maken bij AEM, de tags op Brand Portal wilt publiceren en de tags aan de juiste elementen (of verzamelingen) wilt koppelen:

1. **creeer Markeringen**
Meld u aan bij een AEM Author-instantie met beheerdersrechten en open de **[!UICONTROL AEM Tags]** -console vanuit globale navigatie:

   1. Selecteren **[!UICONTROL Tools]**

   1. Selecteren **[!UICONTROL General]**

   1. Selecteren **[!UICONTROL Tagging]**

1. Selecteer **[!UICONTROL Create]** en selecteer vervolgens de optie **[!UICONTROL Create Tag]** .
1. Geef het volgende op:

   * **[!UICONTROL Title]**

     *(vereist)* Een vertoningstitel voor de markering.
   * **[!UICONTROL Name]**

     *(vereist)* Een naam voor de markering. Als er geen waarde wordt opgegeven, wordt een geldige knooppuntnaam gemaakt op basis van de titel. Zie [&#x200B; TagID &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-manager-65/content/implementing/developing/platform/tagging/framework).
   * **Beschrijving**

     *(facultatief)* Een beschrijving van de markering.
   * **Weg van de Markering**
JCR-pad van de tag.

1. Selecteer **[!UICONTROL Submit]** om de tag te maken.

   Nadat u een tag op een AEM-instantie hebt gemaakt, is de tag beschikbaar voor bijlage bij een element (met de sectie Eigenschappen of de sectie Codes beheren van dat element).

1. **Publish de markering aan Brand Portal**.

   Ga naar de **[!UICONTROL AEM Tags]** console ([!UICONTROL Tools | Tagging | AEM Tags]), selecteer de gewenste markering en Publish aan Brand Portal.

1. **maak de markering aan activa (of inzameling)** vast.

   Selecteer een element (of verzameling) en koppel de gewenste tag via de sectie Eigenschappen of de sectie Codes beheren van dat element. Meer over weten hoe te om markeringen aan activa in AEM Assets toe te wijzen, ga [&#x200B; gebruiksmarkeringen gaan om activa &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-manager-65/content/assets/managing/organize-assets) te organiseren.

1. **de activa van Publish (of inzamelingen) aan Brand Portal**.\
   Als u een element (of verzameling) publiceert naar Brand Portal, is de bijgevoegde tag ook beschikbaar op Brand Portal.

   Als u de bijgevoegde tag wilt weergeven op het respectievelijke element (of de desbetreffende verzameling) in Brand Portal, meldt u zich aan bij Brand Portal en selecteert u het element. Onder de sectie Eigenschappen ziet u de bijgevoegde tag.

## Zoeken bevorderen {#search-promote}

Met AEM Assets Brand Portal kunt u specifieke elementen als de beste resultaten laten zien voor zoekopdrachten op basis van een trefwoordtag.

Voer de volgende stappen uit om elementen voor een zoektrefwoord te verhogen:

1. Open de pagina **[!UICONTROL Properties]** van een element op AEM auteurinstantie.
1. Ga naar de tab **[!UICONTROL Advanced]** .
1. Selecteer **[!UICONTROL Add]** in de sectie **[!UICONTROL Search Promote]** in de sectie **[!UICONTROL Elevate for search keywords]** om de zoektrefwoorden of -tags toe te voegen.

   ![](assets/search-promote.png)

1. Sla de wijzigingen op.
1. Publish het middel aan Brand Portal.
1. Meld u aan bij Brand Portal. Geef de tab **[!UICONTROL Advanced]** weer in de sectie **[!UICONTROL Properties]** van het element.
Het trefwoord **[!UICONTROL Search Promote]** is ook zichtbaar in de eigenschappen van dat element.
