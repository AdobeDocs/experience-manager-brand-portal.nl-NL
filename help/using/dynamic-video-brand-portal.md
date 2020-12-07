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

Video&#39;s adaptief voorvertonen en afspelen op Brand Portal met ondersteuning voor dynamische media. Download ook de dynamische uitvoeringen van de portal en de gedeelde koppelingen.
Poortgebruikers van merken kunnen:

* Een voorvertoning weergeven van video&#39;s op de pagina Asset Details, de Kaartweergave en de voorbeeldpagina voor het delen van koppelingen.
* Video-coderingen afspelen op de pagina Asset Details.
* Geef dynamische uitvoeringen weer op het tabblad Uitvoeringen op de pagina Asset Details.
* Download videocoderingen en mappen met video&#39;s.

>[!NOTE]
>
>Als u met video&#39;s wilt werken en deze naar Brand Portal wilt publiceren, moet u controleren of de AEM-auteur is ingesteld in de modus Dynamische media hybride of Dynamische media **[!DNL Scene 7]**.

Om video&#39;s voor te vertonen, af te spelen en te downloaden, stelt het Brand Portal de volgende twee configuraties beschikbaar voor beheerders:

* [Dynamische hybride ](#configure-dm-hybrid-settings)
configuratie van mediaAls de instantie van de Auteur AEM op dynamische media Hybride wijze loopt.
* [Dynamische  [!DNL Scene 7] ](#configure-dm-scene7-settings)
mediaconfiguratieAls de instantie van de Auteur AEM op dynamische media-**[!DNL Scene 7]** wijze loopt.
Plaats één van beide configuraties die op de configuraties worden gebaseerd u in uw instantie van de Auteur AEM plaatst waarmee de huurder van het Portaal van het Merk wordt herhaald.

>[!NOTE]
>
>Dynamische video&#39;s worden niet ondersteund op Brand Portal-huurders die zijn geconfigureerd met AEM Author die wordt uitgevoerd in de runmode **[!UICONTROL Scene7Connect]**.

## Hoe worden dynamische video&#39;s afgespeeld? {#how-are-dynamic-videos-played}

![Videocoderingen worden opgehaald uit de cloud](assets/VideoEncodes.png)

Als er dynamische medieconfiguraties ([Hybride](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) of [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configuraties) zijn ingesteld op Brand Portal, worden de dynamische uitvoeringen opgehaald van **[!DNL Scene 7]** server. Videocoderingen worden daarom onmiddellijk voorvertoond en afgespeeld en de kwaliteit wordt verstoord.

Aangezien videocoderingscodes niet in de opslagplaats van het Portaal van het Merk worden opgeslagen en van de server **[!DNL Scene 7]** worden gehaald, zorg ervoor dat de Dynamische configuraties van Media op de Instantie van de Auteur AEM en het Portaal van het Merk het zelfde zijn.

>[!NOTE]
>
>Videoviewers en viewervoorinstellingen worden niet ondersteund in Brand Portal. Video&#39;s worden voorvertoond en afgespeeld op standaardviewers in Brand Portal.

## Vereisten {#prerequisites}

Als u met dynamische video&#39;s wilt werken op Brand Portal, moet u:

* **Start AEM-auteur op in de DM-**
modus (Dynamische media). Start de AEM-auteur-instantie (waarmee Brand Portal is geconfigureerd) op de  [Dynamic Media Hybrid-](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) modus of  [Dynamische  [!DNL Scene 7] mediamodus](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configureer Dynamic Media Cloud Services op AEM**
AuteurOp basis van de Dynamic Media Mode waarop AEM Author wordt uitgevoerd, stelt u een van de  [Dynamic Media Cloud ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) Services of  [[!DNL Scene 7] Cloud ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) Services in op AEM Author via  **Tools** |  **Cloud Services** |  **** Dynamic Media.
* **Vorm Dynamische Media op Merk**
PortalGebaseerd op de Dynamische wolkenconfiguraties van Media op Auteur AEM, vorm  [Dynamische ](#configure-dm-hybrid-settings) montages van Media of  [[!DNL Scene 7] ](#configure-dm-scene7-settings)  montages van de administratieve hulpmiddelen van het Portaal van het Merk.
Zorg ervoor dat [de afzonderlijke huurders van het Portaal van het Merk](#separate-tenants) voor AEM Auteursinstanties worden gebruikt die met Dynamische Media Hybrid en Dynamische Media **[!UICONTROL Scene7]** wijzen worden gevormd, als u functionaliteiten van Dynamische Media Hybrid en Dynamische Media **[!UICONTROL S7]** gebruikt.
* **Publiceer omslagen met videocoderingscodes die op Merk**
PortalToepassen  [video ](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) coderingen en publiceer de omslag die rijke media activa van de instantie van de Auteur AEM aan het Portaal van het Merk bevat.
* **IPs van de Afstand van de Lijst van gewenste personen in SPS als veilige voorproef**
toegelatenAls het gebruiken van Dynamische media-**[!DNL Scene 7]** (met  [veilige voorproef ](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) toegelaten voor een bedrijf), dan wordt het geadviseerd dat de  **[!DNL Scene 7]** bedrijfbeheerder de openbare uitgang  [IPs voor respectieve gebieden ](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) toe_voegt op lijst van gewenste personen gebruikend SPS (het **[!UICONTROL Scene 7]** Publiceren Systeem) flits UI.
De IP&#39;s van de egress zijn als volgt:

| **Regio** | **IP van de uitgang** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| EMEA | 185 34 189,1 |
| APAC | 63 140 44 54 |

Zie [Uw account voorbereiden voor een beveiligde testservice](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) om een van deze IP&#39;s voor de uitgang toe te staan.

## Best practices voor

Volg de onderstaande procedures om ervoor te zorgen dat u een voorvertoning van uw dynamische video-elementen kunt weergeven, deze kunt afspelen en van het Brand Portal (en de gedeelde koppelingen) kunt downloaden:

### Afzonderlijke huurders voor dynamische media hybride en Dynamische Media Scene 7 wijzen {#separate-tenants}

Als u zowel Dynamische Media **[!DNL Scene 7]** als Dynamische Hybride eigenschappen van Media gebruikt, wordt het geadviseerd dat u verschillende Poorthuurders van het Merk voor AEM Auteursinstanties gebruikt die met Dynamische Media Hybrid en Dynamische Media **[!DNL Scene 7]** wijzen worden gevormd.<br />

![Auteur en BP één op één afbeelding](assets/BPDynamicMedia.png)

### Dezelfde configuratiedetails op AEM-auteur en Brand Portal

Zorg ervoor dat de configuratiedetails-zoals **[!UICONTROL Title]**, **[!UICONTROL Registration ID]**, **[!UICONTROL Video Service URL]** (in **[!UICONTROL Dynamic Media Hybrid]**) en **[!UICONTROL Title]**, geloofsbrieven (**[!UICONTROL Email]** en Wachtwoord), **[!UICONTROL Region]**, **[!UICONTROL Company]** (in Dynamische Media **[!DNL Scene 7]**) - het zelfde in het Portaal van het Merk en **[!UICONTROL AEM cloud configuration]** zijn.

### Lijst van gewenste personen openbare uitgang IPs voor Dynamische Scène 7 van Media wijze

Als dynamische media **[!UICONTROL Scene 7]**-hebbend [veilige voorproef toegelaten](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-wordt gebruikt om videoactiva aan het Portaal van het Merk te dienen, dan **[!UICONTROL Scene 7]** vestigt een specifieke beeldserver voor het opvoeren milieu&#39;s of interne toepassingen. Om het even welk verzoek aan deze server controleert het oorsprongIP adres. Als het inkomende verzoek niet binnen de goedgekeurde lijst van IP adressen is, is een mislukkingsreactie teruggekeerd.
De **[!UICONTROL Scene-7]** Beheerder van het Bedrijf, daarom, vormt een goedgekeurde lijst van IP adressen voor hun milieu **[!UICONTROL Secure Testing]**, door **[!UICONTROL SPS]** (Scene-7 het Publiceren Systeem) flits UI. Zorg ervoor dat de IP van de uitgang voor uw respectieve gebied (van het volgende) aan die goedgekeurde lijst wordt toegevoegd.
Zie [Uw account voorbereiden voor een beveiligde testservice](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) om een van deze IP&#39;s voor de uitgang toe te staan.
De IP&#39;s van de uitgang zijn als volgt:

| **Regio** | **IP van de uitgang** |
|--- |--- |
| NA | 130.248.160.66, 52.151.32.108 |
| EMEA | 185 34 189,1 |
| APAC | 63 140 44 54 |

## Dynamische media (hybride)-instellingen {#configure-dm-hybrid-settings} configureren

Als de instantie van de Auteur AEM op dynamische media hybride wijze loopt, dan gebruik **[!UICONTROL Video]** tegel van het administratieve hulpmiddelenpaneel om Dynamische de gatewaymontages van Media te vormen.

>[!NOTE]
>
>De [videocoderingsprofielen](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) worden niet gepubliceerd naar Brand Portal, maar worden opgehaald van de **[!UICONTROL Scene 7]**-server. Zorg er daarom voor dat videocoderingscodes in Brand Portal kunnen worden afgespeeld, dat de configuratiedetails hetzelfde zijn als [[!UICONTROL Scene7 cloud configuration]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in uw AEM-auteur-instantie.

Dynamische mediaconfiguraties instellen op Brand Portal-huurders:

1. Selecteer het AEM logo voor toegang tot beheergereedschappen op de werkbalk bovenaan in het Brand Portal.
1. Selecteer de **[!UICONTROL Video]**-tegel in het deelvenster met beheergereedschappen.

   ![Dynamic Media Hybride Config op Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL Edit Dynamic Media Configuration]** pagina wordt geopend.

   ![Dynamic Media Hybride Configuration op Brand Portal](assets/edit-dynamic-media-config.png)

1. Geef **[!UICONTROL Registration ID]** en **[!UICONTROL Video Service URL]** (DM-Gateway URL) op. Zorg ervoor dat deze details dezelfde zijn als die in **[!UICONTROL Tools > Cloud Services]** in uw AEM Auteur-instantie.
1. Selecteer **Opslaan** om de configuratie op te slaan.

## Dynamische media Scene7-instellingen configureren {#configure-dm-scene7-settings}

Als de AEM Auteur instantie op Dynamische Media- **[!UICONTROL Scene 7]** wijze loopt, dan gebruik **[!UICONTROL Dynamic Media Configuration]** tegel van het administratieve hulpmiddelenpaneel om de **[!UICONTROL Scene 7]** servermontages te vormen.

Dynamische media **[!UICONTROL Scene 7]**-configuraties instellen op Brand Portal-huurders:

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
