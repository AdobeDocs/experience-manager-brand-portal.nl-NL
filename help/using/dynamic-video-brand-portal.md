---
title: Dynamische videoondersteuning op Brand Portal
seo-title: Dynamische videoondersteuning op Brand Portal
description: Dynamische videoondersteuning op Brand Portal
seo-description: Dynamische videoondersteuning op Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: b69025074080b83ac699da434fc525fea1cb100a
workflow-type: tm+mt
source-wordcount: '1136'
ht-degree: 0%

---


# Dynamische videoondersteuning op Brand Portal {#dynamic-video-support-on-brand-portal}

Video&#39;s adaptief voorvertonen en afspelen op Brand Portal met Dynamic Media-ondersteuning. Download ook de dynamische uitvoeringen van de portal en de gedeelde koppelingen.
Poortgebruikers van merken kunnen:

* Een voorvertoning weergeven van video&#39;s op de pagina Asset Details, de Kaartweergave en de voorbeeldpagina voor het delen van koppelingen.
* Video-coderingen afspelen op de pagina Asset Details.
* Geef dynamische uitvoeringen weer op het tabblad Uitvoeringen op de pagina Asset Details.
* Download videocoderingen en mappen met video&#39;s.

>[!NOTE]
>
>Als u video&#39;s wilt bewerken en publiceren naar Brand Portal, moet u controleren of de AEM-auteur is ingesteld in de Dynamic Media Hybrid-modus of in de Dynamic Media-modus **[!DNL Scene 7]**.

Om video&#39;s voor te vertonen, af te spelen en te downloaden, stelt het Brand Portal de volgende twee configuraties beschikbaar voor beheerders:

