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
source-git-commit: 64aa436f8416b8280f465166dbe692c300843eed
workflow-type: tm+mt
source-wordcount: '1034'
ht-degree: 2%

---


# De downloads van de Brand Portal {#guide-to-accelerate-downloads-from-brand-portal} versnellen

Brand Portal maakt het mogelijk de downloadprestaties van grote bestanden met bedrijfsmiddelen te verbeteren door deze te integreren met IBM Aspera Connect, een toepassing die op aanvraag kan worden geïnstalleerd. De toepassing gebruikt merkgebonden technologie om de overheadkosten van TCP te verwijderen en helpt overdrachtsnelheid van de activadossiers te verbeteren. Deze integratie zorgt voor een verbeterde downloadervaring.

>[!NOTE]
>
>Downloadsnelheid verschilt voor gebruikers omdat dit afhankelijk is van factoren zoals netwerkbandbreedte, serverlatentie en geografische locatie van clients.

De **[!UICONTROL Fast Download]** configuratie is door gebrek toegelaten, die beduidend de tijd vermindert om de gewenste activadossiers van het Portaal van het Merk te downloaden.

![](assets/download-configuration-old.png)

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

1. Meld u aan bij Brand Portal met behulp van een ondersteunde browser.
1. Blader naar de mappen of elementen die u wilt downloaden en selecteer deze. Klik op het pictogram **[!UICONTROL Download]** op de werkbalk boven in het scherm. Het dialoogvenster **[!UICONTROL Download]** wordt weergegeven met de selectievakjes **[!UICONTROL Asset(s)]** en **[!UICONTROL Enable download acceleration]** standaard geselecteerd.

   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >De functionaliteit voor het verzenden van e-mailmeldingen via de koppeling voor het downloaden van middelen wordt momenteel niet ondersteund, terwijl snellere downloads zijn ingeschakeld.

   ![](assets/fast-download-emailchk.png)

1. Klik op **[!UICONTROL Download]**.

   Als u de downloadervaring voor uw zakelijke portalaccount wilt versnellen, moet de clienttoepassing van Aspera Connect zijn geïnstalleerd in de browserextensie.

1. **Aspera Connect-client downloaden**

   Als Aspera Connect-client niet op uw systeem is geïnstalleerd of als de bestaande Aspera Connect-client verouderd is, wordt een vraag weergegeven op de browserpagina vanwaar u de systeemspecifieke Aspera Connect-client kunt downloaden door **[!UICONTROL Download Latest Version]** te selecteren.

   ![](assets/aspera-not-launched.png)

   Als u de meest recente versie van Aspera Connect wilt downloaden van [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), selecteert u **[!UICONTROL Download Now]** en volgt u de instructies.

1. **Aspera Connect-client installeren**

   Als u de installatie van de IBM Aspera Connect-client wilt installeren, voert u de installatie uit vanuit het .msi-bestand van de IBM Aspera Connect-clienttoepassing en volgt u de installatiewizard.

1. Als de client is geïnstalleerd, vernieuwt u de browserpagina en start u de downloadstappen opnieuw.

   Wanneer u Aspera Connect voor het eerst gebruikt, wordt de browser gevraagd om de koppeling te openen met **[!UICONTROL IBM Aspera Connect]**. Als u dit dialoogvenster in de toekomst wilt overslaan, schakelt u **[!UICONTROL Remember my choice for FASP links]** in.

   >[!NOTE]
   >
   >Dit bericht is anders in de verschillende browsers.

1. Een dialoogvenster bevestigt of de overdracht moet worden voortgezet. Selecteer **[!UICONTROL Allow]** om te beginnen.
Als u dit dialoogvenster in de toekomst wilt overslaan, schakelt u **[!UICONTROL Use my choice for all connections with this host]** in.
Het downloaden begint. In een dialoogvenster ziet u de voortgang van het downloaden. In het dialoogvenster kunt u **[!UICONTROL pause]**, **[!UICONTROL resume]** of **[!UICONTROL cancel]** de download gebruiken.
De toepassing Aspera Connect biedt een Activiteitenvenster op het systeem waarin de gebruiker alle overdrachtssessies kan weergeven en beheren. Raadpleeg de [documentatie van Aspera Connect Client](https://downloads.asperasoft.com/en/documentation/8) voor meer informatie.

![](assets/aspera-activity-window.png)

Nadat het downloaden is voltooid, wordt in een dialoogvenster de locatie weergegeven waar de middelen naar het systeem van de gebruiker worden gedownload. Als er een fout optreedt, wordt er een fout weergegeven.

>[!NOTE]
>
>Er is een bekende beperking in de clienttoepassing van Aspera Connect dat er geen vraag verschijnt om de downloadlocatie te selecteren als **[!UICONTROL Always ask me where to save downloaded files]** is ingeschakeld onder het tabblad **[!UICONTROL Transfers]** binnen **[!UICONTROL Preferences]**. Geef de locatie op in het tekstvak **[!UICONTROL Save downloaded files to]** voordat u begint met downloaden.

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
