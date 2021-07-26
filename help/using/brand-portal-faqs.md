---
title: Veelgestelde vragen
seo-title: null
description: Bekijk de veelgestelde vragen in de Adobe Experience Manager Assets Brand Portal.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 22104bff436b432e2198bd770f1f39d5c4350518
workflow-type: tm+mt
source-wordcount: '1469'
ht-degree: 0%

---

# Veelgestelde vragen {#frequently-asked-questions}

De veelgestelde vragen over Brand Portal zijn toegespitst op de vragen en problemen die eindgebruikers kunnen tegenkomen tijdens het werken met de nieuwste AEM Assets Brand Portal 6.4.6-release of eerdere versies.


## Brand Portal 6.4.6 Veelgestelde vragen  {#faqs-bp646}

**Ques. Het bestaande oudere eindpunt OAuth (`https://legacy-oauth.cloud.adobe.io/login`) werkt niet. Wat zou de mogelijke reden kunnen zijn?**

**Ans.** Verouderde OAuth-configuratie is vervangen. U moet AEM Assets auteur instanties aan het recentste de dienstpak bevorderen en het vormen via de Console van de Ontwikkelaar van de Adobe. Zie [AEM Assets configureren met Brand Portal](configure-aem-assets-with-brand-portal.md) voor meer informatie. Nochtans, voor Verouderde configuratie OAuth om tot u bevordert te werken, werk het Oudere eindpunt OAuth aan `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/` bij.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Ques. Ik kan de middelen van de bijdragemap niet publiceren van Brand Portal naar AEM Assets na de upgrade naar Adobe Developer Console. Mijn auteur bevindt zich op AEM 6.5.4. Wat zou de mogelijke reden kunnen zijn?**

**Ans.** Ja, er is een bekend probleem bij het publiceren van de middelen van de bijdragemap naar AEM Assets op AEM 6.5.4 via Adobe Developer Console.

De kwestie is vastgelegd in AEM 6.5.5. U kunt uw AEM Assets-instantie upgraden naar het nieuwste servicepack AEM 6.5.5 en [uw configuraties upgraden](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) op de Adobe Developer Console.

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**Ques. Ik zie de inhoud van de bijdragemap niet gepubliceerd vanuit Brand Portal in AEM Assets. Wat zou de mogelijke reden kunnen zijn?**

**Ans.** Neem contact op met de AEM Assets-beheerder om de configuraties te controleren en ervoor te zorgen dat uw Brand Portal-huurder slechts met één AEM Assets-auteurinstantie is geconfigureerd.

Dit probleem doet zich mogelijk voor wanneer u een Brand Portal-medewerker hebt geconfigureerd voor meerdere AEM Assets-auteur-instanties. Bijvoorbeeld, vormt de beheerder de zelfde huurder van Brand Portal op de de auteurinstantie van AEM Assets van het opvoeren en productiemilieu. In dit geval wordt de functie voor het publiceren van middelen geactiveerd in Brand Portal, maar de AEM Assets-instantie die de maker van de middelen heeft, kan de elementcode niet importeren die de replicator niet ontvangt voor de token die de aanvraag indient.


**Ques. Ik kan geen middelen van AEM Assets naar Brand Portal publiceren. Het replicatielogboek verklaart dat de verbinding uit timed. Is er een snelle oplossing?**

**Ans.** Het publiceren ontbreekt gewoonlijk met een onderbrekingsfout als er veelvoudige hangende verzoeken in de replicatierij zijn. Om deze kwestie op te lossen, zorg ervoor dat de replicatieagenten worden gevormd om onderbreking te vermijden.

Voer de volgende stappen uit om de replicatieagent te vormen:
1. Meld u aan bij de AEM Assets-auteur.
1. Navigeer in het deelvenster **Gereedschappen** naar **[!UICONTROL Deployment]** > **[!UICONTROL Replication]**.
1. Klik op **[!UICONTROL Agents on author]** op de pagina Replicatie. U kunt de vier replicatieagenten voor uw huurder van Brand Portal zien.
1. Klik de replicatieagent URL om de agentendetails te openen.
1. Klik **[!UICONTROL Edit]** om de montages van de replicatieagent te wijzigen.
1. Klik in Agent-instellingen op het tabblad **[!UICONTROL Extended]**.
1. Schakel het selectievakje **[!UICONTROL Close Connection]** in.
1. Herhaal stap 4 door 7 om alle vier replicatieagenten te vormen.
1. Start de server opnieuw en controleer de verbinding.


