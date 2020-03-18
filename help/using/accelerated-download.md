---
title: Speed up the Brand Portal downloads
seo-title: De downloads van de Brand Portal versnellen
description: Verbeter downloadprestaties van Brand Portal en de gedeelde koppelingen.
seo-description: Enhance download performance from Brand Portal and the shared links.
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: mgulati
topic-tags: download-install
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bfc145fed0c0
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Speed up the Brand Portal downloads {#guide-to-accelerate-downloads-from-brand-portal}

Brand Portal allows enhancing the download performance of large asset files by integrating with IBM Aspera Connect, which is an install-on-demand application. The application uses proprietary technology to remove TCP overheads and helps improve transfer speed of the asset files. Deze integratie zorgt voor een verbeterde downloadervaring.

>[!NOTE]
>
>Downloadsnelheid verschilt voor gebruikers omdat dit afhankelijk is van factoren zoals netwerkbandbreedte, serverlatentie en geografische locatie van clients.

Als deze optie is ingeschakeld, kunnen gebruikers van Brand Portal de tijd die nodig is om de gewenste elementbestanden te downloaden, aanzienlijk verkorten via Brand Portal of de gedeelde koppeling door de Aspera Connect-client te installeren.

![](assets/enable-fast-file-download.png)

## Vereisten om bestanden sneller te downloaden {#prerequisites-to-accelerate-file-download}

Als u de bestanden sneller wilt downloaden, moet u het volgende doen:

* **[!UICONTROL Enable Download Acceleration]** (standaard uitgeschakeld) in [!UICONTROL General Settings] het deelvenster met beheergereedschappen.
* Poort 33001 (zowel TCP als UDP) is open op de firewall. Raadpleeg de documentatie bij [Aspera Connect Client voor meer informatie over de voorwaarden](https://downloads.asperasoft.com/en/documentation/8).
* Installeer Aspera Connect met behulp van beheerdersrechten.
* Raadpleeg de ondersteuningsmatrix van [Aspera Connect-platform voor platformondersteuning van Aspera Transfer Client](https://www.asperasoft.com/company/support/transfer-clients/).

## Domeinen downloaden {#download-domains}

Hier volgen de downloaddomeinen voor verschillende geografische gebieden:

| Gebiedscode | Domein |
|---|---|
| NA OF1 | downloads-na1.brand-portal.adobe.com |
| NA VA5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

## Sample download performance using file accelerator {#expected-download-performance-using-file-accelerator}

The following table shows download performance for 2 GB file using Aspera Connect file download accelerator:

*De waargenomen resultaten variëren toe te schrijven aan factoren zoals netwerkbandbreedte, serverlatentie, en cliëntplaats, aangezien de server van het Portaal van het Merk bij Oregon (Verenigde Staten) is.*

| Client location | Latentie tussen client en server (milliseconden) | Snelheid met Aspera Connect File Transfer Accelerator (MBps) | Tijd die nodig is om 2 GB bestand te downloaden met Aspera File Transfer Accelerator (seconden) |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| V.S. West (N. Californië) | 18 | 36 | 57 |
| V.S. West (Oregon) | 42 | 36 | 57 |
| V.S. Oost (N. Virginia) | 85 | 35 | 58 |
| APAC (Tokio) | 124 | 36 | 57 |
| Noida (India) | 275 | 13.36 | 153 |
| Sydney | 175 | 29 | 70 |
| London | 179 | 35 | 58 |
| Singapore | 196 | 34 | 60 |

## Download workflow using file accelerator {#download-workflow-using-file-accelerator}

To download assets faster from Brand Portal:

1. Meld u aan bij Brand Portal met behulp van een ondersteunde browser.
1. Browse and select the desired asset file, folder, or collection to download. Tik/klik op de downloadoptie.
Het dialoogvenster Downloaden wordt geopend met de optie [Downloadversnelling] inschakelen geselecteerd.
   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >De functionaliteit voor het verzenden van e-mailmeldingen via de koppeling voor het downloaden van middelen wordt momenteel niet ondersteund, terwijl snellere downloads zijn ingeschakeld.

   ![](assets/fast-download-emailchk.png)

1. Tik/klik op de **[!UICONTROL Download]** optie.
Als u de downloadervaring voor uw zakelijke portalaccount wilt versnellen, moet de clienttoepassing van Aspera Connect op uw systeem zijn geïnstalleerd.

1. **Download Aspera Connect Client** Als de Aspera Connect-client niet op uw systeem is geïnstalleerd of de bestaande geïnstalleerde Aspera Connect-client verouderd is, wordt een vraag weergegeven op de browserpagina vanwaar u de systeemspecifieke Aspera Connect-client kunt downloaden door **[!UICONTROL Download Latest Version]** te selecteren.

   ![](assets/aspera-not-launched.png)

   Als u de meest recente versie van Aspera Connect wilt downloaden van [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), selecteert **[!UICONTROL Download Now]** en volgt u de instructies.

1. **Installeer Aspera Connect Client** To install IBM Aspera Connect client setup, voer de installatie uit vanuit het .msi-bestand van de IBM Aspera Connect-clienttoepassing en volg de installatiewizard.

1. Wanneer de client is geïnstalleerd, vernieuwt u de browserpagina en start u de downloadstappen opnieuw of selecteert u **[!UICONTROL Restart]** in het **[!UICONTROL Download]** dialoogvenster Middelen (Stap 2).
Wanneer u Aspera Connect voor het eerst gebruikt, wordt de browser gevraagd om de koppeling te openen met **[!UICONTROL IBM Aspera Connect]**. Schakel deze optie in als u dit dialoogvenster in de toekomst wilt overslaan. **[!UICONTROL Remember my choice for FASP links]**

   >[!NOTE]
   >
   >Dit bericht is anders in de verschillende browsers.

1. Een dialoogvenster bevestigt of de overdracht moet worden voortgezet. Select **[!UICONTROL Allow]** to begin.
To skip this dialog in future, enable **[!UICONTROL Use my choice for all connections with this host]**.
Download begins. A dialog box shows the progress of the download. Gebruik het dialoogvenster om te downloaden **[!UICONTROL pause]**, **[!UICONTROL resume]** of **[!UICONTROL cancel]** te downloaden.
Aspera Connect application provides an Activity Window on the system where user can view and manage all transfer sessions. Raadpleeg de documentatie bij [](https://downloads.asperasoft.com/en/documentation/8)Aspera Connect Client voor meer informatie.

![](assets/aspera-activity-window.png)

On successful completion of the download, a dialog box shows the location where assets are downloaded onto the user&#39;s system. Als er een fout optreedt, wordt er een fout weergegeven.

>[!NOTE]
>
>There is a known limitation in Aspera Connect client application that no prompt to select download location appears if **[!UICONTROL Always ask me where to save downloaded files]** is enabled under the tab [!UICONTROL Transfers] within [!UICONTROL Preferences]. Before any download begins, provide the location in the text box **[!UICONTROL Save downloaded files to]**.

## Bestandsversneller gebruiken in Microsoft Edge-browser {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge wordt uitgevoerd in de EPM-modus (Enhanced Protected Mode), waardoor communicatie met de Aspera Connect-server, op hetzelfde privénetwerk of met een vertrouwde site wordt voorkomen. Daarom wordt telkens wanneer een verbinding met de server tot stand wordt gebracht, een pop-up weergegeven.

![](assets/switchapps-msedge.png)

Als u de functie voor versnelde download wilt gebruiken op Microsoft Edge, verwijdert u de Brand Portal-site uit de lijst met vertrouwde sites.

1. Open het Configuratiescherm (druk op **[!UICONTROL Window key + X]** en selecteer **[!UICONTROL Control Panel]**).
1. Ga naar **[!UICONTROL Network and Internet > Internet Options]**. Click the **[!UICONTROL Security]** tab.
1. Klik op de knop **[!UICONTROL Trusted sites zone]** en klik vervolgens op **[!UICONTROL Sites]**.
1. Merk Portal-site verwijderen uit de lijst.

## Voorkeuren voor Aspera Connect-client {#aspera-connect-client-preferences}

Er zijn een paar handige voorkeuren die u kunt instellen in de voorkeur voor IBM Aspera Connect Client door met de rechtermuisknop op het pictogram te klikken en de optie **[!UICONTROL Preferences]**.

![](assets/download_assets_frombrandportalimg19.png)

U kunt de standaarddownloadlocatie instellen.

![](assets/aspera-preferences.png)

Bovendien kan de Aspera Connect-client worden gemarkeerd om automatisch te starten bij het opstarten van het systeem, zodat de Connect-client wordt uitgevoerd en de download sneller kan worden gestart.

![](assets/aspera-automaticallylaunch.png)

## Problemen met downloadversnelling oplossen {#troubleshoot-issues-with-download-acceleration}

Als de downloadversnelling niet voor u werkt, volgt u deze stappen om problemen op te lossen:

1. Check that ports are not blocked, by visiting [https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/) from your machine.

   If ports are not OK, then reach out to your network team and ensure that Ports 33001 (both TCP &amp; UDP) are not blocked in the firewall.

1. If the ports are OK then check if your network is not slow, by measuring the available bandwidth using [https://www.speedtest.net/](https://www.speedtest.net/).

   If the bandwidth is a few (1-10 Mbps) or in Kbps, then use Aspera Preferences and try to limit the bandwidth equal to the available bandwidth.

1. Als u wilt controleren of de downloads van de Aspera-demoserver werken, gebruikt u [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user).\
   (login:  asperaweb , password:  demoaspera )

1. Als geen van de bovenstaande stappen voor het oplossen van problemen werkt, schakelt u de optie Downloadversnelling inschakelen uit en gebruikt u de normale download.
