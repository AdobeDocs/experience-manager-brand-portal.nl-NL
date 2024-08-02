---
title: Overzicht van Experience Manager Assets Brand Portal
description: Leer hoe u met Experience Manager Assets Brand Portal eenvoudig goedgekeurde creatieve middelen kunt aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten.
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: 32a67abf466dd3bf635b851b02377ed23591915e
workflow-type: tm+mt
source-wordcount: '1539'
ht-degree: 0%

---

# Overzicht van Experience Manager Assets Brand Portal {#overview-of-aem-assets-brand-portal}

Als markator, moet u soms met kanaalpartners en interne bedrijfsgebruikers samenwerken om, relevante digitale inhoud tot stand te brengen te beheren en snel te leveren aan klanten. De tijdige levering van relevante inhoud over de volledige klantenreis is kritiek aan het drijven van grotere vraag, omzetting, overeenkomst, en klantenloyaliteit.

Maar het ontwikkelen van oplossingen die efficiënte en veilige delen van zaken zoals goedgekeurde merklogo&#39;s, campagneactiva, of productschoten met teams, partners, en resellers steunen is een uitdaging. Het waarborgen van zowel efficiëntie als veiligheid in dit proces vereist zorgvuldige planning en uitvoering.

**Adobe Experience Manager (AEM) Assets Brand Portal** concentreert zich op de behoefte van de prijsmeter om effectief met de globaal verdeelde gebruikers van Brand Portal samen te werken door activadistributie en activa bijdragemogelijkheden te verstrekken.

Met Asset Distribution kunt u goedgekeurde creatieve elementen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten. Dankzij de bijdrage aan bedrijfsmiddelen kunnen Brand Portal-gebruikers echter elementen uploaden naar Brand Portal en publiceren naar Experience Manager Assets, zonder dat ze toegang hoeven te hebben tot de auteursomgeving. De bijdrageeigenschap wordt geroepen als **Middelen van Assets in Brand Portal**. En samen verbetert het de algemene ervaring van Brand Portal op het gebied van de distributie van activa en de bijdrage van de Brand Portal-gebruikers (externe agentschappen/teams), versnelt het de tijd-aan-markt voor activa, en vermindert het risico van niet-naleving en onbevoegde toegang.
Zie, [ Middelen van Activa in Brand Portal ](brand-portal-asset-sourcing.md).

Met de browsergebaseerde portalomgeving kunt u elementen eenvoudig uploaden, doorbladeren, zoeken, voorvertonen en exporteren in goedgekeurde indelingen.

## Experience Manager Assets configureren met Brand Portal {#configure-brand-portal}

Als u Adobe Experience Manager Assets configureert met Brand Portal, kunt u functies voor het publiceren van bedrijfsmiddelen, het distribueren van bedrijfsmiddelen en het leveren van bedrijfsmiddelen inschakelen voor de Brand Portal-gebruikers.

>[!NOTE]
>
>Het configureren van Experience Manager Assets met Brand Portal wordt ondersteund op Experience Manager Assets as a Cloud Service, Experience Manager Assets 6.3 en hoger.

Experience Manager Assets as a Cloud Service wordt automatisch geconfigureerd met Brand Portal door Brand Portal vanuit de Cloud Manager te activeren. De activeringsworkflow maakt de vereiste configuraties op de achtergrond en activeert Brand Portal op dezelfde IMS org als de Experience Manager Assets as a Cloud Service instantie.

Nochtans, wordt Experience Manager Assets (op gebouw en beheerde dienst) manueel gevormd met Brand Portal gebruikend Adobe Developer Console, die een teken van Identity Management van de Adobe van de Diensten (IMS) voor vergunning van de huurder van Brand Portal aanschaft.

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

