---
title: Werken met rapporten
description: Experience Manager Assets Brand Portal-beheerders kunnen rapporten weergeven over het gebruik van Brand Portal en rapporten maken, beheren en weergeven over gedownloade, verlopen, gepubliceerde en via Brand Portal gedeelde elementen.
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 03d0292c-23c2-4ea0-9781-eb27768e6c33
source-git-commit: 133ea1fc342e4460e7d0661205c7411a509143eb
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 0%

---

# Werken met rapporten {#work-with-reports}

De rapportagefunctie is van essentieel belang voor het beoordelen van het gebruik van Brand Portal en het weten hoe interne en externe gebruikers met goedgekeurde middelen omgaan. Beheerders kunnen het Brand Portal-gebruiksrapport weergeven. Dit rapport is altijd beschikbaar op de pagina Asset Reports. Rapporten voor gebruikersaanmeldingen en gedownloade, verlopen, gepubliceerde en via koppelingen gedeelde elementen kunnen echter worden gegenereerd en weergegeven vanaf de pagina Asset Reports. Deze rapporten zijn nuttig in het analyseren van middelenplaatsing, die u zeer belangrijke succesmetriek laat afleiden om de goedkeuring van goedgekeurde activa binnen en buiten uw organisatie te meten.

De interface van het rapportbeheer is intuïtief en omvat fijnkorrelige opties en controles om tot bewaarde rapporten toegang te hebben. U kunt rapporten weergeven, downloaden of verwijderen van de pagina Asset Reports, waar alle eerder gegenereerde rapporten worden weergegeven.

## Rapporten weergeven {#view-reports}

Voer de volgende stappen uit om een rapport weer te geven:

1. Klik in de werkbalk boven in het scherm op het logo van de Experience Manager voor toegang tot de beheergereedschappen.

   ![](assets/aemlogo.png)

1. Klik in het deelvenster met beheergereedschappen op **[!UICONTROL Create/Manage Reports]** om de pagina **[!UICONTROL Asset Reports]** te openen.

   ![](assets/access-asset-reports.png)

1. Open het **[!UICONTROL Usage]** -rapport en andere gegenereerde rapporten op de pagina Asset Reports.

   >[!NOTE]
   >
   >Gebruiksrapport is een standaardrapport dat in Brand Portal wordt gegenereerd. Kan niet maken of verwijderen. U kunt echter wel de rapporten Download, Expiration, Publish, `Link Share` en gebruikersaanmelding maken, downloaden en verwijderen.

   Klik op de rapportkoppeling om een rapport weer te geven. U kunt ook het rapport selecteren en op het pictogram Weergave op de werkbalk klikken.

   In **[!UICONTROL Usage Report]** wordt informatie weergegeven over het aantal actieve Brand Portal-gebruikers, de opslagruimte die door alle elementen wordt ingenomen en het totale aantal elementen in Brand Portal. De Brand Portal-gebruikers die niet aan een productprofiel in de Admin Console zijn toegewezen, worden beschouwd als inactieve gebruikers en worden niet weergegeven in de **[!UICONTROL Usage Report]** .
Het rapport toont ook de toegestane capaciteit voor elk van deze informatiemetriek.

   ![](assets/usage-report.png)

   Het **[!UICONTROL User Logins]** -rapport bevat informatie over de gebruikers die zich hebben aangemeld bij Brand Portal. Het rapport toont vertoningsnamen, e-mail IDs, persona&#39;s (admin, kijker, redacteur, gast), groepen, laatste login, activiteitenstatus, en login telling van elke gebruiker van de plaatsing van Brand Portal 6.4.2 tot de tijd van rapportgeneratie.

   ![](assets/user-logins.png)

   **[!UICONTROL Download]** bevat een lijst met alle elementen die in een bepaalde datum en tijd zijn gedownload.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >In het middelenrapport **[!UICONTROL Download]** worden alleen de elementen weergegeven die afzonderlijk zijn geselecteerd en gedownload van Brand Portal. Als een gebruiker een map met elementen heeft gedownload, geeft het rapport de map of de elementen in de map niet weer.

   In het rapport **[!UICONTROL Expiration]** worden alle elementen weergegeven en weergegeven die in een bepaald tijdsbestek zijn verlopen.

   ![](assets/expiration-report.png)

   **[!UICONTROL Publish]** geeft een overzicht en informatie over alle elementen die in een opgegeven tijdsperiode van Experience Manager Assets naar Brand Portal zijn gepubliceerd.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >In het Publish-rapport wordt geen informatie weergegeven over inhoudsfragmenten, omdat de inhoudsfragmenten niet naar de Brand Portal kunnen worden gepubliceerd.

   Het **[!UICONTROL Link Share]** -rapport bevat een lijst met alle elementen die via koppelingen vanuit de Brand Portal-interface in een bepaald tijdframe worden gedeeld. Het rapport geeft aan wanneer het element via een koppeling is gedeeld, welke gebruiker het heeft gedeeld en op welke vervaldatum van de koppeling is overgegaan. Het meldt ook het aantal gedeelde verbindingen voor de huurder en de gebruikers. De kolommen van het Rapport van het Aandeel van de Verbinding zijn niet klantgericht.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >Het rapport Delen van koppeling geeft geen gebruikers weer die toegang hebben tot het element dat via de koppeling wordt gedeeld of dat het element via de koppeling heeft gedownload.
   >
   >Voor het bijhouden van downloads via de gedeelde koppeling moet u een downloadrapport genereren nadat u de optie **[!UICONTROL Only Link Share Downloads]** op de pagina **[!UICONTROL Create Report]** hebt geselecteerd. De gebruiker (Gedownload door) is in dit geval echter anoniem.

