---
title: Overzicht van de AEM Assets Brand Portal
seo-title: Overzicht van de AEM Assets Brand Portal
description: Met AEM Assets Brand Portal kunt u eenvoudig goedgekeurde creatieve middelen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten.
seo-description: Met AEM Assets Brand Portal kunt u eenvoudig goedgekeurde creatieve middelen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
translation-type: tm+mt
source-git-commit: 9169407bbbfabd94be31c89c028be64e55afc064

---


# Overzicht van de AEM Assets Brand Portal {#overview-of-aem-assets-brand-portal}

Als markator, moet u soms met kanaalpartners en interne bedrijfsgebruikers samenwerken om, relevante digitale inhoud snel tot stand te brengen te beheren en te leveren aan klanten. De tijdige levering van relevante inhoud over de volledige klantenreis is kritiek aan het drijven van grotere vraag, omzetting, overeenkomst, en klantenloyaliteit.

Het is echter een uitdaging om oplossingen te ontwikkelen die efficiënte en veilige delen van goedgekeurde merklogo&#39;s, richtlijnen, campagnemiddelen of productschoten met uitgebreide interne teams, partners en wederverkopers ondersteunen.

**Het Brand Portal** van Adobe Experience Manager (AEM) is gericht op de behoefte van de markt om effectief samen te werken met de wereldwijd gedistribueerde gebruikers van het Brand Portal door mogelijkheden voor middelendistributie en middelenbijdragen te bieden.

Met Asset Distribution kunt u eenvoudig goedgekeurde creatieve elementen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten. Terwijl gebruikers van het Brand Portal met behulp van Asset Contribution elementen kunnen uploaden naar het Brand Portal en kunnen publiceren naar AEM Assets, zonder dat ze toegang hoeven te hebben tot de omgeving van de auteur. De bijdragefunctie wordt genoemd als **Middelen**. Samen verbetert het de algemene ervaring van het Brand Portal op het gebied van de distributie van activa en de bijdrage van de gebruikers van het Brand Portal (externe agentschappen/teams), versnelt het de tijd-aan-markt voor activa, en vermindert het risico van niet-naleving en onbevoegde toegang.
Zie [Asset Sourcing in Brand Portal](brand-portal-asset-sourcing.md).

Met de browsergebaseerde portalomgeving kunt u elementen gemakkelijk uploaden, doorbladeren, zoeken, voorvertonen en exporteren in een goedgekeurde indeling.

## AEM-middelen configureren met Brand Portal {#configure-brand-portal}

Adobe Experience Manager-middelen (AEM) worden geconfigureerd met Brand Portal via Adobe I/O, dat een IMS-token aanschaft voor toestemming van uw Brand Portal-huurder.

>[!NOTE]
>
>AEM Assets configureren met Brand Portal via Adobe I/O wordt ondersteund op AEM Assets Cloud Service, AEM Assets 6.3 en hoger.

### Vereisten om AEM-middelen te configureren met Brand Portal {#prerequisites}

U hebt het volgende nodig om AEM-middelen te configureren met Brand Portal:

* Een AEM Assets-instantie die wordt uitgevoerd.
* URL van medewerker van Brand Portal.
* Een gebruiker met de bevoegdheden van de systeembeheerder op de IMS-organisatie van de Poorthuurder van het Merk.

Zie AEM-elementen [configureren met Brand Poral](../using/configure-aem-assets-with-brand-portal.md)voor meer informatie.

## Personen van gebruikers in Brand Portal {#Personas}

Het Portaal van het merk steunt de volgende gebruikersrollen:

* Gastgebruiker
* Viewer
* Editor
* Beheerder

De volgende lijst maakt een lijst van de taken die de gebruikers in deze rollen kunnen uitvoeren:

|  | **Bladeren** | **Zoeken** | **Downloaden** | **Mappen delen** | **Een verzameling delen** | **Elementen delen als koppeling** | **Toegang tot beheerhulpprogramma&#39;s** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Gastgebruiker** | ✓* | ✓* | ✓* | x | x | x | x |
| **Viewer** | ✓ | ✓ | ✓ | x | x | x | x |
| **Editor** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Beheerder** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

* Gastgebruikers kunnen alleen in openbare mappen en verzamelingen bladeren, er toegang toe hebben en er naar zoeken.

### Gastgebruiker {#guest-user}

Om het even welke gebruiker die beperkte toegang tot activa op het Portaal van het Merk heeft zonder authentificatie te ondergaan is een gastgebruiker. De gastzitting staat gebruikers toegang tot openbare omslagen en inzamelingen toe. Als gastgebruiker, kunt u door activa details doorbladeren en volledige activamening van leden van openbare omslagen en inzamelingen hebben. U kunt openbare middelen zoeken, downloaden en toevoegen aan [!UICONTROL lichtbakverzameling] .

De gastsessie beperkt u echter het maken van verzamelingen en opgeslagen zoekopdrachten en deelt deze verder. Gebruikers in een gastsessie hebben geen toegang tot de instellingen voor mappen en verzamelingen en kunnen geen elementen delen als koppeling. Hier is een lijst van taken die een gastgebruiker kan uitvoeren:

[Bladeren en openbare middelen openen](browse-assets-brand-portal.md)

[Openbare middelen zoeken](brand-portal-searching.md)

[Overheidsmiddelen downloaden](brand-portal-download-users.md)

[Elementen toevoegen aan [!UICONTROL lichtbak]](brand-portal-light-box.md#add-assets-to-lightbox)

### Viewer {#viewer}

Een standaardgebruiker in Brand Portal is doorgaans een gebruiker met de rol van Viewer. Een gebruiker met deze rol heeft toegang tot toegestane mappen, verzamelingen en elementen. De gebruiker kan ook naar elementen (oorspronkelijke of specifieke vertoningen) bladeren, deze voorvertonen, downloaden en exporteren, accountinstellingen configureren en naar elementen zoeken. Hier volgt een lijst met taken die een viewer kan uitvoeren:

[Bladeren door elementen](browse-assets-brand-portal.md)

[Middelen zoeken](brand-portal-searching.md)

[Elementen downloaden](brand-portal-download-users.md)

### Editor {#editor}

Een gebruiker met de rol van Editor kan alle taken uitvoeren die een Viewer kan uitvoeren. Bovendien kunnen de Editor en de Editor de bestanden en mappen weergeven die een beheerder deelt. De gebruiker met de rol van een Editor kan ook inhoud (bestanden, mappen, verzamelingen) met anderen delen.

Naast de taken die een Viewer kan uitvoeren, kan een Editor de volgende extra taken uitvoeren:

[Mappen delen](brand-portal-sharing-folders.md)

[Een verzameling delen](brand-portal-share-collection.md)

[Elementen delen als koppeling](brand-portal-link-share.md)

### Beheerder {#administrator}

Een beheerder bevat een gebruiker die is gemarkeerd als systeembeheerder of beheerder van het Brand Portal-product in de [!UICONTROL beheerconsole]. Een beheerder kan systeembeheerders en gebruikers toevoegen en verwijderen, voorinstellingen definiëren, e-mail verzenden naar gebruikers en portaalgebruik en opslagrapporten weergeven.

Een beheerder kan alle taken uitvoeren die een Redacteur de volgende extra taken kan uitvoeren:

[Gebruikers, groepen en gebruikersrollen beheren](brand-portal-adding-users.md)

[Achtergrond, paginakoppen en e-mails aanpassen](brand-portal-branding.md)

[Aangepaste zoekfacetten gebruiken](brand-portal-search-facets.md)

[Het metagegevensschema gebruiken](brand-portal-metadata-schemas.md)

[Voorinstellingen voor afbeeldingen of dynamische uitvoeringen toepassen](brand-portal-image-presets.md)

[Werken met rapporten](brand-portal-reports.md)

Naast de bovenstaande taken kan een auteur in AEM Assets de volgende taken uitvoeren:

[AEM-middelen configureren met Brand Portal](../using/configure-aem-assets-with-brand-portal.md)

[Mappen publiceren naar Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Verzamelingen publiceren naar Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Alternatieve alias voor Brand Portal-URL {#tenant-alias-for-portal-url}

Merkportal 6.4.3 en hoger kunnen organisaties één alternatieve (alias) URL hebben voor de bestaande URL van hun Poorthuurder. De alias-URL kan worden gemaakt door een alternatief voorvoegsel in de URL te plaatsen.\
Merk op dat alleen het voorvoegsel van de Brand Portal-URL kan worden aangepast en niet de volledige URL. Zo kan een organisatie met bestaande domeingeomettrix. **[!UICONTROL brand-portal.adobe.com]** op verzoek **[!UICONTROL geomettrixinc.brand-portal.adobe.com]** maken.

Nochtans, kan de instantie van de Auteur AEM slechts met huurder identiteitskaart URL en niet met huurder alias (afwisselende) URL worden [gevormd](../using/configure-aem-assets-with-brand-portal.md) .

>[!NOTE]
>
>Om een alias voor huurdersnaam in bestaande portaal URL te krijgen, moeten de organisaties de steun van Adobe met een nieuw verzoek van de huurdersalias contacteren. Dit verzoek wordt verwerkt door eerst te controleren of de alias beschikbaar is en vervolgens de alias te maken.
>
>Als u de oude alias wilt vervangen of de oude alias wilt verwijderen, moet hetzelfde proces worden gevolgd.

## Toegang aanvragen tot Brand Portal {#request-access-to-brand-portal}

Gebruikers kunnen toegang tot het Brand Portal aanvragen via het aanmeldingsscherm. Deze aanvragen worden verzonden naar beheerders van het Brand Portal, die via de Adobe [!UICONTROL Admin Console]toegang verlenen aan gebruikers. Nadat toegang is verleend, ontvangen gebruikers een e-mailbericht.

Ga als volgt te werk om toegang aan te vragen:

1. Van de de login pagina van het Portaal van het Merk, uitgezochte **[!UICONTROL Klik hier]** die aan Toegang beantwoordt **[!UICONTROL nodig?]**. Nochtans, om de gastzitting in te gaan, selecteer **[!UICONTROL Klik hier]** die aan de Toegang van de **[!UICONTROL Gast beantwoordt?]**.

   ![Meldingsscherm voor portal Merk](assets/bp-login-requestaccess.png)

   De pagina [!UICONTROL Verzoek om toegang] wordt geopend.

1. Als u toegang wilt aanvragen tot het Brand Portal van een organisatie, hebt u een geldige [!UICONTROL Adobe-id], [!UICONTROL Enterprise-id]of [!UICONTROL federated-id]nodig.

   Meld u aan met uw id (scenario 1) of maak een [!UICONTROL Adobe-id] (scenario 2) op de pagina Toegang  aanvragen:<br />
   ![[!UICONTROL Toegang aanvragen]](assets/bplogin_request_access_2.png)

   **Scenario 1**
   1. Als u een [!UICONTROL Adobe-id], [!UICONTROL Enterprise-id]of [!UICONTROL federatieve id]hebt, klikt u op **[!UICONTROL Aanmelden]**.
De pagina [!UICONTROL Aanmelden] wordt geopend.
   1. Geef uw [!UICONTROL Adobe-id] gegevens op en klik op **[!UICONTROL Aanmelden]**.<br />
   ![Adobe-aanmelding](assets/bplogin_request_access_3.png)

   U wordt omgeleid naar de pagina [!UICONTROL Verzoek om toegang] .<br />
   **Scenario 2**
   1. Als u geen [!UICONTROL Adobe-id]hebt, klikt u op **[!UICONTROL Een Adobe-id]** ophalen op de pagina [!UICONTROL Toegang] aanvragen om een Adobe-id te maken.
De pagina [!UICONTROL Aanmelden] wordt geopend.
   1. Klik op Een Adobe-id **[!UICONTROL ophalen]**.
De pagina [!UICONTROL Aanmelden] wordt geopend.
   1. Voer uw voornaam en achternaam, e-mailadres en wachtwoord in.
   1. Selecteer **[!UICONTROL Aanmelden]**.<br />
   ![](assets/bplogin_request_access_5.png)

   U wordt omgeleid naar de pagina [!UICONTROL Verzoek om toegang] .

1. Op de volgende pagina worden uw naam en e-mailadres weergegeven waarmee u toegang kunt aanvragen. Laat een opmerking staan voor de beheerder en klik op **[!UICONTROL Verzenden]**.<br />

   ![](assets/bplogin-request-access.png)

## Productbeheerders verlenen toegang {#grant-access-to-brand-portal}

Merk Portal-productbeheerders ontvangen toegangsverzoeken in hun Merkortaal-systeemvak en via e-mails in hun postvak.

![Toegang aangevraagd bericht](assets/bplogin_request_access_7.png)

Om toegang te verlenen, moeten de productbeheerders de relevante melding in het Poortmeldingsgebied van het Merk klikken en dan Toegang ****verlenen klikken.
Productbeheerders kunnen ook de koppeling in de e-mail met het toegangsverzoek volgen om naar Adobe [!UICONTROL Admin Console] te gaan en de gebruiker aan de relevante productconfiguratie toe te voegen.

U wordt omgeleid naar de startpagina van de [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) . Met Adobe [!UICONTROL Admin Console] kunt u gebruikers maken en deze toewijzen aan productprofielen (voorheen bekend als productconfiguraties) die als groepen in Brand Portal worden weergegeven. Voor meer informatie over het toevoegen van gebruikers in [!UICONTROL Console]Admin, zie een gebruiker [](brand-portal-adding-users.md#add-a-user) toevoegen (stap 4-7 in de procedure volgen om een gebruiker toe te voegen).

## Merkporttalen {#brand-portal-language}

U kunt de Brand Portal-taal wijzigen vanuit Adobe [!UICONTROL Experience Cloud Settings].

![Toegang aangevraagd bericht](assets/BPLang.png)

De taal wijzigen:

1. Selecteer [!UICONTROL Gebruiker] > Profiel  bewerken in het bovenste menu.<br />
   ![Profiel bewerken](assets/EditBPProfile.png)

1. Selecteer op de pagina Instellingen [!UICONTROL van] Experience Cloud een taal in het keuzemenu [!UICONTROL Taal] .

## Meldingen over onderhoud aan Brand Portal {#brand-portal-maintenance-notification}

Voordat het Brand Portal is gepland voor onderhoud, wordt een melding weergegeven als een banner nadat u zich hebt aangemeld bij Brand Portal. Een voorbeeldmelding:

![](assets/bp_maintenance_notification.png)

U kunt dit bericht negeren en doorgaan met het gebruik van Brand Portal. Deze melding wordt in elke nieuwe sessie weergegeven.

## Vrijgave en systeeminformatie {#release-and-system-information}

* [Nieuwe functies](whats-new.md)
* [Release-opmerkingen](brand-portal-release-notes.md)
* [Ondersteunde bestandsindelingen](brand-portal-supported-formats.md)

## Gerelateerde bronnen {#related-resources}

* [Adobe Klantenservice](https://helpx.adobe.com/marketing-cloud/contact-support.html)
* [AEM-forums](https://www.adobe.com/go/aod_forums_en)