* [Dynamic Media Hybride ](#configure-dm-hybrid-settings)
configuratieAls de AEM Auteur instantie op dynamische media Hybride wijze loopt.
* [Dynamische  [!DNL Scene 7] ](#configure-dm-scene7-settings)
mediaconfiguratieAls de instantie van de Auteur AEM op dynamische media-**[!DNL Scene 7]** wijze loopt.
Plaats één van beide configuraties die op de configuraties worden gebaseerd u in uw instantie van de Auteur AEM plaatst waarmee de huurder van het Portaal van het Merk wordt herhaald.

>[!NOTE]
>
>Dynamische video&#39;s worden niet ondersteund op Brand Portal-huurders die zijn geconfigureerd met AEM Author die wordt uitgevoerd in de runmode **[!UICONTROL Scene7Connect]**.

## Hoe worden dynamische video&#39;s afgespeeld? {#how-are-dynamic-videos-played}

![Videocoderingen worden opgehaald uit de cloud](assets/VideoEncodes.png)

Als Dynamic Media-configuraties ([Hybride](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) of [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configuraties) zijn ingesteld op Brand Portal, worden de dynamische uitvoeringen opgehaald van **[!DNL Scene 7]** server. Videocoderingen worden daarom onmiddellijk voorvertoond en afgespeeld en de kwaliteit wordt verstoord.

Aangezien videocoderingscodes niet worden opgeslagen in de opslagplaats van het Brand Portal en worden opgehaald van de **[!DNL Scene 7]**-server, dient u ervoor te zorgen dat de Dynamic Media-configuraties op AEM-auteur en -portal gelijk zijn.

>[!NOTE]
>
>Videoviewers en viewervoorinstellingen worden niet ondersteund in Brand Portal. Video&#39;s worden voorvertoond en afgespeeld op standaardviewers in Brand Portal.

## Vereisten {#prerequisites}

Als u met dynamische video&#39;s wilt werken op Brand Portal, moet u:

* **Start AEM-auteur op in de**
modus DM (Dynamic Media). Start de AEM-auteur-instantie (waarmee het Brand Portal is geconfigureerd) op de  [Dynamic Media Hybrid-](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) modus of  [Dynamic  [!DNL Scene 7] Mediamode](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configureer Dynamic Media Cloud Services op AEM**
AuthorGebaseerd op de Dynamic Media-modus waarop AEM Author actief is, stel een van de  [Dynamic Media Cloud ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) Services of  [[!DNL Scene 7] Cloud ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) Services in op AEM Author via  **Tools** |  **Cloud Services** |  **** Dynamic Media.
* **Configureer Dynamic Media on Brand**
PortalGebaseerd op de Dynamic Media-cloudconfiguraties op AEM-auteur, configureer  [Dynamic Media-](#configure-dm-hybrid-settings) instellingen of  [[!DNL Scene 7] ](#configure-dm-scene7-settings)  instellingen met beheertools van het Brand Portal.
Zorg ervoor dat [de afzonderlijke huurders van het Merk ](#separate-tenants) voor de instanties van de Auteur van AEM worden gebruikt die met de wijzen van Dynamic Media Hybrid en van Dynamic Media **[!UICONTROL Scene7]** worden gevormd, als u functionaliteiten van Dynamic Media Hybrid en Dynamic Media **[!UICONTROL S7]** gebruikt.
* **Publiceer omslagen met videocoderingscodes die op Merk**
PortalToepassen  [video ](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) coderingen en publiceer de omslag die rijke media activa van de instantie van de Auteur AEM aan het Portaal van het Merk bevat.
* **IPs van de Afstand van de Lijst van gewenste personen in SPS als veilige voorproef**
toegelatenAls het gebruiken van Dynamic Media-**[!DNL Scene 7]** (met  [veilige voorproef ](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) toegelaten voor een bedrijf), dan wordt het geadviseerd dat de  **[!DNL Scene 7]** bedrijfbeheerder de openbare uitgang  [IPs voor respectieve gebieden ](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) voegt op lijst van gewenste personen gebruikend SPS (het **[!UICONTROL Scene 7]** Publiceren Systeem) flits UI.
De IP&#39;s van de egress zijn als volgt:

| **Regio** | **IP van de uitgang** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| EMEA | 185 34 189,1 |
| APAC | 63 140 44 54 |

Zie [Uw account voorbereiden voor een beveiligde testservice](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) om een van deze IP&#39;s voor de uitgang toe te staan.

## Best practices voor

Volg de onderstaande procedures om ervoor te zorgen dat u een voorvertoning van uw dynamische video-elementen kunt weergeven, deze kunt afspelen en van het Brand Portal (en de gedeelde koppelingen) kunt downloaden:

### Afzonderlijke huurders voor Dynamic Media Hybrid en Dynamic Media Scene 7 modi {#separate-tenants}

Als u zowel Dynamic Media **[!DNL Scene 7]** als Dynamic Media Hybrid eigenschappen gebruikt, wordt het geadviseerd dat u verschillende Poorthuurders van het Merk voor AEM Author instanties gebruikt die met Dynamic Media Hybrid en Dynamic Media **[!DNL Scene 7]** wijzen worden gevormd.<br />

![Auteur en BP één op één afbeelding](assets/BPDynamicMedia.png)

### Dezelfde configuratiedetails op AEM-auteur en Brand Portal

Zorg ervoor dat de configuratiedetails-zoals **[!UICONTROL Title]**, **[!UICONTROL Registration ID]**, **[!UICONTROL Video Service URL]** (in **[!UICONTROL Dynamic Media Hybrid]**) en **[!UICONTROL Title]**, geloofsbrieven (**[!UICONTROL Email]** en Wachtwoord), **[!UICONTROL Region]**, **[!UICONTROL Company]** (in Dynamic Media **[!DNL Scene 7]**)-zijn het zelfde in het Portaal van het Merk en **[!UICONTROL AEM cloud configuration]**.

### Lijst van gewenste personen openbare uitgang IPs voor de wijze van Scène 7 van Dynamic Media

Als Dynamic Media **[!UICONTROL Scene 7]**-hebbend [veilige voorproef toegelaten](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-wordt gebruikt om videoactiva aan het Portaal van het Merk te dienen, dan **[!UICONTROL Scene 7]** vestigt een specifieke beeldserver voor het opvoeren milieu&#39;s of interne toepassingen. Om het even welk verzoek aan deze server controleert het oorsprongIP adres. Als het inkomende verzoek niet binnen de goedgekeurde lijst van IP adressen is, is een mislukkingsreactie teruggekeerd.
De **[!UICONTROL Scene-7]** Beheerder van het Bedrijf, daarom, vormt een goedgekeurde lijst van IP adressen voor hun milieu **[!UICONTROL Secure Testing]**, door **[!UICONTROL SPS]** (Scene-7 het Publiceren Systeem) flits UI. Zorg ervoor dat de IP van de uitgang voor uw respectieve gebied (van het volgende) aan die goedgekeurde lijst wordt toegevoegd.
Zie [Uw account voorbereiden voor een beveiligde testservice](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) om een van deze IP&#39;s voor de uitgang toe te staan.
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
>De [videocoderingsprofielen](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) worden niet gepubliceerd naar Brand Portal, maar worden opgehaald van de **[!UICONTROL Scene 7]**-server. Zorg er daarom voor dat videocoderingscodes in Brand Portal kunnen worden afgespeeld, dat de configuratiedetails hetzelfde zijn als [[!UICONTROL Scene7 cloud configuration]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in uw AEM-auteur-instantie.

Dynamic Media-configuraties instellen op Brand Portal-huurders:

1. Selecteer het AEM logo voor toegang tot beheergereedschappen op de werkbalk bovenaan in het Brand Portal.
1. Selecteer de **[!UICONTROL Video]**-tegel in het deelvenster met beheergereedschappen.

   ![Dynamic Media Hybrid Config op Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL Edit Dynamic Media Configuration]** pagina wordt geopend.

   ![Dynamic Media Hybrid Configuration on Brand Portal](assets/edit-dynamic-media-config.png)

1. Geef **[!UICONTROL Registration ID]** en **[!UICONTROL Video Service URL]** (DM-Gateway URL) op. Zorg ervoor dat deze details dezelfde zijn als die in **[!UICONTROL Tools > Cloud Services]** in uw AEM Auteur-instantie.
1. Selecteer **Opslaan** om de configuratie op te slaan.

## Dynamic Media Scene7-instellingen configureren {#configure-dm-scene7-settings}

Als de AEM-auteur-instantie in de Dynamic Media- **[!UICONTROL Scene 7]**-modus wordt uitgevoerd, gebruikt u **[!UICONTROL Dynamic Media Configuration]**-tegel in het deelvenster met beheergereedschappen om de **[!UICONTROL Scene 7]**-serverinstellingen te configureren.

Dynamic Media **[!UICONTROL Scene 7]**-configuraties instellen op Brand Portal-huurders:

1. Selecteer het AEM logo voor toegang tot beheergereedschappen op de werkbalk bovenaan in het Brand Portal.

2. Selecteer in het deelvenster met beheergereedschappen de **[!UICONTROL Dynamic Media Configuration]**-tegel.<br />
   ![DM- [!UICONTROL Scene 7] configuratie op Brand Portal](assets/DMS7-Tile.png)
   **[!UICONTROL Edit Dynamic Media Configuration]** pagina wordt geopend.<br />
   ![Scène 7 Configuratie op het Portaal van het Merk](assets/S7Config.png)

3. Geef:
   * **[!UICONTROL Title]**
   * Referenties (**[!UICONTROL Email ID]** en **[!UICONTROL Password]**) om tot Scene 7 server toegang te hebben
   * **[!UICONTROL Region]**
Zorg ervoor dat deze waarden gelijk zijn aan die in uw AEM-auteur-instantie.

4. Selecteer **[!UICONTROL Connect to Dynamic Media]**.

5. Geef **[!UICONTROL Company name]** en **[!UICONTROL Save]** de configuratie op.
