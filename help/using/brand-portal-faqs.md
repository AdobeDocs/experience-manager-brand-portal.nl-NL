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
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1516'
ht-degree: 0%

---

# Veelgestelde vragen {#frequently-asked-questions}

De veelgestelde vragen over Brand Portal zijn toegespitst op de vragen en problemen die eindgebruikers kunnen tegenkomen tijdens het werken met de nieuwste Experience Manager Assets Brand Portal 6.4.6-release of eerdere versies.


## Brand Portal 6.4.6 Veelgestelde vragen  {#faqs-bp646}

**Ques. Het bestaande oudere eindpunt OAuth (`https://legacy-oauth.cloud.adobe.io/login`) werkt niet. Wat zou de mogelijke reden kunnen zijn?**

**Ans.** Verouderde OAuth-configuratie is vervangen. U moet Experience Manager Assets-auteur-instanties upgraden naar het nieuwste servicepakket en deze via Adobe Developer Console configureren. Zie [ Experience Manager Assets met Brand Portal ](configure-aem-assets-with-brand-portal.md) voor details vormen. Voor oudere OAuth-configuratie werkt u echter totdat u een upgrade uitvoert, het verouderde OAuth-eindpunt wordt bijgewerkt naar `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/` .

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Ques. Ik kan de middelen van de bijdragemap niet publiceren van Brand Portal naar Experience Manager Assets na de upgrade naar Adobe Developer Console. Mijn auteur-exemplaar staat op Experience Manager Assets 6.5.4. Wat zou de mogelijke reden kunnen zijn?**

**Ans.** Ja, er is een bekend probleem bij het publiceren van de middelen van de bijdragemap naar Experience Manager Assets 6.5.4 via Adobe Developer Console.

Het probleem is opgelost in Experience Manager Assets 6.5.5. U kunt uw instantie van Experience Manager Assets aan het recentste de dienstpak bevorderen en [ bevorderen uw configuraties ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) op Adobe Developer Console.

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**Ques. Ik zie de inhoud van de bijdragemap niet die vanuit Brand Portal in Experience Manager Assets is gepubliceerd. Wat zou de mogelijke reden kunnen zijn?**

**Ans.** Neem contact op met uw Experience Manager Assets-beheerder om de configuraties te controleren en te controleren of uw Brand Portal-huurder is geconfigureerd met slechts één Experience Manager Assets-auteurinstantie.

Dit probleem doet zich mogelijk voor wanneer u een Brand Portal-medewerker hebt geconfigureerd voor meerdere Experience Manager Assets-auteur-instanties. Bijvoorbeeld, vormt de beheerder de zelfde huurder van Brand Portal op de de auteurinstantie van Experience Manager Assets van het opvoeren en productiemilieu. In dit geval wordt de functie voor het publiceren van middelen geactiveerd in Brand Portal, maar de Experience Manager Assets-instantie die de maker van de middelen heeft, kan de elementcode niet importeren die de replicator niet ontvangt voor de token die de aanvraag indient.


**Ques. Ik kan geen middelen van Experience Manager Assets naar Brand Portal publiceren. Het replicatielogboek verklaart dat de verbinding uit timed. Is er een snelle oplossing?**

**Ans.** Doorgaans mislukt het publiceren door een time-outfout als er meerdere aanvragen in behandeling zijn in de replicatiewachtrij. Om deze kwestie op te lossen, zorg ervoor dat de replicatieagenten worden gevormd om onderbreking te vermijden.

Voer de volgende stappen uit om de replicatieagent te vormen:

1. Meld u aan bij de Experience Manager Assets-auteur.
1. Van het **paneel van Hulpmiddelen**, navigeer aan **[!UICONTROL Deployment]** > **[!UICONTROL Replication]**.
1. Klik op **[!UICONTROL Agents on author]** op de pagina Replicatie. U kunt de vier replicatieagenten voor uw huurder van Brand Portal zien.
1. Klik de replicatieagent URL om de agentendetails te openen.
1. Klik **[!UICONTROL Edit]** om de montages van de replicatieagent te wijzigen.
1. Klik in Agent-instellingen op de tab **[!UICONTROL Extended]** .
1. Schakel het selectievakje **[!UICONTROL Close Connection]** in.
1. Herhaal stap 4 door 7 om alle vier replicatieagenten te vormen.
1. Start de server opnieuw en controleer de verbinding.


