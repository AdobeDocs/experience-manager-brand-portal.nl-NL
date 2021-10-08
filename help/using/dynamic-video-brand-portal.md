---
title: Dynamische video-ondersteuning op Brand Portal
seo-title: Dynamic video support on Brand Portal
description: Dynamische video-ondersteuning op Brand Portal
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: e970775efa611357378516119077a3bfd52b124f
workflow-type: tm+mt
source-wordcount: '1123'
ht-degree: 0%

---

# Dynamische video-ondersteuning op Brand Portal {#dynamic-video-support-on-brand-portal}

U kunt video&#39;s adaptief voorvertonen en afspelen op Brand Portal met ondersteuning voor Dynamic Media. Download ook de dynamische uitvoeringen van de portal en de gedeelde koppelingen.
Brand Portal-gebruikers kunnen:

* Een voorvertoning weergeven van video&#39;s op de pagina Asset Details, de Kaartweergave en de voorbeeldpagina voor het delen van koppelingen.
* Video-coderingen afspelen op de pagina Asset Details.
* Geef dynamische uitvoeringen weer op het tabblad Uitvoeringen op de pagina Asset Details.
* Download videocoderingen en mappen met video&#39;s.

>[!NOTE]
>
>Om met video&#39;s te werken en hen te publiceren aan Brand Portal, zorg ervoor dat uw instantie van de Auteur van de Experience Manager opstelling of op Dynamic Media Hybrid wijze of Dynamic Media **[!DNL Scene 7]** wijze is.

Voor het voorvertonen, afspelen en downloaden van video&#39;s stelt Brand Portal de volgende twee configuraties beschikbaar aan beheerders:

* [Dynamic Media Hybride ](#configure-dm-hybrid-settings)
configuratieAls de instantie van de Auteur van de Experience Manager op dynamische media Hybride wijze loopt.
* [Dynamic  [!DNL Scene 7] ](#configure-dm-scene7-settings)
MediaconfigurationIf Experience Manager Author instance is running on dynamic media-**[!DNL Scene 7]** mode.
Plaats één van beide configuraties die op de configuraties worden gebaseerd u in uw instantie van de Auteur van de Experience Manager plaatst waarmee de huurder van Brand Portal wordt herhaald.

>[!NOTE]
>
>Dynamische video&#39;s worden niet ondersteund op Brand Portal-huurders die zijn geconfigureerd met Experience Manager Author die wordt uitgevoerd in de runmode **[!UICONTROL Scene7Connect]**.

## Hoe worden dynamische video&#39;s afgespeeld? {#how-are-dynamic-videos-played}

![Videocoderingen worden opgehaald uit de cloud](assets/VideoEncodes.png)

Als Dynamic Media-configuraties ([Hybride](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) of [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configuraties) zijn ingesteld op Brand Portal, worden de dynamische uitvoeringen opgehaald van **[!DNL Scene 7]** server. Videocoderingen worden daarom onmiddellijk voorvertoond en afgespeeld en de kwaliteit wordt verstoord.

Aangezien videocoderingscodes niet worden opgeslagen in de Brand Portal-opslagplaats en worden opgehaald van de **[!DNL Scene 7]**-server, moet u ervoor zorgen dat de Dynamic Media-configuraties op AEM Author Instance en Brand Portal gelijk zijn.

>[!NOTE]
>
>Videoviewers en viewervoorinstellingen worden niet ondersteund in Brand Portal. Video&#39;s worden voorvertoond en afgespeeld op standaardviewers in Brand Portal.

## Vereisten {#prerequisites}

Als u met dynamische video&#39;s wilt werken op Brand Portal, moet u:

* **Start AEM-auteur op in de**
modus DM (Dynamic Media). Start de AEM-auteur-instantie (waarmee Brand Portal is geconfigureerd) op de  [Dynamic Media Hybrid-](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) modus of  [Dynamic  [!DNL Scene 7] Mediamode](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html).
* **Configureer Dynamic Media Cloud Services op AEM**
AuthorGebaseerd op de Dynamic Media-modus waarop AEM Author actief is, stel een van de  [Dynamic Media Cloud ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) Services of  [[!DNL Scene 7] Cloud ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html) Services in op AEM Author via  **Tools** |  **Cloud Services** |  **** Dynamic Media.
* **Configureer Dynamic Media on Brand**
PortalGebaseerd op de Dynamic Media-cloudconfiguraties op AEM-auteur, configureer  [Dynamic Media-](#configure-dm-hybrid-settings) instellingen of - [[!DNL Scene 7] ](#configure-dm-scene7-settings)  instellingen met de beheerprogramma&#39;s van Brand Portal.
Zorg ervoor dat [afzonderlijke Brand Portal-huurders](#separate-tenants) worden gebruikt voor AEM-auteur-instanties die zijn geconfigureerd met de modi Dynamic Media Hybrid en Dynamic Media **[!UICONTROL Scene7]** als u functies van Dynamic Media Hybrid en Dynamic Media **[!UICONTROL S7]** gebruikt.
* **Publiceer omslagen met videocoderingen die op Merk**
Portal worden toegepastPas  [videocoderingen ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) toe en publiceer de omslag die rijke media activa van de instantie van de Auteur AEM aan Brand Portal bevat.
* **IPs van de Afstand van de Lijst van gewenste personen in SPS als veilige voorproef**
toegelatenAls het gebruiken van Dynamic Media-**[!DNL Scene 7]** (met  [veilige voorproef ](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) toegelaten voor een bedrijf), dan wordt het geadviseerd dat de  **[!DNL Scene 7]** bedrijfbeheerder de openbare uitgang  [IPs voor respectieve gebieden ](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) voegt op lijst van gewenste personen gebruikend SPS (het **[!UICONTROL Scene 7]** Publiceren Systeem) flits UI.
De IP&#39;s van de egress zijn als volgt:

| **Regio** | **IP van de uitgang** |
|--- |--- |
| NA | 130.248.160.68, 20.94.203.130 |
| EMEA | 185.34.189.3, 51.132.146.75 |
| APAC | 63 140 44 54 |

Zie [Uw account voorbereiden voor een beveiligde testservice](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) om een van deze IP&#39;s voor de uitgang toe te staan.

## Best practices voor

Voer de volgende handelingen uit om ervoor te zorgen dat u een voorvertoning van uw dynamische video-elementen kunt weergeven, deze kunt afspelen en van Brand Portal kunt downloaden (en gedeelde koppelingen):

### Afzonderlijke huurders voor de modi Dynamic Media Hybrid en Dynamic Media Scene 7 {#separate-tenants}

Als u zowel Dynamic Media **[!DNL Scene 7]** als Dynamic Media Hybrid eigenschappen gebruikt, wordt het geadviseerd dat u verschillende huurders van Brand Portal voor AEM Auteur instanties gebruikt die met Dynamic Media Hybrid en Dynamic Media **[!DNL Scene 7]** wijzen worden gevormd.


![Auteur en BP één op één afbeelding](assets/BPDynamicMedia.png)

### Dezelfde configuratiedetails op AEM Author-instantie en Brand Portal

Zorg ervoor dat de configuratiedetails-zoals **[!UICONTROL Title]**, **[!UICONTROL Registration ID]**, **[!UICONTROL Video Service URL]** (in **[!UICONTROL Dynamic Media Hybrid]**) en **[!UICONTROL Title]**, geloofsbrieven (**[!UICONTROL Email]** en Wachtwoord), **[!UICONTROL Region]**, **[!UICONTROL Company]** (in Dynamic Media **[!DNL Scene 7]**)-zijn het zelfde in Brand Portal en **[!UICONTROL AEM cloud configuration]**.

### Lijst van gewenste personen openbare uitgang IPs voor de wijze van Scène 7 van Dynamic Media

Als Dynamic Media **[!UICONTROL Scene 7]**-hebbend [secure preview enabled](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-wordt gebruikt om video activa aan Brand Portal te dienen, dan **[!UICONTROL Scene 7]** vestigt een specifieke beeldserver voor het opvoeren van milieu&#39;s of interne toepassingen. Om het even welk verzoek aan deze server controleert het oorsprongIP adres. Als het inkomende verzoek niet binnen de goedgekeurde lijst van IP adressen is, is een mislukkingsreactie teruggekeerd.
De **[!UICONTROL Scene-7]** Beheerder van het Bedrijf, daarom, vormt een goedgekeurde lijst van IP adressen voor hun milieu **[!UICONTROL Secure Testing]**, door **[!UICONTROL SPS]** (Scene-7 het Publiceren Systeem) flits UI. Zorg ervoor dat de IP van de uitgang voor uw respectieve gebied (van het volgende) aan die goedgekeurde lijst wordt toegevoegd.
Zie [Uw account voorbereiden voor een beveiligde testservice](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) om een van deze IP&#39;s voor de uitgang toe te staan.
De IP&#39;s van de uitgang zijn als volgt:

| **Regio** | **IP van de uitgang** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| EMEA | 185 34 189,1 |
| APAC | 63 140 44 54 |

## Dynamic Media-instellingen (hybride) configureren {#configure-dm-hybrid-settings}

Als de instantie van de Auteur AEM op dynamische media hybride wijze loopt, dan gebruik **[!UICONTROL Video]** tegel van het administratieve hulpmiddelenpaneel om de gatewaymontages van Dynamic Media te vormen.

>[!NOTE]
>
>De [videocoderingsprofielen](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) worden niet gepubliceerd naar Brand Portal, maar worden opgehaald van de **[!UICONTROL Scene 7]**-server. Zorg er daarom voor dat videocoderingen alleen met succes in Brand Portal kunnen worden afgespeeld als de configuratiedetails hetzelfde zijn als de [Scene7-cloudconfiguratie](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html) in uw AEM-auteurinstantie.

Dynamic Media-configuraties instellen op Brand Portal-huurders:

1. Selecteer het AEM logo voor toegang tot beheergereedschappen op de werkbalk bovenaan in Brand Portal.
1. Selecteer de **[!UICONTROL Video]**-tegel in het deelvenster met beheergereedschappen.

   ![Dynamic Media Hybride Config op Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL Edit Dynamic Media Configuration]** pagina wordt geopend.

   ![Dynamic Media Hybrid Configuration op Brand Portal](assets/edit-dynamic-media-config.png)

1. Geef **[!UICONTROL Registration ID]** en **[!UICONTROL Video Service URL]** (DM-Gateway URL) op. Zorg ervoor dat deze details dezelfde zijn als die in **[!UICONTROL Tools > Cloud Services]** in uw AEM Auteur-instantie.
1. Selecteer **Opslaan** om de configuratie op te slaan.

## Dynamic Media Scene7-instellingen configureren {#configure-dm-scene7-settings}

Als de AEM-auteur-instantie in de Dynamic Media- **[!UICONTROL Scene 7]**-modus wordt uitgevoerd, gebruikt u **[!UICONTROL Dynamic Media Configuration]**-tegel in het deelvenster met beheergereedschappen om de **[!UICONTROL Scene 7]**-serverinstellingen te configureren.

Dynamic Media **[!UICONTROL Scene 7]**-configuraties instellen op Brand Portal-huurders:

1. Selecteer het AEM logo voor toegang tot beheergereedschappen op de werkbalk bovenaan in Brand Portal.

2. Selecteer de **[!UICONTROL Dynamic Media Configuration]**-tegel in het deelvenster met beheergereedschappen.

   ![DM- [!UICONTROL Scene 7] configuratie op Brand Portal](assets/DMS7-Tile.png)

   **[!UICONTROL Edit Dynamic Media Configuration]** pagina wordt geopend.

   ![Scène 7 Configuratie op Brand Portal](assets/S7Config.png)

3. Geef:

   * **[!UICONTROL Title]**
   * Referenties (**[!UICONTROL Email ID]** en **[!UICONTROL Password]**) om tot Scene 7 server toegang te hebben
   * **[!UICONTROL Region]**

   Zorg ervoor dat deze waarden gelijk zijn aan die in uw AEM-auteur-instantie.

4. Selecteer **[!UICONTROL Connect to Dynamic Media]**.

5. Geef **[!UICONTROL Company name]** en **[!UICONTROL Save]** de configuratie op.
