---
title: De downloads van de Brand Portal versnellen
seo-title: De downloads van de Brand Portal versnellen
description: Verbeter downloadprestaties van Brand Portal en de gedeelde koppelingen.
seo-description: Verbeter downloadprestaties van Brand Portal en de gedeelde koppelingen.
uuid: 2871137e-6471-49a7-872a-841bd92543d1
contentOwner: mgulati
topic-tags: download-install
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 301f7a0b-5527-4aac-b731-bfc145fed0c0
translation-type: tm+mt
source-git-commit: fab0855e8d30e7b6ddf9b4ae5b2ce1fb627c81ce
workflow-type: tm+mt
source-wordcount: '999'
ht-degree: 3%

---


# De downloads van de Brand Portal {#guide-to-accelerate-downloads-from-brand-portal} versnellen

Met Adobe Experience Manager Assets Brand Portal kunt u de downloadprestaties van grote elementbestanden verbeteren door te integreren met IBM Aspera Connect, een toepassing die op aanvraag kan worden geïnstalleerd. De toepassing gebruikt merkgebonden technologie om de overheadkosten van TCP te verwijderen en helpt overdrachtsnelheid van de activadossiers te verbeteren. Deze integratie zorgt voor een verbeterde downloadervaring.

>[!NOTE]
>
>Downloadsnelheid verschilt voor gebruikers omdat dit afhankelijk is van factoren zoals netwerkbandbreedte, serverlatentie en geografische locatie van clients.

De **[!UICONTROL Fast Download]** configuratie is door gebrek toegelaten, die beduidend de tijd vermindert om de gewenste activadossiers van het Portaal van het Merk te downloaden.

![](assets/download-settings-new.png)

## Vereisten om het downloaden van bestanden te versnellen {#prerequisites-to-accelerate-file-download}

Als u de bestanden sneller wilt downloaden, moet u het volgende doen:

* Navigeer naar **[!UICONTROL Tools]** > **[!UICONTROL Download]** en controleer of de **[!UICONTROL Fast Download]**-configuratie is ingeschakeld in **[!UICONTROL Download Settings]**.
* Zorg ervoor dat poort 33001 (zowel TCP als UDP) is geopend op de firewall. Zie [IBM Aspera Connect Client documentation](https://downloads.asperasoft.com/en/documentation/8) voor meer informatie over de voorwaarden.
* [Installeer IBM Aspera Connect 3.9.9](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html) in de browserextensie met beheerdersrechten.
* Zie [IBM Aspera Connect platform support matrix](https://www.asperasoft.com/company/support/transfer-clients/) voor platformondersteuning van de Aspera-overdrachtclient.

## Domeinen {#download-domains} downloaden

Hier volgen de downloaddomeinen voor verschillende geografische gebieden:

| Gebiedscode | Domein |
|---|---|
| NA OF1 | downloads-na1.brand-portal.adobe.com |
| NA VA5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN2 | downloads-apac1.brand-portal.adobe.com |

## Voorbeeld van downloadprestaties met gebruik van bestandsaccelerator {#expected-download-performance-using-file-accelerator}

In de volgende tabel worden de downloadprestaties voor 2 GB-bestanden weergegeven met de Aspera Connect-bestandsdownloadaccelerator:

*De waargenomen resultaten variëren toe te schrijven aan factoren zoals netwerkbandbreedte, serverlatentie, en cliëntplaats, aangezien de server van het Portaal van het Merk bij Oregon (Verenigde Staten) is.*

| Clientlocatie | Latentie tussen client en server (milliseconden) | Snelheid met Aspera Connect File Transfer Accelerator (MBps) | Tijd die nodig is om 2 GB bestand te downloaden met Aspera File Transfer Accelerator (seconden) |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| V.S. West (N. Californië) | 18 | 36 | 57 |
| V.S. West (Oregon) | 42 | 36 | 57 |
| V.S. Oost (N. Virginia) | 85 | 35 | 58 |
| APAC (Tokio) | 124 | 36 | 57 |
| Noida (India) | 275 | 13,36 | 153 |
| Sydney | 175 | 29 | 70 |
| Londen | 179 | 35 | 58 |
| Singapore | 196 | 34 | 60 |

## Workflow downloaden met bestandsaccelerator {#download-workflow-using-file-accelerator}

Middelen sneller downloaden van Brand Portal:

1. Meld u aan bij uw Brand Portal-huurder. Standaard wordt de weergave **[!UICONTROL Files]** geopend, die alle gepubliceerde elementen en mappen bevat.

   Voer een van de volgende handelingen uit:

   * Selecteer de elementen of mappen die u wilt downloaden. Klik op het pictogram **[!UICONTROL Download]** op de werkbalk boven in het scherm.

      ![select-multiple-assets](assets/select-assets-new.png)

   * Als u specifieke elementuitvoeringen van een element wilt downloaden, plaatst u de aanwijzer boven het element en klikt u op het pictogram **[!UICONTROL Download]** in de miniaturen van de snelle handeling.

      ![select-element](assets/select-asset.png)

1. Het dialoogvenster **[!UICONTROL Download]** met alle geselecteerde elementen wordt geopend.

   Selecteer het selectievakje **[!UICONTROL Create separate folder for each asset]** om de maphiërarchie van het Brand Portal te behouden tijdens het downloaden van elementen.

   De downloadknop geeft het aantal geselecteerde items weer. Als u klaar bent met het toepassen van de regels, klikt u op **[!UICONTROL Download items]**. Zie [Elementen downloaden](../using/brand-portal-download-assets.md#download-assets) voor meer informatie over het toepassen van regels.

   ![download-dialog](assets/download-dialog-box-new.png)

1. Standaard is de instelling **[!UICONTROL Fast Download]** ingeschakeld in **[!UICONTROL Download Settings]**. Daarom wordt een bevestigingsvenster weergegeven waarin u middelen kunt downloaden met IBM Aspera Connect.

   Als u de middelen voor het eerst downloadt en IBM Aspera Connect niet in uw browser heeft geïnstalleerd of als de bestaande versie verouderd is, wordt u gevraagd [de Aspera-downloadaccelerator](https://www.ibm.com/support/knowledgecenter/SSXMX3_3.9.9/kc/connect_welcome.html) te installeren.

   ![](assets/aspera-not-launched.png)

1. **Aspera Connect-client installeren**

   Als u de installatie van de IBM Aspera Connect-client wilt installeren, voert u de installatie uit vanuit het .msi-bestand van de IBM Aspera Connect-clienttoepassing en volgt u de installatiewizard.

   ![](assets/aspera-download-1.png)

1. Als de client is geïnstalleerd, vernieuwt u de browserpagina en start u de downloadstappen opnieuw.

1. Als u **[!UICONTROL Fast Download]** wilt blijven gebruiken, klikt u op **[!UICONTROL Allow]**. Alle geselecteerde vertoningen worden gedownload in een ZIP-map met behulp van IBM Aspera Connect.

   Nadat het downloaden is voltooid, wordt in een dialoogvenster de locatie weergegeven waar de middelen naar het systeem van de gebruiker worden gedownload.

   ![](assets/aspera-download-2.png)

   Als u IBM Aspera Connect niet wilt gebruiken, klikt u op **[!UICONTROL Deny]**. Als **[!UICONTROL Fast Download]** wordt ontkend of ontbreekt, bevolkt het systeem een Bericht van de Fout. Klik op de knop **[!UICONTROL Normal Download]** om door te gaan met het downloaden van de elementen.

>[!NOTE]
>
>Als de instelling **[!UICONTROL Fast Download]** door de beheerder is uitgeschakeld, worden de geselecteerde uitvoeringen rechtstreeks gedownload in een ZIP-map zonder gebruik te maken van IBM Aspera Connect.

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

## Bestandsversneller gebruiken in Microsoft Edge-browser {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge wordt uitgevoerd in de EPM-modus (Enhanced Protected Mode), waardoor communicatie met de Aspera Connect-server, op hetzelfde privénetwerk of met een vertrouwde site wordt voorkomen. Daarom wordt telkens wanneer een verbinding met de server tot stand wordt gebracht, een pop-up weergegeven.

![](assets/switchapps-msedge.png)

Als u de functie voor versnelde download wilt gebruiken op Microsoft Edge, verwijdert u de Brand Portal-site uit de lijst met vertrouwde sites.

1. Open het Configuratiescherm (**[!UICONTROL Window key + X]**, dan selecteer **[!UICONTROL Control Panel]**).
1. Ga naar **[!UICONTROL Network and Internet]** > **[!UICONTROL Internet Options]**. Klik op het tabblad **[!UICONTROL Security]**.
1. Klik **[!UICONTROL Trusted sites zone]**, dan klik **[!UICONTROL Sites]**.
1. Merk Portal-site verwijderen uit de lijst.

## Voorkeuren voor Adobe Connect-client {#aspera-connect-client-preferences}

Er zijn een paar handige voorkeuren die u kunt instellen in de voorkeur voor IBM Aspera Connect Client door met de rechtermuisknop op het pictogram te klikken en **[!UICONTROL Preferences]** te selecteren.

![](assets/download_assets_frombrandportalimg19.png)

U kunt de standaarddownloadlocatie instellen.

![](assets/aspera-preferences.png)

Bovendien kan de Aspera Connect-client worden gemarkeerd om automatisch te starten bij het opstarten van het systeem, zodat de Connect-client wordt uitgevoerd en de download sneller kan worden gestart.

![](assets/aspera-automaticallylaunch.png)

## Problemen met downloadversnelling {#troubleshoot-issues-with-download-acceleration} oplossen

Als de downloadversnelling niet voor u werkt, volgt u deze stappen om problemen op te lossen:

1. Controleer of poorten niet worden geblokkeerd door [https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/) van uw computer te bezoeken.

   Als de havens niet O.K. zijn, dan bereik uit aan uw netwerkteam en zorg ervoor dat de Havens 33001 (zowel TCP &amp; UDP) niet in de firewall worden geblokkeerd.

1. Als de havens O.K. zijn dan controleer als uw netwerk niet langzaam is, door de beschikbare bandbreedte te meten gebruikend [https://www.speedtest.net/](https://www.speedtest.net/).

   Als de bandbreedte weinig (1-10 Mbps) of in Kbps is, dan gebruik de Voorkeur van de RUIMTE en probeer om de bandbreedte te beperken gelijk aan de beschikbare bandbreedte.

1. Als u wilt controleren of de downloads van de Aspera-demoserver werken, gebruikt u [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user).\
   (aanmelden:  asperaweb, wachtwoord:  demoaspera )

1. Als geen van de bovenstaande stappen voor het oplossen van problemen werkt, schakelt u de optie Downloadversnelling inschakelen uit en gebruikt u de normale download.