Experience Manager Assets Brand Portal staat [ gasttoegang ](#request-access-to-brand-portal) aan Brand Portal toe. Een gastgebruiker heeft geen geloofsbrieven nodig om het portaal in te gaan en heeft toegang tot de openbare omslagen en de inzamelingen. Als gastgebruiker, kunt u door activa details doorbladeren en een volledige activamening van leden van openbare omslagen en inzamelingen hebben. U kunt openbare middelen zoeken, downloaden en toevoegen aan de [!UICONTROL Lightbox] -verzameling.

Nochtans, beperkt de gastzitting u van het creëren van inzamelingen en bewaarde onderzoeken, en deelt hen verder. Gebruikers in een gastsessie hebben geen toegang tot de instellingen voor mappen en verzamelingen en kunnen hun middelen niet als koppeling delen. Hier is een lijst van taken die een gastgebruiker kan uitvoeren:

* [Bladeren en openbare middelen openen](browse-assets-brand-portal.md)

* [Openbare middelen zoeken](brand-portal-searching.md)

* [Overheidsmiddelen downloaden](brand-portal-download-assets.md)

* [Elementen toevoegen aan [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

Voor meer informatie, ga naar [ Gast Toegang tot Brand Portal ](../using/guest-access.md).

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

Een beheerder bevat een gebruiker die is gemarkeerd als systeembeheerder of Brand Portal-productbeheerder in de [!UICONTROL Admin Console] . Een beheerder kan systeembeheerders en gebruikers toevoegen en verwijderen, voorinstellingen definiëren, e-mail verzenden naar gebruikers en portaalgebruik en opslagrapporten weergeven.

>[!NOTE]
>
>In Brand Portal heeft een gebruiker die is gemarkeerd met de rol van supportbeheerder in [!UICONTROL Admin Console] dezelfde rechten als een systeembeheerder.

Een beheerder kan alle taken uitvoeren die een Redacteur kan uitvoeren. Hieronder vindt u de extra taken die een beheerder kan uitvoeren:

* [Gebruikers, groepen en gebruikersrollen beheren](brand-portal-adding-users.md)
* [Achtergrond, paginakoppen en e-mails aanpassen](brand-portal-branding.md)
* [Aangepaste zoekfacetten gebruiken](brand-portal-search-facets.md)
* [Metagegevensschema gebruiken](brand-portal-metadata-schemas.md)
* [Voorinstellingen voor afbeeldingen of dynamische uitvoeringen toepassen](brand-portal-image-presets.md)
* [Werken met rapporten](brand-portal-reports.md)

Naast de bovenstaande taken kan een auteur in AEM Assets de volgende taken uitvoeren:

* [AEM Assets configureren met Brand Portal](../using/configure-aem-assets-with-brand-portal.md)
* [Mappen publiceren naar Brand Portal](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/brand-portal-publish-folder)
* [Verzamelingen publiceren naar Brand Portal](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/brand-portal-publish-collection)

## Alternatieve alias voor Brand Portal URL {#tenant-alias-for-portal-url}

Vanaf Brand Portal 6.4.3 kunnen organisaties één alternatieve (alias) URL hebben voor elke bestaande URL van hun Brand Portal-huurder. De alias-URL kan worden gemaakt door een alternatief voorvoegsel in de URL te plaatsen.\
Als de huurdersnaam meer dan 32 karakters is, dan moet een huurdersalias worden gecreeerd.
Merk op dat alleen het voorvoegsel van de Brand Portal URL kan worden aangepast en niet de volledige URL. Zo kan een organisatie met een bestaand domein `geomettrix.brand-portal.adobe.com` op verzoek `geomettrixinc.brand-portal.adobe.com` maken.

Nochtans, kan de AEM instantie van de Auteur [ worden gevormd ](../using/configure-aem-assets-with-brand-portal.md) slechts met huurder identiteitskaart URL en niet met huurder alias (afwisselend) URL.

>[!NOTE]
>
>Om een alias voor de huurdersnaam in een bestaande portaal URL te krijgen, moeten de organisaties de Steun van de Klant met een nieuw verzoek van de huurdersalias contacteren. Eerst, controleer als de alias beschikbaar is, dan creeer de alias om dit verzoek te verwerken.
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
De pagina [!UICONTROL Sign-in] wordt geopend.

   1. Geef uw [!UICONTROL Adobe ID] -gegevens op en klik op **[!UICONTROL Sign-in]** .

      ![ teken van de Adobe binnen ](assets/bplogin_request_access_3.png)

   U wordt omgeleid naar de pagina [!UICONTROL Request Access] .

   **Scenario 2**

   1. Als u geen [!UICONTROL Adobe ID] hebt, klikt u op **[!UICONTROL Get an Adobe ID]** van de pagina [!UICONTROL Request Access] om er een te maken.
De pagina [!UICONTROL Sign-in] wordt geopend.
   1. Klik op **[!UICONTROL Get an Adobe ID]** .
De pagina [!UICONTROL Sign-up] wordt geopend.
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
Productbeheerders kunnen ook de koppeling in de e-mail met het toegangsverzoek volgen om de Adobe [!UICONTROL Admin Console] te bezoeken en de gebruiker aan de desbetreffende productconfiguratie toe te voegen.

U wordt opnieuw gericht aan de [ Adobe [!UICONTROL Admin Console] ](https://adminconsole.adobe.com/enterprise/overview) homepage. Met de Adobe [!UICONTROL Admin Console] kunt u gebruikers maken en deze toewijzen aan productprofielen (voorheen productconfiguraties genoemd) die in Brand Portal als groepen worden weergegeven. Voor meer informatie over het toevoegen van gebruikers in [!UICONTROL Admin Console], zie [ een gebruiker ](brand-portal-adding-users.md#add-a-user) toevoegen (stap 4-7 in de procedure volgen om een gebruiker toe te voegen).

## Brand Portal talen {#brand-portal-language}

U kunt de Brand Portal-taal wijzigen vanuit Adobe [!UICONTROL Experience Cloud Settings] .

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
