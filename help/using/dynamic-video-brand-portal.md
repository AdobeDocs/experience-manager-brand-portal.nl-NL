---
title: Dynamische video-ondersteuning op Brand Portal
description: Dynamische video-ondersteuning op Brand Portal
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: e2e007550b557e790533204d49271c90b3b8647d
workflow-type: tm+mt
source-wordcount: '1123'
ht-degree: 0%

---

# Dynamische video-ondersteuning op Brand Portal {#dynamic-video-support-on-brand-portal}

Video&#39;s adaptief voorvertonen en afspelen op Brand Portal met ondersteuning voor Dynamic Media. Download ook de dynamische uitvoeringen van de portal en de gedeelde koppelingen.
Brand Portal-gebruikers kunnen:

* Geef een voorvertoning weer van video&#39;s op de pagina Asset Details, de Kaartweergave en de voorbeeldpagina voor het delen van koppelingen.
* Video-coderingen afspelen op de pagina Asset Details.
* Geef dynamische uitvoeringen weer op het tabblad Uitvoeringen op de pagina Asset Details.
* Download videocoderingen en mappen met video&#39;s.

>[!NOTE]
>
>Als u video&#39;s wilt bewerken en publiceren naar Brand Portal, moet u controleren of de Experience Manager Author-instantie is ingesteld in de Dynamic Media Hybrid-modus of de Dynamic Media **[!DNL Scene7]**-modus.

Voor het voorvertonen, afspelen en downloaden van video&#39;s stelt Brand Portal de volgende twee configuraties beschikbaar aan beheerders:

* [ Hybride configuratie van Dynamic Media ](#configure-dm-hybrid-settings)
Als de Experience Manager Author-instantie wordt uitgevoerd in Dynamic Media - hybride modus.
* [ Dynamic Media  [!DNL Scene7]  configuratie ](#configure-dm-scene7-settings)
Als de Experience Manager Author-instantie wordt uitgevoerd in de modus Dynamic Media - **[!DNL Scene7]** .
Plaats één van beide configuraties die op de configuraties worden gebaseerd u in uw instantie van de Auteur van de Experience Manager plaatst waarmee de huurder van Brand Portal wordt herhaald.

>[!NOTE]
>
>Dynamische video&#39;s worden niet ondersteund op Brand Portal-huurders die zijn geconfigureerd met Experience Manager Author die wordt uitgevoerd in de uitvoermodus van **[!UICONTROL Scene7 Connect]** .

## Hoe worden dynamische video&#39;s afgespeeld? {#how-are-dynamic-videos-played}

![ Video worden coderingen gehaald van wolk ](assets/VideoEncodes.png)

Als de configuraties van Dynamic Media ([ Hybride ](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) of [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configuraties) opstelling op Brand Portal zijn, worden de dynamische vertoningen opgehaald van de **[!DNL Scene7]** server. Videocoderingen worden daarom onmiddellijk voorvertoond en afgespeeld en de kwaliteit wordt verstoord.

De Brand Portal-opslagplaats slaat geen videocoderingen op en haalt deze op van de **[!DNL Scene7]** -server. Zorg ervoor dat de Dynamic Media-configuraties op zowel de Adobe Experience Manager Author Instance als Brand Portal gelijk zijn.

>[!NOTE]
>
>Videoviewers en viewervoorinstellingen worden niet ondersteund in Brand Portal. Video&#39;s worden voorvertoond en afgespeeld op standaardviewers in Brand Portal.

## Vereisten {#prerequisites}

Als u met dynamische video&#39;s wilt werken op Brand Portal, moet u:

* **De Auteur van de Experience Manager van het Begin op de wijze van Dynamic Media**

  Begin de instantie van de Auteur van de Experience Manager (waarmee Brand Portal) of in [ Dynamic Media -  [!DNL Scene7]  wordt gevormd wijze ](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/config-dms7#enabling-dynamic-media-in-scene-mode) of in [ Dynamic Media - Hybride wijze ](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/config-dynamic) of

* **vorm de Cloud Servicen van Dynamic Media op de instantie van de Auteur van de Experience Manager**

  Gebaseerd op de wijze van Dynamic Media (de wijze van Scene7 of de Hybride wijze) die de Auteur van de Experience Manager op loopt, plaats of {de Cloud Servicen van 0} Dynamic Media ([!DNL Scene7] wijze) [&#128279;](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/config-dms7#configuring-dynamic-media-cloud-services) of [ Cloud Servicen van Dynamic Media (Hybride wijze) ](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/config-dms7#configuring-dynamic-media-cloud-services) op de Auteur van de Experience Manager van **Hulpmiddelen** | **Cloud Servicen** | **Dynamic Media**.

* **vorm Dynamic Media op Brand Portal**

  Gebaseerd op de configuraties van de Wolk van Dynamic Media op de Auteur van de Experience Manager, vorm [ montages van Dynamic Media ](#configure-dm-hybrid-settings) of [[!DNL Scene7]  montages ](#configure-dm-scene7-settings) van Brand Portal administratieve hulpmiddelen.

  Zorg ervoor dat [ de afzonderlijke huurders van Brand Portal ](#separate-tenants) voor de instanties van de Auteur van de Experience Manager worden gebruikt die in Dynamic Media - **[!UICONTROL Scene7]** wijze en Dynamic Media - Hybride wijze worden gevormd. Als u de functies van Dynamic Media **[!UICONTROL S7]** en Dynamic Media Hybrid gebruikt, is deze benadering bijzonder belangrijk.

* **de omslagen van Publish met video die coderen op Brand Portal worden toegepast**

  Pas [ videocoderingen ](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/video-profiles) toe en publiceer de omslag die rijke media activa van de instantie van de Auteur van de Experience Manager aan Brand Portal bevat.

* **Lijst van gewenste personen Eind IPs in SPS als veilige voorproef toegelaten**

  Als het gebruiken van Dynamic Media **[!DNL Scene7]** (met [ veilige voorproef toegelaten ](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public) voor een bedrijf), dan wordt het geadviseerd dat **[!DNL Scene7]** bedrijfbeheerder [ de openbare uitgang IPs ](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public#testing-the-secure-testing-service) voor respectieve gebieden voegt op lijst van gewenste personen gebruikend SPS (**[!UICONTROL Scene7]** het Publiceren Systeem) flits UI.

  De IP&#39;s van de egress zijn als volgt:

  | **Gebied** | **IP van de Eis** |
  |--- |--- |
  | NA | 130.248.160.68, 20.94.203.130 |
  | EMEA | 18.34.189.3, 51.132.146.75 |
  | APAC | 63 140 44 54 |

  Om één van beiden van deze uitgang IPs te lijsten van gewenste personen, zie [ uw rekening voor een veilige het testen dienst ](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public#testing-the-secure-testing-service) voorbereiden.

## Aanbevolen procedures

Voer de volgende handelingen uit om dynamische video-elementen van Brand Portal (en gedeelde koppelingen) te bekijken, af te spelen en te downloaden:

### Afzonderlijke huurders voor Dynamic Media - Scene7 en Dynamic Media - Hybride modi {#separate-tenants}

Als u de functies Dynamic Media - **[!DNL Scene7]** mode en Dynamic Media - Hybride modus gebruikt, kunt u verschillende Brand Portal-huurders gebruiken voor instanties van de Experience Manager Author die zijn geconfigureerd met Dynamic Media - **[!DNL Scene7]** en Dynamic Media - Hybride modi.


![ Auteur en BP één aan één afbeelding ](assets/BPDynamicMedia.png)

### Dezelfde configuratiedetails bij de instantie van de Auteur van de Experience Manager en Brand Portal

Zorg ervoor dat de configuratiedetails in Brand Portal en **[!UICONTROL Experience Manager Cloud Configuration]** hetzelfde zijn. Dezelfde configuratiedetails bevatten het volgende:

* **[!UICONTROL Title]**
* **[!UICONTROL Registration ID]**
* **[!UICONTROL Video Service URL]** in **[!UICONTROL Dynamic Media - Hybrid mode]**
* **[!UICONTROL Title]**
* Referenties (**[!UICONTROL Email]** en wachtwoord)
* **[!UICONTROL Region]**
* **[!UICONTROL Company]** in de modus Dynamic Media - **[!DNL Scene7]**

### Lijst van gewenste personen openbare uitgang IPs voor de wijze van Scene7 van Dynamic Media

Als Dynamic Media **[!UICONTROL Scene7]** - het hebben van [ veilige toegelaten voorproef ](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public) - wordt gebruikt om videoactiva aan Brand Portal te dienen, dan **[!UICONTROL Scene7]** vestigt een specifieke beeldserver voor het opvoeren van milieu&#39;s of interne toepassingen. Om het even welk verzoek aan deze server controleert het oorsprongIP adres. Als het inkomende verzoek niet binnen de goedgekeurde lijst van IP adressen is, is een mislukkingsreactie teruggekeerd.
Daarom configureert de **[!UICONTROL Scene7]** bedrijfsbeheerder een goedgekeurde lijst met IP-adressen voor de **[!UICONTROL Secure Testing]** -omgeving van hun bedrijf via de Flash-gebruikersinterface van **[!UICONTROL SPS]** (Scene7 Publishing System). Zorg ervoor dat de IP van de uitgang voor uw respectieve gebied (van het volgende) aan die goedgekeurde lijst wordt toegevoegd.
Om één van beiden van deze uitgang IPs te lijsten van gewenste personen, zie [ uw rekening voor een veilige het testen dienst ](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public#testing-the-secure-testing-service) voorbereiden.
De IP&#39;s van de uitgang zijn als volgt:

| **Gebied** | **IP van de Eis** |
|--- |--- |
| NA | 130.248.160.68, 20.94.203.130 |
| EMEA | 51.132.146.75, 130.248.244.202, 130.248.244.203, 130.248.244.204, 130.2 48.244.210, 130.248.244.211, 13.248.244.212 |
| APAC | 63 140 44 54 |

## Dynamic Media-instellingen (hybride) configureren {#configure-dm-hybrid-settings}

Als de Experience Manager Author-instantie wordt uitgevoerd in de hybride modus voor dynamische media, gebruikt u de **[!UICONTROL Video]** -tegel in het deelvenster met beheergereedschappen om Dynamic Media-gatewayinstellingen te configureren.

>[!NOTE]
>
>De [ video het coderen profielen ](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/video-profiles) worden niet gepubliceerd aan Brand Portal. In plaats daarvan worden ze opgehaald van de **[!UICONTROL Scene7]** -server. Daarom voor video codeert om met succes in Brand Portal worden gespeeld, zorg ervoor dat de configuratiedetails het zelfde als de [ Cloud Servicen van Dynamic Media ([!DNL Scene7] wijze) ](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/dynamic/config-dms7#configuring-dynamic-media-cloud-services) in uw instantie van de Auteur van de Experience Manager zijn.

Dynamic Media-configuraties instellen op Brand Portal-huurders:

1. Selecteer het logo van de Experience Manager, zodat u toegang hebt tot de beheergereedschappen via de werkbalk boven in Brand Portal.
1. Selecteer de tegel **[!UICONTROL Video]** in het deelvenster met beheergereedschappen.

   ![ Hybride Config van Dynamic Media op Brand Portal ](assets/DMHybrid-Video.png)

   **[!UICONTROL Edit Dynamic Media Configuration]** wordt geopend.

   ![ Hybride Configuratie van Dynamic Media op Brand Portal ](assets/edit-dynamic-media-config.png)

1. Geef **[!UICONTROL Registration ID]** en **[!UICONTROL Video Service URL]** (DM-Gateway URL) op. Zorg ervoor dat deze details dezelfde zijn als die details in **[!UICONTROL Tools > Cloud Services]** in de instantie Auteur van de Experience Manager.
1. Selecteer **sparen** om de configuratie te bewaren.

## Dynamic Media Scene7-instellingen configureren {#configure-dm-scene7-settings}

Als de Experience Manager Author-instantie wordt uitgevoerd in de Dynamic Media- **[!UICONTROL Scene7]** -modus, gebruikt u de **[!UICONTROL Dynamic Media Configuration]** -tegel in het deelvenster met beheergereedschappen om de **[!UICONTROL Scene7]** -serverinstellingen te configureren.

Dynamic Media **[!UICONTROL Scene7]** -configuraties instellen op Brand Portal-huurders:

1. Selecteer het logo van de Experience Manager, zodat u toegang hebt tot de beheergereedschappen via de werkbalk boven in Brand Portal.

2. Selecteer de tegel **[!UICONTROL Dynamic Media Configuration]** in het deelvenster met beheergereedschappen.

   ![ DM [!UICONTROL Scene 7] configuratie op Brand Portal ](assets/DMS7-Tile.png)

   **[!UICONTROL Edit Dynamic Media Configuration]** wordt geopend.

   ![ Scène 7 Configuratie op Brand Portal ](assets/S7Config.png)

3. Geef:

   * **[!UICONTROL Title]**
   * Referenties (**[!UICONTROL Email ID]** en **[!UICONTROL Password]**) voor toegang tot de Scene7-server
   * **[!UICONTROL Region]**

   Zorg ervoor dat deze waarden gelijk zijn aan de waarden in de Experience Manager Author-instantie.

4. Selecteer **[!UICONTROL Connect to Dynamic Media]** .

5. Geef **[!UICONTROL Company name]** en **[!UICONTROL Save]** de configuratie op.