## Rapporten genereren {#generate-reports}

Beheerders kunnen de volgende standaardrapporten genereren en beheren. Na generatie, worden de rapporten bewaard voor [ recentere toegang ](../using/brand-portal-reports.md#main-pars-header).

* Aanmeldingsgegevens gebruiker
* Downloaden
* Verlopen
* Publish
* Delen van koppeling

De kolommen in het rapport Download, Expiration en Publish kunnen worden aangepast voor weergave. Voer de volgende stappen uit om een rapport te genereren:

1. Klik in de werkbalk boven in het scherm op het logo van de Experience Manager voor toegang tot de beheergereedschappen.

1. Klik in het deelvenster met beheergereedschappen op **[!UICONTROL Create/Manage Reports]** om de pagina **[!UICONTROL Asset Reports]** te openen.

   ![](assets/asset-reports.png)

1. Klik op **[!UICONTROL Create]** op de pagina Elementrapporten.
1. Selecteer op de pagina **[!UICONTROL Create Report]** een rapport dat u wilt maken en klik op **[!UICONTROL Next]** .

   ![](assets/crete-report.png)

1. Configureer rapportdetails. Geef een titel, beschrijving, mapstructuur op (waar het rapport statistische gegevens moet uitvoeren en genereren) en geef een datumbereik op voor **[!UICONTROL Download]** -, **[!UICONTROL Expiration]** - en **[!UICONTROL Publish]** -rapporten.

   ![](assets/create-report-page.png)

   Voor het **[!UICONTROL Link Share]** -rapport zijn alleen de parameters titel, beschrijving en datumbereik nodig.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >Wanneer u het rapport genereert, worden speciale tekens `#` en `%` in de titel vervangen door een afbreekstreepje (-).

1. Klik op **[!UICONTROL Next]** om de kolommen Download-, Expiration- en Publish-rapporten te configureren.
1. Schakel de desbetreffende selectievakjes naar wens in of uit. Als u bijvoorbeeld de namen van gebruikers (die elementen hebben gedownload) in het **[!UICONTROL Download]** -rapport wilt weergeven, selecteert u **[!UICONTROL Downloaded By]** . De volgende afbeelding illustreert het selecteren van de standaardkolommen in het rapport Downloaden.

   ![](assets/createdownloadreport.png)

   U kunt ook Aangepaste kolommen aan deze rapporten toevoegen om meer gegevens voor uw aangepaste vereisten weer te geven.

   Ga als volgt te werk om aangepaste kolommen toe te voegen aan het rapport Downloaden, Publish of Verlopen:

   1. Als u een aangepaste kolom wilt weergeven, klikt u op **[!UICONTROL Add]** in [!UICONTROL Custom Columns] .
   1. Geef de naam van de kolom op in het veld **[!UICONTROL Column Name]** .
   1. Selecteer de eigenschap waaraan de kolom moet worden toegewezen met een eigenschapkiezer.

      ![](assets/property-picker.png)
U kunt ook het pad typen in het veld Pad eigenschap.

      ![](assets/property-path.png)

      Om meer Kolommen van de Douane toe te voegen, klik **toevoegen** en herhaal stappen 2 en 3.

1. Klik op **[!UICONTROL Create]**. Een bericht meldt dat de rapportgeneratie is in werking gesteld.

## Rapporten downloaden {#download-reports}

Voer een van de volgende handelingen uit om een rapport op te slaan en te downloaden als een CSV-bestand:

* Selecteer een rapport op de pagina Elementrapporten, en klik **[!UICONTROL Download]** van de toolbar bij de bovenkant.

![](assets/download-asset-report.png)

* Open een rapport op de pagina Asset Reports. Selecteer de optie **[!UICONTROL Download]** boven aan de rapportpagina.

![](assets/download-report-fromwithin.png)

## Rapporten verwijderen {#delete-reports}

Als u een bestaand rapport wilt verwijderen, selecteert u het rapport op de pagina **[!UICONTROL Asset Reports]** en klikt u **[!UICONTROL Delete]** op de werkbalk boven in het scherm.

>[!NOTE]
>
>**[!UICONTROL Usage]** -rapport kan niet worden verwijderd.
