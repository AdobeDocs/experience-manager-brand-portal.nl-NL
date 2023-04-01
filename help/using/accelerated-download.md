---
title: Brand Portal-downloads versnellen
seo-title: Speed up the Brand Portal downloads
description: Verbeter de downloadprestaties van Brand Portal en de gedeelde koppelingen.
seo-description: Enhance download performance from Brand Portal and the shared links.
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: Vishabh Gupta
topic-tags: download-install, download assets
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bfc145fed0c0
exl-id: cf28df58-c6dd-4b12-8279-01351892009f
source-git-commit: b91e0b4f03beb37d826ce75ac49498b7b79e4a39
workflow-type: tm+mt
source-wordcount: '978'
ht-degree: 2%

---

# Brand Portal-downloads versnellen {#guide-to-accelerate-downloads-from-brand-portal}

<!-- This topic is woefully out of date. It talks at length about using a third party application whose URLs have a variety of problems. Topic should either be deleted or updated entirely to not talk about a specific third party application that Adobe has no control over. It also appears that the third party app is NOT free anymore. -->

Adobe Experience Manager Assets Brand Portal maakt het mogelijk de downloadprestaties van grote bestanden met middelen te verbeteren door integratie met IBM® Aspera Connect, een toepassing die op aanvraag wordt geïnstalleerd. De toepassing gebruikt merkgebonden technologie om de overheadkosten van TCP te verwijderen en helpt overdrachtsnelheid van de activadossiers te verbeteren. Deze integratie zorgt voor een verbeterde downloadervaring.

>[!NOTE]
>
>Downloadsnelheid verschilt voor gebruikers omdat dit afhankelijk is van factoren zoals netwerkbandbreedte, serverlatentie en geografische locatie van clients.

De **[!UICONTROL Fast Download]** De configuratie is standaard ingeschakeld, waardoor de downloadtijd voor de gewenste elementbestanden van Brand Portal aanzienlijk afneemt.

![](assets/download-settings-new.png)

## Vereisten om bestanden sneller te downloaden {#prerequisites-to-accelerate-file-download}

Als u de bestanden sneller wilt downloaden, moet u het volgende doen:

