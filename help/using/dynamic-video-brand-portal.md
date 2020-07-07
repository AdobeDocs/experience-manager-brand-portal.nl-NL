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
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 0%

---


# Dynamische videoondersteuning op Brand Portal {#dynamic-video-support-on-brand-portal}

Video&#39;s adaptief voorvertonen en afspelen op Brand Portal met ondersteuning voor Dynamic Media. Download ook de dynamische uitvoeringen van de portal en de gedeelde koppelingen.
Poortgebruikers van merken kunnen:

* Een voorvertoning weergeven van video&#39;s op de pagina Asset Details, de Kaartweergave en de voorbeeldpagina voor het delen van koppelingen.
* Video-coderingen afspelen op de pagina Asset Details.
* Geef dynamische uitvoeringen weer op het tabblad Uitvoeringen op de pagina Asset Details.
* Download videocoderingen en mappen met video&#39;s.

>[!NOTE]
>
>Om met video&#39;s te werken en hen te publiceren aan het Portaal van het Merk, zorg ervoor dat uw instantie van AEM Author opstelling of op de Hybride wijze van Dynamic Media of **[!DNL Scene 7]** wijze van Dynamic Media is.

Om video&#39;s voor te vertonen, af te spelen en te downloaden, stelt het Brand Portal de volgende twee configuraties beschikbaar voor beheerders:

