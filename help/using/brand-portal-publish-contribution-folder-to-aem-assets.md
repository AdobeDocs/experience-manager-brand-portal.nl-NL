---
title: Elementen uploaden en de map Contribution publiceren van Brand Portal naar AEM Assets
seo-title: Elementen uploaden en de map Contribution publiceren van Brand Portal naar AEM Assets
description: Bekijk meer inzicht in het uploaden van nieuwe middelen en het publiceren van de map met bijdragen van Brand Portal naar AEM Assets.
seo-description: Bekijk meer inzicht in het uploaden van nieuwe middelen en het publiceren van de map met bijdragen van Brand Portal naar AEM Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 268ee9dc83e98e01107f474780b658b8ccefafa4
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 0%

---


# Bijdragemap publiceren naar AEM Assets {#using-asset-souring-in-bp}

De gebruikers van het Portaal van het merk met aangewezen toestemmingen kunnen veelvoudige activa, of omslagen uploaden die veelvoudige activa bevatten, aan de bijdrageomslag. Gebruikers van Brand Portal kunnen echter alleen elementen uploaden naar de map **NEW**. De map **SHARED** is bedoeld voor de distributie van basislijnelementen (referentie-inhoud) die door de gebruikers van het Brand Portal kunnen worden gebruikt bij het maken van nieuwe middelen voor een bijdrage.

De gebruiker van het Portaal van het merk die toestemming heeft om tot de bijdrageomslag toegang te hebben kan de volgende activiteiten uitvoeren:

* [Elementvereisten downloaden](#download-asset-requirements)
* [Nieuwe elementen uploaden naar de map voor bijdragen](#uplad-new-assets-to-contribution-folder)
* [Bijdragemap publiceren naar AEM Assets](#publish-contribution-folder-to-aem)

## Elementvereisten {#download-asset-requirements} downloaden

De gebruikers van het Portaal van het merk ontvangen automatisch e-mail/pulse berichten wanneer een bijdrageomslag door de AEM gebruiker wordt gedeeld, die hen toestaat om het korte (activa vereiste) document te downloaden, evenals de basisactiva (verwijzing inhoud) te downloaden, van **SHARED** omslag om hun de activavereisten te begrijpen.

De gebruiker van het Portaal van het merk voert de volgende activiteiten uit om activavereisten te downloaden:

* **Download overzicht**: Download de samenvatting (document met middelenvereisten) die is toegevoegd aan de bijdragemap en die informatie bevat over elementen zoals het type middelen, het doel, de ondersteunde indelingen, de maximale grootte van de middelen, enz.
* **Basiselementen** downloaden: Download de basislijnelementen die kunnen worden gebruikt om de vereiste typen elementen te begrijpen. De gebruikers van het Portaal van het merk kunnen deze activa als verwijzing gebruiken om nieuwe activa voor bijdrage tot stand te brengen.

Het dashboard voor Brand Portal weerspiegelt alle bestaande mappen die zijn toegestaan aan de gebruiker van het Brand Portal en de nieuw gedeelde bijdragemap. In dit voorbeeld heeft de gebruiker van het Brand Portal alleen toegang tot de zojuist gemaakte map met bijdragen. Er wordt geen andere bestaande map gedeeld met de gebruiker.

**Elementvereisten downloaden:**

1. Meld u aan bij uw Brand Portal-exemplaar.
1. Selecteer de bijdragemap in het dashboard voor het Brand Portal.
1. Klik op **[!UICONTROL Properties]** ![](assets/properties.png). Het venster Eigenschappen wordt geopend en hierin worden de gegevens van de map Asset Contribution weergegeven.
   ![](assets/download-asset-requirement1.png)
1. Klik **[!UICONTROL Download Brief]** ![](assets/download.png) om het document met elementvereisten op uw lokale computer te downloaden.
   ![](assets/download-asset-requirement2.png)
1. Ga terug naar het dashboard van de Portaalpagina van het Merk.
1. Klik om de bijdragemap te openen. U ziet twee submappen -**[!UICONTROL SHARED]** en **[!UICONTROL NEW]** in de bijdragemap. De map SHARED bevat alle basiselementen (referentie-inhoud) die door de beheerders worden gedeeld.
1. U kunt de map **[!UICONTROL SHARED]** downloaden met alle basislijnelementen op uw lokale computer.
U kunt ook de map **[!UICONTROL SHARED]** openen en op **Downloadpictogram** ![](assets/download.png) klikken om afzonderlijke bestanden/mappen te downloaden.
   ![](assets/download-asset-requirement3.png)

Doorloop de samenvatting (document met vereisten voor elementen) en verwijs naar de basiselementen om inzicht te krijgen in de vereisten voor elementen. Nu kunt u nieuwe middelen maken voor de bijdrage en deze uploaden naar de map met bijdragen.


## Elementen uploaden naar bijdragemap {#uplad-new-assets-to-contribution-folder}

Nadat de gebruikers van het Brand Portal de vereisten voor middelen hebben doorlopen, kunnen ze nieuwe middelen maken voor hun bijdrage en deze uploaden naar de map NEW in de map met bijdragen.

>[!NOTE]
>
>De gebruikers van de Poorten van het Merk kunnen activa slechts aan de NIEUWE omslag uploaden.
>
>De maximale uploadlimiet voor elke Brand Portal-huurder is **10** GB, die cumulatief wordt toegepast op alle bijdragemappen.

>[!NOTE]
>
>Aanbevolen wordt om de uploadruimte vrij te geven na publicatie van de map met bijdragen aan AEM Assets, zodat deze beschikbaar is voor de andere gebruikers van het Brand Portal.
>
>Als er een behoefte is om de uploadlimiet van uw Poorthuurder van het Merk voorbij **10** GB uit te breiden, contacteer de Steun van de Adobe die het vereiste specificeert.


**Nieuwe elementen uploaden:**

1. Meld u aan bij uw Brand Portal-exemplaar.
Het dashboard voor het Brand Portal geeft alle bestaande mappen weer die zijn toegestaan aan de gebruiker van het Brand Portal, samen met de nieuwe gedeelde bijdragemap.

1. Selecteer de map met de bijdrage en klik om deze te openen. De map voor bijdragen bevat twee submappen: **[!UICONTROL SHARED]** en **[!UICONTROL NEW]**.

1. Klik op de **[!UICONTROL NEW]** omslag.

   ![](assets/upload-new-assets1.png)

1. Klik op **[!UICONTROL Create]** > **[!UICONTROL Files]** om afzonderlijke bestanden of mappen (.zip) met meerdere elementen te uploaden.

   ![](assets/upload-new-assets2.png)

1. Blader naar elementen (bestanden of mappen) en upload deze naar de map **[!UICONTROL NEW]**.

   ![](assets/upload-new-assets3.png)

Nadat u alle elementen of mappen naar de map NEW hebt geüpload, publiceert u de map met bijdragen naar AEM Assets.


## Bijdragemap publiceren naar AEM Assets {#publish-contribution-folder-to-aem}

Gebruikers van het Brand Portal kunnen de map met bijdragen publiceren naar AEM Assets zonder dat ze toegang hoeven te hebben tot de AEM auteur.

Zorg ervoor dat u de elementvereisten hebt doorlopen en dat u de nieuw gemaakte middelen in de map **NEW** in de map met bijdragen hebt geüpload.

**Map met bijdragen publiceren:**

1. Meld u aan bij uw Brand Portal-exemplaar.

1. Selecteer de bijdragemap in het dashboard voor het Brand Portal.
1. Klik op **[!UICONTROL Publish to AEM]**.

   ![](assets/export.png)

   ![](assets/publish-contribution-folder-to-aem.png)

Er wordt een e-mail-/pulsmelding verzonden naar de gebruiker en beheerders van het Brand Portal in verschillende stadia van de publicatieworkflow:
1. **In wachtrij**  - Er wordt een melding verzonden naar de gebruikers- en merkportalbeheerders van het Brand Portal wanneer een publicatieworkflow wordt geactiveerd in het Brand Portal.

1. **Voltooid**  - Er wordt een melding verzonden naar de gebruikers en beheerders van het Brand Portal wanneer de map met bijdragen met succes is gepubliceerd naar AEM Assets.

Nadat de nieuwe middelen naar AEM Assets zijn gepubliceerd, kunnen de gebruikers van het Brand Portal deze uit de map NEW verwijderen. De beheerder van het Brand Portal kan de elementen uit de map NEW en Shared verwijderen.

Zodra de doelstelling van het creëren van de bijdrageomslag wordt bereikt, kan de beheerder van het Portaal van het Merk de bijdrageomslag schrappen om uploadruimte voor andere gebruikers vrij te geven.

**Status van taak publiceren**

Er zijn twee rapporten die de beheerders kunnen gebruiken om de status van de omslagen van de activabijdrage te bekijken die van het Portaal van het Merk aan AEM Assets worden gepubliceerd.

* Navigeer in Brand Portal naar **[!UICONTROL Tools]** > **[!UICONTROL Asset Contribution Status]**. Dit rapport geeft de status van alle publicatietaken in verschillende stadia van de publicatieworkflow weer.

   ![](assets/contribution-folder-status.png)

* Navigeer in AEM Assets-auteurinstantie naar **[!UICONTROL Tools]** > **[!UICONTROL Jobs]**. Dit rapport geeft de uiteindelijke status (Voltooid of Fout) weer van alle publicatietaken.

   ![](assets/publishing-status.png)

>[!NOTE]
>
>De gebruikersinterface van AEM Assets als Cloud Service kan een klein verschil hebben maar de workflow blijft ongewijzigd.