## Brand Portal 6.4.5 - Veelgestelde vragen  {#faqs-bp645}

**Ques. Wat is de belangrijkste wijziging in de release van Brand Portal 6.4.5?**

**Ans.** AEM Assets Brand Portal 6.4.5 is een release met functies waarmee de Brand Portal-gebruikers inhoud kunnen uploaden van het Brand Portal-exemplaar naar AEM Assets en de map Contribution opnieuw kunnen publiceren zonder beheerdersrechten.
Zie [Asset Sourcing in Brand Portal](brand-portal-asset-sourcing.md) voor meer informatie.



**Ques. Zal ik toegang tot om het even welke bestaande activa, eigenschappen, of configuraties verliezen ik heb gecreeerd?**

**Ans.** Alle bestaande functies en configuraties blijven intact. Uw eindgebruikers worden niet beïnvloed en uw inhoud blijft intact.



**Ques. Wanneer ga ik naar de nieuwe versie van Brand Portal?**

**Ans.** Brand Portal 6.4.5 werd in oktober 2019 aan de productie vrijgegeven. En de volgende Brand Portal-versie zal naar verwachting in het derde kwartaal van 2020 worden uitgebracht.
Voor updates en versiewijziging wordt aanbevolen de [Release-aantekeningen](brand-portal-release-notes.md) en [Nieuwe functies in Brand Portal](whats-new.md) bij te houden.



**Ques. Zullen mijn gebruikers worden beïnvloed?**

**Ans.** De Brand Portal 6.4.5-release bevindt zich uitsluitend in Brand Portal, dus dit heeft geen gevolgen voor uw eindgebruikers.



**Ques. Is er een actie vereist van mijn kant als gebruiker van Brand Portal?**

**Ans.** De Brand Portal 6.4.5-release wordt geleverd met een nieuwe functie genaamd Asset Sourcing. AEM beheerder moet de functie Asset Sourcing in AEM Assets configureren om deze functie in te schakelen voor de Brand Portal-gebruikers. Raadpleeg [Asset Sourcing inschakelen](brand-portal-asset-sourcing.md) voor meer informatie.



**Ques. Wie kan een map met bijdragen maken?**

**Ans.** Elke AEM gebruiker met bevoegdheden om een nieuwe map in AEM Assets te maken, kan een  **** Contribute-map maken. Als u een **Contribute**-map wilt maken, maakt u een nieuwe map van het type **Asset Contribution**.
Deze map wordt gedeeld met de actieve Brand Portal-gebruikers voor een bijdrage.



**Ques. Wat bevat een map met bijdragen?**

**Ans.** **De** Contribute-map bevat twee submappen  **** NEWand  **SHARED**. In eerste instantie is de map NEW leeg en bevat de map SHARED de referentie-inhoud (herbruikbare elementen) voor de Brand Portal-gebruikers.
De Brand Portal-gebruikers openen de map **Contribution** en uploaden inhoud naar de map **NEW**.



**Ques.  Kan ik de naam van een bestaande map voor bijdragen wijzigen?**

**Ans.** **Nee**, u kunt de naam van een bestaande  **** Contribute-map niet wijzigen.



**Ques. Wat zijn de activavereisten met r.t bijdrage?**

**Ans.** Het  **** Briefdocument dat aan de omslag van de  **** Bijdrage en de verwijzingsinhoud (herbruikbare activa) wordt geupload in  **** SHAREDfolder helpt de gebruiker van Brand Portal de behoefte van bijdrage en verwachtingen als contribuant begrijpen, en collectief genoemd als activavereisten.



**Ques. Kan ik middelen uploaden naar om het even welke toegelaten omslag?**

**Ans.** Niet alle toegestane mappen. Een Brand Portal-gebruiker kan inhoud alleen uploaden naar de map **Contribution** die wordt gedeeld door de AEM of Brand Portal-beheerder.



**Ques. Hoe krijg ik toegang tot een omslag van de Bijdrage?**

**Ans.** U hebt alleen toegang tot een  **** Contribute-map als deze met u is gedeeld. U krijgt een e-mail-/pulsmelding wanneer een map met bijdragen met u wordt gedeeld. U kunt de map Contribution openen via de koppeling die in de e-mail wordt gedeeld, of u kunt zich aanmelden bij uw Brand Portal-exemplaar en naar het belpictogram gaan voor kennisgeving om de map Contribution te openen.

