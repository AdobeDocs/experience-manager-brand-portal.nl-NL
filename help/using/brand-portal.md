---
title: Overzicht van Experience Manager Assets Brand Portal
seo-title: Overview of Experience Manager Assets Brand Portal
description: Met Experience Manager Assets Brand Portal kunt u eenvoudig goedgekeurde creatieve middelen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten.
seo-description: Experience Manager Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: d84d138a2819ff293d0c808b0dcebe02e03da121
workflow-type: tm+mt
source-wordcount: '1511'
ht-degree: 0%

---

# Overzicht van Experience Manager Assets Brand Portal {#overview-of-aem-assets-brand-portal}

Als markator, moet u soms met kanaalpartners en interne bedrijfsgebruikers samenwerken om, relevante digitale inhoud snel tot stand te brengen te beheren en te leveren aan klanten. De tijdige levering van relevante inhoud over de volledige klantenreis is kritiek aan het drijven van grotere vraag, omzetting, overeenkomst, en klantenloyaliteit.

Het is echter een uitdaging om oplossingen te ontwikkelen die efficiënte en veilige delen van goedgekeurde merklogo&#39;s, richtlijnen, campagnemiddelen of productschoten met uitgebreide interne teams, partners en wederverkopers ondersteunen.

**Adobe Experience Manager (AEM) Assets Brand Portal** concentreert zich op de behoefte van de prijsmeter om effectief met de globaal verdeelde gebruikers van Brand Portal samen te werken door activadistributie en activa bijdragemogelijkheden te verstrekken.

Met Asset Distribution kunt u eenvoudig goedgekeurde creatieve elementen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten. Terwijl de inbreng van activa de gebruikers van Brand Portal de capaciteit om activa aan Brand Portal te uploaden en aan Experience Manager Assets te publiceren toelaat, zonder toegang tot het auteursmilieu te vereisen. De bijdrageeigenschap wordt geroepen als **Middelen van Assets in Brand Portal**. En samen verbetert het de algemene ervaring van Brand Portal op het gebied van de distributie van activa en de bijdrage van de Brand Portal-gebruikers (externe agentschappen/teams), versnelt het de tijd-aan-markt voor activa, en vermindert het risico van niet-naleving en onbevoegde toegang.
Zie, [ Middelen van Activa in Brand Portal ](brand-portal-asset-sourcing.md).

Met de browsergebaseerde portalomgeving kunt u elementen gemakkelijk uploaden, doorbladeren, zoeken, voorvertonen en exporteren in een goedgekeurde indeling.

## Experience Manager Assets configureren met Brand Portal {#configure-brand-portal}

Als u Adobe Experience Manager Assets configureert met Brand Portal, kunt u functies voor het publiceren van bedrijfsmiddelen, het distribueren van bedrijfsmiddelen en het leveren van bedrijfsmiddelen inschakelen voor de Brand Portal-gebruikers.

>[!NOTE]
>
>Het configureren van Experience Manager Assets met Brand Portal wordt ondersteund op Experience Manager Assets as a Cloud Service, Experience Manager Assets 6.3 en hoger.

Experience Manager Assets as a Cloud Service wordt automatisch geconfigureerd met Brand Portal door Brand Portal vanuit de Cloud Manager te activeren. De activeringsworkflow maakt de vereiste configuraties op de achtergrond en activeert Brand Portal op dezelfde IMS org als de Experience Manager Assets as a Cloud Service instantie.

Terwijl Experience Manager Assets (op gebouw en beheerde dienst) manueel met Brand Portal wordt gevormd gebruikend Adobe Developer Console, die een teken van de Diensten van de Adobe Identity Management (IMS) voor vergunning van de huurder van Brand Portal aanschaft.

Voor meer informatie, zie [ het vormen Experience Manager Assets met Brand Portal ](../using/configure-aem-assets-with-brand-portal.md).

## Personen van gebruikers in Brand Portal {#Personas}

Brand Portal ondersteunt de volgende gebruikersrollen:

* Gastgebruiker
* Viewer
* Editor
* Beheerder