* Navigeren naar **[!UICONTROL Tools]** > **[!UICONTROL Download]** en verifieert **[!UICONTROL Fast Download]** configuratie is ingeschakeld in **[!UICONTROL Download Settings]**.
* Zorg ervoor dat poort 33001 (zowel TCP als UDP) is geopend op de firewall. Voor meer informatie over de eerste vereisten, zie [Documentatie IBM® Aspera Connect Client](https://downloads.asperasoft.com/en/documentation/8).
* **IBM® Aspera Connect 3.9.9 installeren** in de extensie van uw browser met beheerdersrechten (`https://www.ibm.com/docs/en/aspera-connect/3.9.9`).
* Voor platformondersteuning van Aspera Transfer Client raadpleegt u [IBM® Aspera Connect-platformsupportmatrix](https://www.asperasoft.com/company/support/transfer-clients/).

>[!NOTE]
>
>Er is een bekend probleem met IBM® Aspera Connect. Snel downloaden werkt niet met IBM® Aspera Connect versie 3.10 en hoger.

## Domeinen downloaden {#download-domains}

Hier volgen de downloaddomeinen voor verschillende geografische gebieden:

| Gebiedscode | Domein |
|---|---|
| NA OF1 | downloads-na1.brand-portal.adobe.com |
| NA VA5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

## Voorbeeld van downloadprestaties met gebruik van bestandsaccelerator {#expected-download-performance-using-file-accelerator}

In de volgende tabel ziet u de downloadprestaties voor een bestand van 2 GB met de Aspera Connect-bestandsdownloadaccelerator:

*De waargenomen resultaten variëren door factoren zoals netwerkbandbreedte, serverlatentie, en cliëntplaats, gezien de server van Brand Portal bij Oregon (Verenigde Staten) is.*

| Clientlocatie | Latentie tussen client en server (milliseconden) | Snelheid met Aspera Connect File Transfer Accelerator (MBps) | Tijd die nodig is om een bestand van 2 GB te downloaden met Aspera File Transfer Accelerator (seconden) |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| V.S. West (N. Californië) | 18 | 36 | 57 |
| V.S. West (Oregon) | 42 | 36 | 57 |
| V.S. Oost (N. Virginia) | 85 | 35 | 58 |
| APAC (Tokio) | 124 | 36 | 57 |
| Noida (India) | 275 | 13.36 | 153 |
| Sydney | 175 | 29 | 70 |
| Londen | 179 | 35 | 58 |
| Singapore | 196 | 34 | 60 |

## Elementen downloaden {#download-assets}

Zo downloadt u elementen sneller van Brand Portal:

1. Meld u aan bij uw Brand Portal-huurder. Standaard worden de **[!UICONTROL Files]** wordt geopend met alle gepubliceerde elementen en mappen.

   Voer een van de volgende handelingen uit:

   * Selecteer de elementen of mappen die u wilt downloaden. Klik in de werkbalk bovenaan op de knop **[!UICONTROL Download]** pictogram.

      ![select-multiple-assets](assets/select-assets-new.png)

   * Als u specifieke elementuitvoeringen van een element wilt downloaden, plaatst u de aanwijzer boven het element en klikt u op de knop **[!UICONTROL Download]** in de miniaturen voor snelle acties.

      ![select-element](assets/select-asset.png)

1. De **[!UICONTROL Download]** wordt geopend.

   Als u de Brand Portal-maphiërarchie wilt behouden terwijl u elementen downloadt, selecteert u de optie **[!UICONTROL Create separate folder for each asset]** selectievakje.

   De downloadknop geeft het aantal geselecteerde items weer. Als u klaar bent met het toepassen van de regels, klikt u op **[!UICONTROL Download items]**. Ga voor meer informatie over het toepassen van regels naar [downloadmiddelen](../using/brand-portal-download-assets.md#download-assets).

   ![download-dialog](assets/download-dialog-box-new.png)

1. Standaard worden de **[!UICONTROL Fast Download]** instelling is ingeschakeld in het dialoogvenster **[!UICONTROL Download Settings]**. Daarom wordt een bevestigingsvenster weergegeven waarin u middelen kunt downloaden met IBM® Aspera Connect.

   Als u de middelen voor het eerst downloadt en IBM® Aspera Connect niet in uw browser heeft geïnstalleerd of als de bestaande versie verouderd is, wordt u gevraagd om de Aspera-downloadaccelerator te installeren (`https://www.ibm.com/docs/en/aspera-connect/3.9.9`).

   ![](assets/aspera-not-launched.png)

1. **Aspera Connect-client installeren**

   Als u de IBM® Aspera Connect-clientinstallatie wilt installeren, voert u de installatie uit vanuit het .msi-bestand van de IBM® Aspera Connect-clienttoepassing en volgt u de installatiewizard.

   ![](assets/aspera-download-1.png)

1. Als de client is geïnstalleerd, vernieuwt u de browserpagina en start u de downloadstappen opnieuw.

1. Als u wilt doorgaan met gebruiken **[!UICONTROL Fast Download]**, klikt u op **[!UICONTROL Allow]**. Alle geselecteerde vertoningen worden gedownload in een ZIP-map met behulp van IBM® Aspera Connect.

   Nadat het downloaden is voltooid, wordt in een dialoogvenster de locatie weergegeven waar de middelen naar het systeem van de gebruiker worden gedownload.

   ![](assets/aspera-download-2.png)

   Als u IBM® Aspera Connect niet wilt gebruiken, klikt u op **[!UICONTROL Deny]**. Indien **[!UICONTROL Fast Download]** wordt ontkend of ontbreekt, vult het systeem een Bericht van de Fout. Klik op de knop **[!UICONTROL Normal Download]** om door te gaan met het downloaden van de elementen.

>[!NOTE]
Als de **[!UICONTROL Fast Download]** De instelling wordt uitgeschakeld door de beheerder. De geselecteerde uitvoeringen worden rechtstreeks gedownload in een ZIP-map zonder IBM® Aspera Connect te gebruiken.

<!-- 
On successful completion of the download, a dialog box shows the location where assets are downloaded onto the user's system. If there is a failure, it shows error.

   >[!NOTE]
   >
   >There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab **[!UICONTROL Transfers]** within **[!UICONTROL Preferences]**. Before any download begins, provide the location in the text box **[!UICONTROL Save downloaded files to]**.


1. Log in to Brand Portal using a supported browser.
1. Browse and select the folders or assets you want to download. From the toolbar at the top, click the **[!UICONTROL Download]** icon. the **[!UICONTROL Download]** dialog appears with the **[!UICONTROL Asset(s)]** and **[!UICONTROL Enable download acceleration]** check boxes selected by default. 

   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >The functionality to send email notification with the link to download assets is presently not supported while faster downloads are enabled.

   ![](assets/fast-download-emailchk.png)

1. Click **[!UICONTROL Download]**.

   To speed up the download experience on your Brand Portal tenant account, you need to have Aspera Connect client application installed in your browser's extension.

1. **Download Aspera Connect Client**

   If Aspera Connect client is not installed on your system or the existing Aspera Connect client is out of date, a prompt is displayed on the browser page from where you can download the system-specific Aspera Connect client by selecting **[!UICONTROL Download Latest Version]**.

   ![](assets/aspera-not-launched.png)

   To download the latest version of Aspera Connect from [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), select **[!UICONTROL Download Now]** and follow the instructions.

1. **Install Aspera Connect Client**

   To install IBM Aspera Connect client setup, run the setup from  .msi  file of IBM Aspera Connect client application and follow the installation wizard.

1. Once the client is successfully installed, refresh the browser page and initiate the download steps again.

   When using Aspera Connect for the first time, the browser prompts to open the link using **[!UICONTROL IBM Aspera Connect]**. To skip this dialog in future, enable **[!UICONTROL Remember my choice for FASP links]**.

   >[!NOTE]
   >
   >This message is different on the different browsers.

1. A dialog box confirms whether to proceed the transfer or not. Select **[!UICONTROL Allow]** to begin.
To skip this dialog in future, enable **[!UICONTROL Use my choice for all connections with this host]**.
Download begins. A dialog box shows the progress of the download. Use the dialog box to **[!UICONTROL pause]**, **[!UICONTROL resume]**, or **[!UICONTROL cancel]** the download.
Aspera Connect application provides an Activity Window on the system where user can view and manage all transfer sessions. For more information, refer [Aspera Connect Client documentation](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

On successful completion of the download, a dialog box shows the location where assets are downloaded onto the user's system. If there is a failure, it shows error.

   >[!NOTE]
   >
   >There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab **[!UICONTROL Transfers]** within **[!UICONTROL Preferences]**. Before any download begins, provide the location in the text box **[!UICONTROL Save downloaded files to]**.
-->

## Bestandsversneller gebruiken in Microsoft® Edge-browser {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft® Edge wordt uitgevoerd in de Enhanced Protected Mode (EPM), waardoor communicatie met de Aspera Connect-server, op hetzelfde privénetwerk of met een vertrouwde site wordt voorkomen. Daarom wordt telkens wanneer een verbinding met de server tot stand wordt gebracht, een pop-up weergegeven.

![](assets/switchapps-msedge.png)

Als u de functie voor versnelde download wilt gebruiken op Microsoft® Edge, verwijdert u de Brand Portal-site uit de lijst met vertrouwde sites.

1. Het regelpaneel openen (**[!UICONTROL Window key + X]** selecteert u vervolgens **[!UICONTROL Control Panel]**).
1. Ga naar **[!UICONTROL Network and Internet]** > **[!UICONTROL Internet Options]**. Klik op de knop **[!UICONTROL Security]** tab.
1. Klik op de knop **[!UICONTROL Trusted sites zone]** en klik vervolgens op **[!UICONTROL Sites]**.
1. Brand Portal-site verwijderen uit de lijst.

## Voorkeuren voor Aspera Connect-client {#aspera-connect-client-preferences}

Er zijn een paar handige voorkeuren die u kunt instellen in de voorkeur voor IBM® Aspera Connect Client door met de rechtermuisknop op het pictogram te klikken en **[!UICONTROL Preferences]**.

![](assets/download_assets_frombrandportalimg19.png)

U kunt de standaarddownloadlocatie instellen.

![](assets/aspera-preferences.png)

Bovendien kan de Aspera Connect-client worden gemarkeerd om automatisch te starten bij het opstarten van het systeem, zodat de Connect-client wordt uitgevoerd en de download sneller kan worden gestart.

![](assets/aspera-automaticallylaunch.png)

## Problemen met downloadversnelling oplossen {#troubleshoot-issues-with-download-acceleration}

Als downloadversnelling niet voor u werkt, probeert u de volgende suggesties:

1. Controleer of de poorten niet geblokkeerd zijn. Gebruik Google Search om opties te zoeken waarmee u kunt controleren of poorten zijn geblokkeerd, op basis van het gebruikte besturingssysteem.  <!-- THIS URL IS 404 AND DOES NOT REDIRECT [https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/) from your computer. -->

   Als de havens niet O.K. zijn, dan bereik uit aan uw netwerkteam en zorg ervoor dat de Havens 33001 (zowel TCP &amp; UDP) niet in de firewall worden geblokkeerd.

1. Als de havens O.K. zijn, dan controleer als uw netwerk niet langzaam is, door de beschikbare bandbreedte te meten gebruikend [https://www.speedtest.net/](https://www.speedtest.net/).

   Als de bandbreedte weinig (1-10 Mbps) of in Kbps is, dan gebruik de Voorkeur van de RUIMTE en probeer om de bandbreedte te beperken gelijk aan de beschikbare bandbreedte.

   <!-- The URL in this step is giving a 404 error. 1. To confirm whether the downloads from Aspera demo server are working, use [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user).  
   (login:  asperaweb , password:  demoaspera ) -->

1. Als geen van de bovenstaande stappen voor het oplossen van problemen werkt, schakelt u de optie Downloadversnelling inschakelen uit en gebruikt u de normale download.