>[!NOTE]
>
>Als u geen bestaande Brand Portal-gebruiker bent, vraagt u de AEM beheerder om uw gebruiker te maken in de AEM-beheerconsole en uw profiel toe te voegen aan het gebruikersconfiguratiebestand in de lijst met Brand Portal-gebruikers.

**Ques. Wat is het Formaat van het Csv- dossier voor gebruikersinvoer?**

**Ans.** De indeling is dezelfde als de indeling die door de Admin Console wordt ondersteund bij het importeren van bulkgebruikers. E-mail, voornaam en achternaam zijn verplicht.



**Ques. Wat vult de lijst met gebruikers (Brand Portal contributors) in de vervolgkeuzelijst voor gebruikers van Asset Contribution?**

**Ans.** De gebruikers in de vervolgkeuzelijst worden gevuld vanuit het Brand Portal-bestand voor gebruikersconfiguratie (.csv) dat in AEM is geüpload.



**Ques. Waar kan ik de status van import- en publicatietaken zien?**

**Ans.** In AEM kunt u de status van een importbewerking op de  **** asynchrone pagina zien. In Brand Portal kunt u de status van een publicatietaak zien in **[!UICONTROL Tools > Asset Contribution status]**.



**Ques. Wat is de frequentie van een importtaak die periodiek in AEM loopt?**

**Ans.** In AEM worden om de vijf minuten opiniepeilingen gehouden.



**Ques. Is er een drempelwaarde voor het aantal keren dat een map kan worden gepubliceerd van Brand Portal naar AEM Assets?**

**Ans.** Nee, alle elementen in de  **** map NEWfolder worden gepubliceerd naar AEM Assets, ongeacht het feit dat ze eerder zijn gepubliceerd. Elke keer dat een **Contribute**-map wordt gepubliceerd van Brand Portal naar AEM Assets, wordt de inhoud van de map **NEW** genegeerd.



**Ques. Hoe te om nieuwe activa in een omslag van de Bijdrage te uploaden?**

**Ans.** Raadpleeg de gedetailleerde documentatie voor het  [uploaden van middelen naar de map](brand-portal-publish-contribution-folder-to-brand-portal.md) Contribution.



**Ques. Ik zie geen miniaturen/voorvertoningen van de middelen die door een Brand Portal-gebruiker naar de map NEW zijn geüpload?**

**Ans.** Het is zo ontworpen, want er wordt geen workflow uitgevoerd aan het einde van Brand Portal.



**Ques. Wat gebeurt er als een map van AEM Assets naar Brand Portal wordt gepubliceerd die in flux is?**

**Ans.** In AEM worden logbestanden voor elke keer dat een map naar Brand Portal wordt gepubliceerd, bijgehouden. Op het moment van publicatie worden alle elementen die niet naar Brand Portal zijn gepubliceerd, in een replicatiewachtrij geplaatst. Middelen die aan de map worden toegevoegd nadat de publicatietaak is geactiveerd, worden niet gepubliceerd naar Brand Portal. Wanneer de AEM gebruiker de map opnieuw publiceert, worden alleen de elementen die niet eerder zijn gepubliceerd (in de replicatiewachtrij), gepubliceerd naar Brand Portal.
Dit geldt voor alle mappen die van AEM Assets naar Brand Portal worden gepubliceerd en voor de map SHARED in de map Contribution.

**Ques. Wie neem ik contact op met vragen?**

**Ans.** Neem contact op met uw Adobe-accountmanager of klantenondersteuning.

>[!NOTE]
>
>De releaseplanning is tijdelijk en kan worden gewijzigd. Neem contact op met uw Adobe-accountmanager of klantenondersteuning voor het bijgewerkte releaseprogramma.


## Toegang tot en ondersteuning voor producten (beperkt aantal sites) {#product-access-and-support-restricted-sites}

Deze sites zijn alleen beschikbaar voor klanten. Neem contact op met uw Adobe-accountmanager als u een klant bent en toegang nodig hebt.

* [](https://daycare.day.com) [Producttoegang](https://login.marketing.adobe.com)

* [Adobe Klantenservice](https://helpx.adobe.com/contact.html)