De volgende lijst maakt een lijst van de taken die de gebruikers in deze rollen kunnen uitvoeren:

|  | **doorbladeren** | **Zoeken** | **Download** | **de omslagen van het Aandeel** | **deel een inzameling** | **de activa van het Aandeel als verbinding** | **Toegang tot Hulpmiddelen Admin** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Gast gebruiker** | ✓* | ✓* | ✓* | x | x | x | x |
| **Kijker** | ✓ | ✓ | ✓ | x | x | x | x |
| **Redacteur** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Beheerder** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

>[!NOTE]
>
>Gastgebruikers kunnen alleen in openbare mappen en verzamelingen door elementen bladeren, deze openen en zoeken.

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### Gastgebruiker {#guest-user}

Experience Manager Assets Brand Portal staat [ gasttoegang ](#request-access-to-brand-portal) aan Brand Portal toe. Een gastgebruiker heeft geen geloofsbrieven nodig om het portaal in te gaan en heeft toegang tot de openbare omslagen en de inzamelingen. Als gastgebruiker, kunt u door activa details doorbladeren en volledige activamening van leden van openbare omslagen en inzamelingen hebben. U kunt openbare middelen zoeken, downloaden en toevoegen aan [!UICONTROL Lightbox] -verzameling.

De gastsessie beperkt u echter het maken van verzamelingen en opgeslagen zoekopdrachten en deelt deze verder. Gebruikers in een gastsessie hebben geen toegang tot de instellingen voor mappen en verzamelingen en kunnen hun middelen niet als koppeling delen. Hier is een lijst van taken die een gastgebruiker kan uitvoeren:

* [Bladeren en openbare middelen openen](browse-assets-brand-portal.md)

* [Openbare middelen zoeken](brand-portal-searching.md)

* [Overheidsmiddelen downloaden](brand-portal-download-assets.md)

* [Elementen toevoegen aan [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

Voor meer informatie, zie [ gasttoegang tot Brand Portal ](../using/guest-access.md).

### Viewer {#viewer}

Brand Portal-gebruiker gedefinieerd in [!DNL Admin Console] die toegang heeft tot Brand Portal met de rol Viewer. Een gebruiker met deze rol kan zich aanmelden bij Brand Portal en toegang krijgen tot toegestane mappen, verzamelingen en elementen. De gebruiker kan ook naar elementen (oorspronkelijke of specifieke vertoningen) bladeren, deze voorvertonen, downloaden en exporteren, accountinstellingen configureren en naar elementen zoeken. Hier volgt een lijst met taken die een viewer kan uitvoeren:

* [Bladeren door elementen](browse-assets-brand-portal.md)

* [Middelen zoeken](brand-portal-searching.md)

* [Elementen downloaden](brand-portal-download-assets.md)

### Editor {#editor}

Een gebruiker met de rol van Editor kan alle taken uitvoeren die een Viewer kan uitvoeren. Bovendien kunnen de Editor en de Editor de bestanden en mappen weergeven die een beheerder deelt. De gebruiker met de rol van een Editor kan ook inhoud (bestanden, mappen, verzamelingen) met anderen delen.

Naast de taken die een Viewer kan uitvoeren, kan een Editor de volgende extra taken uitvoeren:

* [Mappen delen](brand-portal-sharing-folders.md)

* [Een verzameling delen](brand-portal-share-collection.md)

* [Elementen delen als koppeling](brand-portal-link-share.md)

### Beheerder {#administrator}

Een beheerder bevat een gebruiker die is gemarkeerd als systeembeheerder of Brand Portal-productbeheerder in [!UICONTROL Admin Console] . Een beheerder kan systeembeheerders en gebruikers toevoegen en verwijderen, voorinstellingen definiëren, e-mail verzenden naar gebruikers en portaalgebruik en opslagrapporten weergeven.

>[!NOTE]
>
>In Brand Portal heeft een gebruiker die is gemarkeerd met de rol van supportbeheerder in [!UICONTROL Admin Console] dezelfde rechten als een systeembeheerder.

Een beheerder kan alle taken uitvoeren die een Redacteur kan uitvoeren. Hier volgen de extra taken die een beheerder kan uitvoeren:

* [Gebruikers, groepen en gebruikersrollen beheren](brand-portal-adding-users.md)

* [Achtergrond, paginakoppen en e-mails aanpassen](brand-portal-branding.md)

* [Aangepaste zoekfacetten gebruiken](brand-portal-search-facets.md)

* [Het metagegevensschema gebruiken](brand-portal-metadata-schemas.md)

* [Voorinstellingen voor afbeeldingen of dynamische uitvoeringen toepassen](brand-portal-image-presets.md)

* [Werken met rapporten](brand-portal-reports.md)

Naast de bovenstaande taken kan een auteur in AEM Assets de volgende taken uitvoeren:

* [AEM Assets configureren met Brand Portal](../using/configure-aem-assets-with-brand-portal.md)

* [Mappen publiceren naar Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-folder.html)

* [Verzamelingen publiceren naar Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-collection.html)

## Alternatieve alias voor Brand Portal URL {#tenant-alias-for-portal-url}

Vanaf Brand Portal 6.4.3 kunnen organisaties één alternatieve (alias) URL voor bestaande URL van hun Brand Portal-huurder hebben. De alias-URL kan worden gemaakt door een alternatief voorvoegsel in de URL te plaatsen.\
Als de huurdersnaam meer dan 32 karakters is, dan moet de huurdersalias worden gecreeerd.
Merk op dat alleen het voorvoegsel van de Brand Portal URL kan worden aangepast en niet de volledige URL. Zo kan een organisatie met een bestaand domein `geomettrix.brand-portal.adobe.com` op verzoek `geomettrixinc.brand-portal.adobe.com` maken.

Nochtans, AEM de instantie van de Auteur kan [ worden gevormd ](../using/configure-aem-assets-with-brand-portal.md) slechts met huurder identiteitskaart URL en niet met huurder alias (afwisselend) URL.

>[!NOTE]
>
>Om een alias voor huurdersnaam in bestaande portaal URL te krijgen, moeten de organisaties de steun van de Klant met een nieuw verzoek van de huurdersalias contacteren. Dit verzoek wordt verwerkt door eerst te controleren of de alias beschikbaar is en vervolgens de alias te maken.
>
>Als u de oude alias wilt vervangen of de oude alias wilt verwijderen, moet hetzelfde proces worden gevolgd.

## Toegang tot Brand Portal aanvragen {#request-access-to-brand-portal}

Gebruikers kunnen toegang tot Brand Portal aanvragen via het aanmeldingsscherm. Deze aanvragen worden verzonden naar Brand Portal-beheerders, die via de Adobe toegang verlenen aan gebruikers [!UICONTROL Admin Console] . Nadat toegang is verleend, ontvangen gebruikers een e-mailbericht.

Ga als volgt te werk om toegang aan te vragen:

1. Selecteer op de Brand Portal-aanmeldingspagina de optie **[!UICONTROL Click here]** voor **[!UICONTROL Need Access?]** . Als u echter de gastsessie wilt betreden, selecteert u de **[!UICONTROL Click here]** betreffende sessie van **[!UICONTROL Guest Access?]** .

   ![ Brand Portal login scherm ](assets/bp-login-requestaccess.png)

   De pagina [!UICONTROL Request Access] wordt geopend.

1. Als u toegang wilt aanvragen tot de Brand Portal van een organisatie, moet u over een geldige [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID] of [!UICONTROL Federated ID] beschikken.

   Meld u op de pagina [!UICONTROL Request Access] aan met uw id (scenario 1) of maak een [!UICONTROL Adobe ID] (scenario 2):

   ![[!UICONTROL Request access]](assets/bplogin_request_access_2.png)

   **Scenario 1**

   1. Als u een [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID], of [!UICONTROL Federated ID] hebt, klikt u op **[!UICONTROL Sign In]** .
De pagina [!UICONTROL Sign in] wordt geopend.

   1. Geef uw [!UICONTROL Adobe ID] -gegevens op en klik op **[!UICONTROL Sign in]** .

      ![ teken van de Adobe binnen ](assets/bplogin_request_access_3.png)

   U wordt omgeleid naar de pagina [!UICONTROL Request Access] .

   **Scenario 2**

   1. Als u geen [!UICONTROL Adobe ID] hebt, klikt u op **[!UICONTROL Get an Adobe ID]** van de pagina [!UICONTROL Request Access] om er een te maken.
De pagina [!UICONTROL Sign in] wordt geopend.
   1. Klik op **[!UICONTROL Get an Adobe ID]** .
De pagina [!UICONTROL Sign up] wordt geopend.
   1. Voer uw voornaam en achternaam, e-mailadres en wachtwoord in.
   1. Selecteer **[!UICONTROL Sign up]** .

      ![](assets/bplogin_request_access_5.png)

   U wordt omgeleid naar de pagina [!UICONTROL Request Access] .

1. Op de volgende pagina worden uw naam en e-mailadres weergegeven waarmee u toegang kunt aanvragen. Laat een opmerking staan voor de beheerder en klik op **[!UICONTROL Submit]** .

   ![](assets/bplogin-request-access.png)

## Productbeheerders verlenen toegang {#grant-access-to-brand-portal}

Brand Portal-productbeheerders ontvangen toegangsaanvragen in hun Brand Portal-systeemvak en via e-mails in hun Postvak IN.

![ Toegang verzocht bericht ](assets/bplogin_request_access_7.png)

Als u toegang wilt verlenen, moeten productbeheerders op de desbetreffende melding in het Brand Portal-systeemvak klikken en vervolgens op **[!UICONTROL Grant Access]** klikken.
Productbeheerders kunnen ook de koppeling in de e-mail met het toegangsverzoek volgen om de Adobe [!UICONTROL Admin Console] te bezoeken en de gebruiker aan de relevante productconfiguratie toe te voegen.

U wordt opnieuw gericht aan de [ Adobe [!UICONTROL Admin Console] ](https://adminconsole.adobe.com/enterprise/overview) homepage. Gebruik Adobe [!UICONTROL Admin Console] om gebruikers te maken en deze toe te wijzen aan productprofielen (voorheen productconfiguraties genoemd) die in Brand Portal als groepen worden weergegeven. Voor meer informatie over het toevoegen van gebruikers in [!UICONTROL Admin Console], zie [ een gebruiker ](brand-portal-adding-users.md#add-a-user) toevoegen (stap 4-7 in de procedure volgen om een gebruiker toe te voegen).

## Brand Portal talen {#brand-portal-language}

U kunt de Brand Portal-taal wijzigen vanuit de Adobe [!UICONTROL Experience Cloud Settings] .

![ Toegang verzocht bericht ](assets/BPLang.png)

De taal wijzigen:

1. Selecteer [!UICONTROL User] > [!UICONTROL Edit Profile] in het bovenste menu.

   ![ geef Profiel ](assets/EditBPProfile.png) uit

1. Selecteer op de pagina [!UICONTROL Experience Cloud Settings] een taal in de vervolgkeuzelijst [!UICONTROL Language] .

## Brand Portal-onderhoudsmelding {#brand-portal-maintenance-notification}

Voordat Brand Portal wordt aangemeld voor onderhoud, wordt een bericht weergegeven als een banner nadat u zich hebt aangemeld bij Brand Portal. Een voorbeeldmelding:

![](assets/bp_maintenance_notification.png)

Je kunt dit bericht negeren en doorgaan met Brand Portal. Deze melding wordt in elke nieuwe sessie weergegeven.

## Vrijgave en systeeminformatie {#release-and-system-information}

* [Nieuwe functies](whats-new.md)
* [Release-opmerkingen](brand-portal-release-notes.md)
* [Ondersteunde bestandsindelingen](brand-portal-supported-formats.md)

## Gerelateerde bronnen {#related-resources}

<!--
* [Adobe Customer Support]()
-->

* [ AEM Forums ](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