## Brand Portal 6.4.5 - Veelgestelde vragen  {#faqs-bp645}

**Ques. Wat is de belangrijkste verandering in de versie van Brand Portal 6.4.5?**

**Ans.** Experience Manager Assets Brand Portal 6.4.5 is een functieversie waarmee Brand Portal-gebruikers inhoud kunnen uploaden van het Brand Portal-exemplaar naar Experience Manager Assets en de map Contribution opnieuw kunnen publiceren zonder dat ze beheerdersrechten nodig hebben.
Voor meer informatie, zie [ Middelen van Activa in Brand Portal ](brand-portal-asset-sourcing.md).



**Ques. Zal ik toegang tot om het even welke bestaande activa, eigenschappen, of configuraties verliezen ik heb gecreeerd?**

**Ans.** Alle bestaande functies en configuraties blijven intact. Uw eindgebruikers worden niet beïnvloed en uw inhoud blijft intact.



**Ques. Wanneer ga ik naar de nieuwe versie van Brand Portal?**

**Ans.** Brand Portal 6.4.5 is in oktober 2019 vrijgegeven voor productie. En de volgende Brand Portal-versie zal naar verwachting in het derde kwartaal van 2020 worden uitgebracht.
Voor updates en versieverandering, wordt het geadviseerd om de [ Nota&#39;s van de Versie ](brand-portal-release-notes.md) te volgen en [ wat in Brand Portal ](whats-new.md) nieuw is.



**Ques. Zullen mijn gebruikers worden beïnvloed?**

**Ans.** De Brand Portal 6.4.5-release bevindt zich uitsluitend in Brand Portal, dus dit heeft geen invloed op uw eindgebruikers.



**Ques. Is er om het even welke actie die op mijn deel als gebruiker van Brand Portal wordt vereist?**

**Ans.** De release van Brand Portal 6.4.5 wordt geleverd met een nieuwe functie genaamd Asset Sourcing. De beheerder moet de functie Asset Sourcing in Experience Manager Assets configureren om deze functie in te schakelen voor de Brand Portal-gebruikers. Voor meer informatie, verwijs naar [ Enable Activa die ](brand-portal-asset-sourcing.md).



**Ques. Wie kan een map met bijdragen maken?**

**Ans.** Om het even welke gebruiker van Experience Manager Assets die toestemmingen heeft om een nieuwe omslag in Experience Manager Assets tot stand te brengen, kan de omslag van de a **Bijdrage** tot stand brengen. Om de omslag van de a **Bijdrage** tot stand te brengen, creeer een nieuwe omslag van type **Bijdrage van Activa**.
Deze map wordt gedeeld met de actieve Brand Portal-gebruikers voor een bijdrage.



**Ques. Wat bevat een omslag van de Bijdrage?**

**Ans.** **de omslag van de Bijdrage** bevat twee subfolders **NIEUW** en **GEDEELD**. In eerste instantie is de map NEW leeg en bevat de map SHARED de referentie-inhoud (herbruikbare elementen) voor de Brand Portal-gebruikers.
De gebruikers van Brand Portal hebben toegang tot de **omslag van de Bijdrage** en uploaden inhoud in de **NIEUWE** omslag.



**Ques.  Kan ik de naam van een bestaande omslag van de Bijdrage wijzigen?**

**Ans.** **Nr**, kunt u niet de naam van een bestaande **omslag van de Bijdrage** wijzigen.



**Ques. Wat zijn activa vereisten met de bijdrage van r.t?**

**Ans.** het **Korte** document in bijlage aan de **omslag van de Bijdrage** en de verwijzingsinhoud (herbruikbare activa) uploadde in de **GEDEELDE** omslag helpt de gebruiker van Brand Portal de behoefte van bijdrage en verwachtingen als medewerker begrijpen, en collectief geroepen als activavereisten.



**Ques. Kan ik middelen aan om het even welke toegelaten omslag uploaden?**

**Ans.** Niet alle toegestane mappen. Een gebruiker van Brand Portal kan inhoud slechts aan de **omslag van de Bijdrage** uploaden die door de beheerder van Experience Manager Assets of van Brand Portal wordt gedeeld.



**Ques. Hoe krijg ik toegang tot een omslag van de Bijdrage?**

**Ans.** u kunt tot de omslag van de a **Bijdrage** toegang hebben slechts als het met u is gedeeld. U krijgt een e-mail-/pulsmelding wanneer een map met bijdragen met u wordt gedeeld. U kunt de map Contribution openen via de koppeling die in de e-mail wordt gedeeld, of u kunt zich aanmelden bij uw Brand Portal-exemplaar en naar het belpictogram gaan voor kennisgeving om de map Contribution te openen.

>[!NOTE]
>
>Als u geen bestaande Brand Portal-gebruiker bent, vraagt u de Experience Manager Assets-beheerder om uw gebruiker in de beheerconsole te maken en uw profiel toe te voegen aan het gebruikersconfiguratiebestand in de gebruikerslijst van Brand Portal.

**Ques. Wat is het Formaat van het Csv- dossier voor gebruikersinvoer?**

**Ans.** De indeling is dezelfde als de indeling die door de Admin Console wordt ondersteund bij het importeren van bulkgebruikers. E-mail, voornaam en achternaam zijn verplicht.



**Ques. Wat vult de lijst van gebruikers (Brand Portal contributors) in de de gebruikersdrop-down van de Bijdrage van Activa?**

**Ans.** De gebruikers in de vervolgkeuzelijst worden gevuld vanuit het Brand Portal-bestand voor gebruikersconfiguratie (.csv) dat is geüpload in Experience Manager Assets.



**Ques. Waar kan ik het statuut van invoer en publiceer banen zien?**

**Ans.** in Experience Manager Assets, kunt u het statuut van de invoer in **async** baanpagina zien. In Brand Portal kunt u de status van een publicatietaak zien in **[!UICONTROL Tools > Asset Contribution status]** .



**Ques. Wat is de frequentie van een de invoerbaan die periodiek in Experience Manager loopt?**

**Ans.** In Experience Manager Assets worden om de vijf minuten opiniepeilingen uitgevoerd.



**Ques. Is er om het even welke drempel op het aantal tijden een omslag van Brand Portal aan Experience Manager Assets kan worden gepubliceerd?**

**Ans.** Nr, worden alle activa in de **NIEUWE** omslag gepubliceerd aan Experience Manager Assets ongeacht het feit zij vroeger werden gepubliceerd. Telkens als de omslag van de a **Bijdrage** van Brand Portal aan Experience Manager Assets wordt gepubliceerd, treedt het de inhoud van de **NIEUWE** omslag met voeten.



**Ques. Hoe te om nieuwe activa in een omslag van de Bijdrage te uploaden?**

**Ans.** verwijs naar de gedetailleerde documentatie voor [ Uploading activa aan de omslag van de Bijdrage ](brand-portal-publish-contribution-folder-to-brand-portal.md).



**Ques. Ik zie geen duimnagels/voorproeven op de activa die aan de NIEUWE omslag door een gebruiker van Brand Portal worden geupload?**

**Ans.** Het is zo ontworpen, omdat er geen workflow wordt uitgevoerd aan het einde van Brand Portal.



**Ques. Wat gebeurt er als een omslag van Experience Manager Assets aan Brand Portal wordt gepubliceerd die in flux is?**

**Ans.** In Experience Manager Assets worden logbestanden voor elke keer dat een map naar Brand Portal wordt gepubliceerd, bijgehouden. Op het moment van publicatie worden alle elementen die niet naar Brand Portal zijn gepubliceerd, in een replicatiewachtrij geplaatst. Middelen die aan de map worden toegevoegd nadat de publicatietaak is geactiveerd, worden niet gepubliceerd naar Brand Portal. Wanneer de Experience Manager Assets-gebruiker de map opnieuw publiceert, worden alleen de elementen die niet eerder zijn gepubliceerd (in de replicatiewachtrij), gepubliceerd naar Brand Portal.
Dit geldt voor alle mappen die van Experience Manager Assets naar Brand Portal worden gepubliceerd en voor de map SHARED in de map Contribution.

**Ques. Wie neem ik contact op met vragen?**

**Ans.** Neem contact op met de accountmanager of de klantenondersteuning van de Adobe.

>[!NOTE]
>
>De releaseplanning is tijdelijk en kan worden gewijzigd. Neem contact op met de accountmanager of de klantenondersteuning van de Adobe voor het bijgewerkte releaseprogramma.


## Toegang tot en ondersteuning voor producten (beperkt aantal sites) {#product-access-and-support-restricted-sites}

Deze sites zijn alleen beschikbaar voor klanten. Als u een klant bent en toegang nodig hebt, neemt u contact op met de accountmanager van de Adobe.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