* [Dynamic Media Hybride configuratie](#configure-dm-hybrid-settings)als de instantie van AEM Author op dynamische media Hybride wijze loopt.
* [Dynamic Media [!DNL Scene 7] configuratie](#configure-dm-scene7-settings)Als de instantie van AEM Author op dynamische media-**[!DNL Scene 7]** wijze loopt.
Plaats één van beide configuraties die op de configuraties worden gebaseerd u in uw instantie van AEM Author plaatst waarmee de Poorthuurder van het Merk wordt herhaald.

>[!NOTE]
>
>Dynamische video&#39;s worden niet ondersteund op Brand Portal-huurders die zijn geconfigureerd met AEM Author die wordt uitgevoerd in de **[!UICONTROL Scene7Connect]** runmode.

## Hoe worden dynamische video&#39;s afgespeeld? {#how-are-dynamic-videos-played}

![Videocoderingen worden opgehaald uit de cloud](assets/VideoEncodes.png)

Als de configuraties van Dynamic Media ([Hybride](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) of [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configuraties) opstelling op het Portaal van het Merk zijn, worden de dynamische vertoningen gehaald van **[!DNL Scene 7]** server. Videocoderingen worden daarom onmiddellijk voorvertoond en afgespeeld en de kwaliteit wordt verstoord.

Aangezien videocoderingscodes niet in de opslagplaats van het Portaal van het Merk worden opgeslagen en van **[!DNL Scene 7]** server worden gehaald, zorg ervoor dat de configuraties van Dynamic Media op de Instantie van de AEM Author en Portaal van het Merk het zelfde zijn.

>[!NOTE]
>
>Videoviewers en viewervoorinstellingen worden niet ondersteund in Brand Portal. Video&#39;s worden voorvertoond en afgespeeld op standaardviewers in Brand Portal.

## Vereisten {#prerequisites}

Als u met dynamische video&#39;s wilt werken op Brand Portal, moet u:

* **Start de AEM Author op in de modus** DM (Dynamic Media) (waarmee Brand Portal is geconfigureerd) of in de modus [Hybride](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) Dynamic Media of de modus [](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)Dynamic Media (!DNL Scene 7]).
* **Dynamic Media-wolkenservices configureren op AEM Author** Gebaseerd op de Dynamic Media-modus waarop AEM Author wordt uitgevoerd, stelt u een van de [Dynamic Media-wolkenservices](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) of [[!DNL Scene 7]-wolkenservices](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in op AEM Author van **Tools** | **Cloud Service** | **Dynamic Media**.
* **Vorm Dynamic Media op het Portaal** van het Merk die op de de wolkenconfiguraties van Dynamic Media op AEM Author wordt gebaseerd, vorm [Dynamic Media montages](#configure-dm-hybrid-settings) of [[!DNL Scène 7] montages](#configure-dm-scene7-settings) van de administratieve hulpmiddelen van het Portaal van het Merk.
Zorg ervoor dat de [afzonderlijke huurders](#separate-tenants) van het Portaal van het Merk voor AEM Author instanties worden gebruikt die met Dynamic Media worden gevormd Hybride en de wijzen van Dynamic Media **[!UICONTROL Scene7]** , als u functionaliteiten van Dynamic Media Hybrid en Dynamic Media gebruikt **[!UICONTROL S7]**.
* **Publiceer omslagen met videocoderingen die op het Portaal** van het Merk worden toegepast [videocoderingen](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) toepassen en publiceer de omslag die rijke media activa van instantie AEM Author aan het Portaal van het Merk bevat.
* **IPs van de Afstand van de Lijst van gewenste personen in SPS als veilige voorproef toegelaten** Als het gebruiken van Dynamic Media-**[!DNL Scene 7]** (met [veilige voorproef die voor een bedrijf wordt toegelaten](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) ), dan wordt het geadviseerd dat de **[!DNL Scene 7]** bedrijfbeheerder IPs van de openbare uitgang voor respectieve gebieden [](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)**[!UICONTROL Scene 7]** toe_voegt op lijst van gewenste personen gebruikend SPS (het Uitgeven Systeem) flits UI.
De IP&#39;s van de egress zijn als volgt:

| **Regio** | **IP van de uitgang** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

Als u een van deze IP&#39;s wilt toestaan, raadpleegt u [uw account voorbereiden op de beveiligde testservice](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Best practices voor

Volg de onderstaande procedures om ervoor te zorgen dat u een voorvertoning van uw dynamische video-elementen kunt weergeven, deze kunt afspelen en van het Brand Portal (en de gedeelde koppelingen) kunt downloaden:

### Afzonderlijke huurders voor Dynamic Media Hybride en Dynamic Media Scène 7 modi {#separate-tenants}

Als u zowel Dynamic Media als Dynamic Media Hybride eigenschappen gebruikt, wordt het geadviseerd dat u verschillende Poorthuurders van het Merk voor AEM Author instanties gebruikt die met Dynamic Media Hybride en de wijzen van Dynamic Media worden gevormd **[!DNL Scene 7]** **[!DNL Scene 7]** .<br />

![Auteur en BP één op één afbeelding](assets/BPDynamicMedia.png)

### Dezelfde configuratiedetails bij AEM Author-instantie en Brand Portal

Zorg ervoor dat de configuratiedetails-zoals **[!UICONTROL Title]**, **[!UICONTROL Registration ID]**, **[!UICONTROL Video Service URL]** (in **[!UICONTROL Dynamic Media Hybrid]**) en **[!UICONTROL Title]**, geloofsbrieven (**[!UICONTROL Email]** en Wachtwoord), **[!UICONTROL Region]**, **[!UICONTROL Company]** (in Dynamic Media **[!DNL Scene 7]**) - het zelfde in het Portaal van het Merk en **[!UICONTROL AEM cloud configuration]** zijn.

### Lijst van gewenste personen openbare uitgang IPs voor de wijze van Scène 7 van Dynamic Media

Als Dynamic Media **[!UICONTROL Scene 7]**-met [veilige voorproef toegelaten](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-wordt gebruikt om videoactiva aan het Portaal van het Merk te dienen, dan **[!UICONTROL Scene 7]** vestigt een specifieke beeldserver voor het opvoeren van milieu&#39;s of interne toepassingen. Om het even welk verzoek aan deze server controleert het oorsprongIP adres. Als het inkomende verzoek niet binnen de goedgekeurde lijst van IP adressen is, is een mislukkingsreactie teruggekeerd.
De beheerder van het **[!UICONTROL Scene-7]** Bedrijf, daarom, vormt een goedgekeurde lijst van IP adressen voor het **[!UICONTROL Secure Testing]** milieu van hun bedrijf, door **[!UICONTROL SPS]** (Scene-7 het Publiceren Systeem) flits UI. Zorg ervoor dat de IP van de uitgang voor uw respectieve gebied (van het volgende) aan die goedgekeurde lijst wordt toegevoegd.
Als u een van deze IP&#39;s wilt toestaan, raadpleegt u [uw account voorbereiden op de beveiligde testservice](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
De IP&#39;s van de uitgang zijn als volgt:

| **Regio** | **IP van de uitgang** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Instellingen voor Dynamic Media (hybride) configureren {#configure-dm-hybrid-settings}

Als de instantie van AEM Author op dynamische media hybride wijze loopt, dan gebruik **[!UICONTROL Video]** tegel van het administratieve hulpmiddelenpaneel om de montages van de Dynamic Media gateway te vormen.

>[!NOTE]
>
>De [videocoderingsprofielen](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) worden niet gepubliceerd naar Brand Portal, maar opgehaald van de **[!UICONTROL Scene 7]** server. Daarom voor videocoderingscodes die met succes in het Portaal van het Merk moeten worden gespeeld, zorg ervoor dat de configuratiedetails het zelfde als [[!UICONTROL Scene7 wolkenconfiguratie]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) in uw instantie van AEM Author zijn.

Configuraties van Dynamic Media instellen op Brand Portal-huurders:

1. Selecteer het AEM-logo voor toegang tot beheergereedschappen op de werkbalk bovenaan in het Brand Portal.
1. Selecteer de **[!UICONTROL Video]** tegel in het deelvenster met beheergereedschappen.

   ![Hybride configuratie van Dynamic Media op Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL Edit Dynamic Media Configuration]** pagina wordt geopend.

   ![Hybride configuratie van Dynamic Media op het Merkortaal](assets/edit-dynamic-media-config.png)

1. Specificeer **[!UICONTROL Registration ID]** en **[!UICONTROL Video Service URL]** (DM-Gateway URL). Zorg ervoor dat deze gegevens overeenkomen met de gegevens in **[!UICONTROL Tools > Cloud Services]** uw AEM Author-exemplaar.
1. Selecteer **Opslaan** om de configuratie op te slaan.

## Dynamic Media Scene7-instellingen configureren {#configure-dm-scene7-settings}

Als de instantie van AEM Author op Dynamic Media- **[!UICONTROL Scene 7]** wijze loopt, dan gebruik **[!UICONTROL Dynamic Media Configuration]** tegel van het administratieve hulpmiddelenpaneel om de **[!UICONTROL Scene 7]** servermontages te vormen.

Configuraties van Dynamic Media instellen **[!UICONTROL Scene 7]** op Brand Portal-huurders:

1. Selecteer het AEM-logo voor toegang tot beheergereedschappen op de werkbalk bovenaan in het Brand Portal.

2. Selecteer de **[!UICONTROL Dynamic Media Configuration]** tegel in het deelvenster met beheergereedschappen.<br />
   ![DM- [!UICONTROL Scene 7] configuratie op Brand Portal](assets/DMS7-Tile.png)
   **[!UICONTROL Edit Dynamic Media Configuration]** pagina wordt geopend.<br />
   ![Scène 7 Configuratie op het Portaal van het Merk](assets/S7Config.png)

3. Geef:
   * **[!UICONTROL Title]**
   * De geloofsbrieven (**[!UICONTROL Email ID]** en **[!UICONTROL Password]**) om tot de server van Scene 7 toegang te hebben
   * **[!UICONTROL Region]**
Zorg ervoor dat deze waarden overeenkomen met de waarden in uw AEM Author-instantie.

4. Selecteer **[!UICONTROL Connect to Dynamic Media]**.

5. Verstrek de **[!UICONTROL Company name]**, en **[!UICONTROL Save]** de configuratie.
