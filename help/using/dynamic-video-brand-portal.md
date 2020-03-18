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
source-git-commit: aa6bd187124888cd62ca1f5c7192f9d65ac6ca8a

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
>Als u video&#39;s wilt bewerken en publiceren naar Brand Portal, moet u controleren of de AEM-auteur is ingesteld in de modus Dynamische media hybride of Dynamische media- **[!DNL Scene 7]** modus.

Om video&#39;s voor te vertonen, af te spelen en te downloaden, stelt het Brand Portal de volgende twee configuraties beschikbaar voor beheerders:

* [Dynamische configuratie](#configure-dm-hybrid-settings)van hybride media als de instantie van de Auteur AEM op dynamische media Hybride wijze loopt.
* [Dynamische media [!DNL Scene 7] configuratie](#configure-dm-scene7-settings)als de instantie van de Auteur AEM op dynamische media-**[!DNL Scene 7]** wijze loopt.
Plaats één van beide configuraties die op de configuraties worden gebaseerd u in uw instantie van de Auteur AEM plaatst waarmee de huurder van het Portaal van het Merk wordt herhaald.

>[!NOTE]
>
>Dynamische video&#39;s worden niet ondersteund op Brand Portal-huurders die zijn geconfigureerd met AEM Author die wordt uitgevoerd in de **[!UICONTROL Scene7Connect]** runmode.

## Hoe worden dynamische video&#39;s afgespeeld? {#how-are-dynamic-videos-played}

![Videocoderingen worden opgehaald uit de cloud](assets/VideoEncodes.png)

Als de Dynamische configuraties van Media ([Hybride](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) of [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configuraties) opstelling op het Portaal van het Merk zijn, worden de dynamische vertoningen gehaald van **[!DNL Scene 7]** server. Videocoderingen worden daarom onmiddellijk voorvertoond en afgespeeld en de kwaliteit wordt verstoord.

Aangezien videocoderingscodes niet in de opslagplaats van het Portaal van het Merk worden opgeslagen en van **[!DNL Scene 7]** server worden gehaald, zorg ervoor dat de Dynamische configuraties van Media op de Instantie van de Auteur AEM en het Portaal van het Merk het zelfde zijn.

>[!NOTE]
>
>Videoviewers en viewervoorinstellingen worden niet ondersteund in Brand Portal. Video&#39;s worden voorvertoond en afgespeeld op standaardviewers in Brand Portal.

## Vereisten {#prerequisites}

Als u met dynamische video&#39;s wilt werken op Brand Portal, moet u:

* **Start AEM-auteur op in de modus** DM (Dynamische media) om de AEM-auteur-instantie (waarmee het Brand Portal is geconfigureerd) op te starten in de modus [Dynamische media hybride of](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) Dynamische media-modus [](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)[!DNL Scene 7].
* **Dynamische mediawolkenservices configureren op AEM-auteur** Op basis van de dynamische-mediamodus waarop AEM-auteur actief is, stelt u [Dynamic Media Cloud Services](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) of [[!DNL Scene 7]-cloudservices](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in op AEM-auteur van **Gereedschappen** | **Cloud Services** | **Dynamische media**.
* **Vorm Dynamische Media op het Portaal** van het Merk op de Dynamische wolkenconfiguraties van Media op Auteur AEM, vorm [Dynamische montages](#configure-dm-hybrid-settings) van Media of [[!DNL Scène 7] montages](#configure-dm-scene7-settings) van de administratieve hulpmiddelen van het Portaal van het Merk.
Zorg ervoor dat de [afzonderlijke huurders](#separate-tenants) van het Portaal van het Merk voor AEM Author instanties worden gebruikt die met Dynamische Media Hybrid en Dynamische **[!UICONTROL Scene7]** wijzen van Media worden gevormd, als u functionaliteiten van Dynamische Media Hybride en Dynamische Media gebruikt **[!UICONTROL S7]**.
* **Publiceer omslagen met videocoderingen die op het Portaal** van het Merk worden toegepast [videocoderingen](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) toepassen en publiceer de omslag die rijke media activa van de instantie van de Auteur AEM aan het Portaal van het Merk bevat.
* **Whitelist IPs van de Eis in SPS als de veilige voorproef toegelaten** Als het gebruiken van Dynamische media-**[!DNL Scene 7]** (met [veilige voorproef die voor een bedrijf wordt toegelaten](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) ), dan wordt het geadviseerd dat de **[!DNL Scene 7]** bedrijfbeheerder IPs van de openbare uitgang voor respectieve gebieden [whitelist gebruikend SPS (het](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)**[!UICONTROL Scene 7]** Uitgeven Systeem) flitsinterface.
De IP&#39;s van de egress zijn als volgt:

| **Regio** | **IP van de uitgang** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

Aan whitelist één van beiden van deze uitgang IPs, zie [uw rekening voor de veilige het testen dienst](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)voorbereiden.

## Aanbevolen werkwijzen

Volg de onderstaande procedures om ervoor te zorgen dat u een voorvertoning van uw dynamische video-elementen kunt weergeven, deze kunt afspelen en van het Brand Portal (en de gedeelde koppelingen) kunt downloaden:

### Afzonderlijke huurders voor de modi Dynamische media Hybride en Dynamische Media Scene 7 {#separate-tenants}

Als u zowel Dynamische Media **[!DNL Scene 7]** als Dynamische Hybride eigenschappen van Media gebruikt, wordt het geadviseerd dat u verschillende Poorthuurders van het Merk voor AEM Auteursinstanties gebruikt die met Dynamische Hybride van Media en Dynamische wijzen van Media worden gevormd **[!DNL Scene 7]** .<br />

![Auteur en BP één op één afbeelding](assets/BPDynamicMedia.png)

### Dezelfde configuratiedetails op AEM-auteur en Brand Portal

Zorg ervoor dat de configuratiedetails-zoals **[!UICONTROL Title]**, **[!UICONTROL Registration ID]**, **[!UICONTROL Video Service URL]** (in **[!UICONTROL Dynamic Media Hybrid]**) en **[!UICONTROL Title]**, geloofsbrieven (**[!UICONTROL Email]** en Wachtwoord), **[!UICONTROL Region]**, **[!UICONTROL Company]** (in Dynamische Media **[!DNL Scene 7]**) - het zelfde in het Portaal van het Merk en **[!UICONTROL AEM cloud configuration]** zijn.

### Whitelist openbaar uitgang IPs voor Dynamische Scène 7 van Media wijze

Als Dynamic Media **[!UICONTROL Scene 7]**- [veilige voorvertoning ingeschakeld](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)gebruikt wordt om video-elementen aan Brand Portal te leveren, **[!UICONTROL Scene 7]** wordt een speciale afbeeldingsserver voor testomgevingen of interne toepassingen ingesteld. Om het even welk verzoek aan deze server controleert het oorsprongIP adres. Als het inkomende verzoek niet binnen de goedgekeurde lijst van IP adressen is, is een mislukkingsreactie teruggekeerd.
De beheerder van het **[!UICONTROL Scene-7]** Bedrijf, daarom, vormt een goedgekeurde lijst van IP adressen voor het **[!UICONTROL Secure Testing]** milieu van hun bedrijf, door **[!UICONTROL SPS]** (Scene-7 het Publiceren Systeem) flits UI. Zorg ervoor dat de IP van de uitgang voor uw respectieve gebied (van het volgende) aan die goedgekeurde lijst wordt toegevoegd.
Aan whitelist één van beiden van deze uitgang IPs, zie [uw rekening voor de veilige het testen dienst](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)voorbereiden.
De IP&#39;s van de uitgang zijn als volgt:

| **Regio** | **IP van de uitgang** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Dynamische media (hybride)-instellingen configureren {#configure-dm-hybrid-settings}

Als de instantie van de Auteur AEM op dynamische media hybride wijze loopt, dan gebruik **[!UICONTROL Video]** tegel van het administratieve hulpmiddelenpaneel om Dynamische de gatewaymontages van Media te vormen.
>[!NOTE]
>
>De [videocoderingsprofielen](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) worden niet gepubliceerd naar Brand Portal, maar opgehaald van de **[!UICONTROL Scene 7]** server. Daarom voor videocoderingscodes die met succes in het Portaal van het Merk moeten worden gespeeld, zorg ervoor dat de configuratiedetails het zelfde als de [[!UICONTROL Scene7 wolkenconfiguratie]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in uw instantie van de Auteur AEM zijn.
Dynamische mediaconfiguraties instellen op Brand Portal-huurders:

1. Selecteer het AEM-logo voor toegang tot beheergereedschappen op de werkbalk bovenaan in het Brand Portal.

2. Selecteer de **[!UICONTROL Video]** tegel in het deelvenster met beheergereedschappen.<br />
   ![Dynamic Media Hybride Config op Brand Portal](assets/DMHybrid-Video.png)
   **[!UICONTROL Edit Dynamic Media Configuration]** pagina wordt geopend.<br />
   ![Dynamic Media Hybride Configuration op Brand Portal](assets/edit-dynamic-media-config.png)

3. Specificeer **[!UICONTROL Registration ID]** en **[!UICONTROL Video Service URL]** (DM-Gateway URL). Zorg ervoor dat deze gegevens overeenkomen met die in **[!UICONTROL Tools > Cloud Services]** uw AEM-auteur-exemplaar.

4. Selecteer **Opslaan** om de configuratie op te slaan.

## Dynamische montages van Media Scene7 vormen {#configure-dm-scene7-settings}

Als de instantie van de Auteur AEM op Dynamische media- **[!UICONTROL Scene 7]** wijze loopt, dan gebruik **[!UICONTROL Dynamic Media Configuration]** tegel van het administratieve hulpmiddelenpaneel om de **[!UICONTROL Scene 7]** servermontages te vormen.

Dynamische media- **[!UICONTROL Scene 7]** configuraties instellen op Brand Portal-huurders:

1. Selecteer het AEM-logo voor toegang tot beheergereedschappen op de werkbalk bovenaan in het Brand Portal.

2. Selecteer de **[!UICONTROL Dynamic Media Configuration]** tegel in het deelvenster met beheergereedschappen.<br />
   ![DM- [!UICONTROL Scene 7] configuratie op Brand Portal](assets/DMS7-Tile.png)
   **[!UICONTROL Edit Dynamic Media Configuration]** pagina wordt geopend.<br />
   ![Scène 7 Configuratie op het Portaal van het Merk](assets/S7Config.png)

3. Geef:
   * **[!UICONTROL Title]**
   * De geloofsbrieven (**[!UICONTROL Email ID]** en **[!UICONTROL Password]**) om tot de server van Scene 7 toegang te hebben
   * **[!UICONTROL Region]**
Zorg ervoor dat deze waarden gelijk zijn aan die in uw AEM-auteur-instantie.

4. Selecteer **[!UICONTROL Connect to Dynamic Media]**.

5. Verstrek de **[!UICONTROL Company name]**, en **[!UICONTROL Save]** de configuratie.
