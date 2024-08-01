---
title: Veelgestelde vragen
description: Bekijk de veelgestelde vragen in de Adobe Experience Manager Assets Brand Portal.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 4c701781e7dc62b9d2b018fd13b1ae9616bbb840
workflow-type: tm+mt
source-wordcount: '1485'
ht-degree: 0%

---

# Veelgestelde vragen {#frequently-asked-questions}

De veelgestelde vragen over Brand Portal zijn toegespitst op de vragen en problemen die eindgebruikers kunnen tegenkomen tijdens het werken met de nieuwste Experience Manager Assets Brand Portal 6.4.6-versie of eerdere versies.


## Brand Portal 6.4.6 Veelgestelde vragen {#faqs-bp646}

**Vraag: Het bestaande eindpunt OAuth van de erfenis (`https://legacy-oauth.cloud.adobe.io/login`) werkt niet. Wat zou de mogelijke reden kunnen zijn?**

**Antwoord:** De oudere configuratie OAuth is verouderd. Voer een upgrade uit van Experience Manager Assets-auteur naar het nieuwste servicepakket en configureer dit via Adobe Developer Console. Zie [ Experience Manager Assets met Brand Portal ](configure-aem-assets-with-brand-portal.md) voor details vormen. Voor oudere OAuth-configuratie werkt u echter totdat u een upgrade uitvoert, het verouderde OAuth-eindpunt wordt bijgewerkt naar `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/` .

**Vraag: Ik kan niet de activa van de bijdrageomslag van Brand Portal aan Experience Manager Assets publiceren na bevordering aan Adobe Developer Console. Mijn auteur-exemplaar staat op Experience Manager Assets 6.5.4. Wat zou de mogelijke reden kunnen zijn?**

**Antwoord:** ja, is er een bekende kwestie terwijl het publiceren van de activa van de bijdrageomslag aan Experience Manager Assets 6.5.4 via Adobe Developer Console.

Het probleem is opgelost in Experience Manager Assets 6.5.5. U kunt uw instantie van Experience Manager Assets aan het recentste de dienstpak bevorderen en [ bevorderen uw configuraties ](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65) op Adobe Developer Console.


**Vraag: Ik zie de inhoud van de bijdrageomslag niet die van Brand Portal in Experience Manager Assets wordt gepubliceerd. Wat zou de mogelijke reden kunnen zijn?**

**Antwoord:** Contacteer uw beheerder van Experience Manager Assets om de configuraties te verifiëren en ervoor te zorgen dat uw huurder van Brand Portal met slechts één de auteursinstantie van Experience Manager Assets wordt gevormd.

Dit probleem doet zich mogelijk voor wanneer u een Brand Portal-medewerker hebt geconfigureerd voor meerdere Experience Manager Assets-auteur-instanties. Bijvoorbeeld, vormt de beheerder de zelfde huurder van Brand Portal op de de auteurinstantie van Experience Manager Assets van een het opvoeren en productiemilieu. In dit geval wordt de functie voor het publiceren van middelen geactiveerd in Brand Portal, maar de instantie van de Experience Manager Assets-auteur importeert het element niet omdat de replicatieagent het token voor het aanvragen niet ontvangt.


**Vraag: Ik kan activa van Experience Manager Assets aan Brand Portal niet publiceren. Het replicatielogboek verklaart dat de verbinding uit timed. Is er een snelle oplossing?**

**Antwoord:** gewoonlijk ontbreekt het publiceren met een onderbrekingsfout als er veelvoudige hangende verzoeken in de replicatierij zijn. Om deze kwestie op te lossen, zorg ervoor dat de replicatieagenten worden gevormd om onderbreking te vermijden.

Voer de volgende stappen uit om de replicatieagent te vormen:

1. Meld u aan bij de Experience Manager Assets-auteur.
1. Van het **paneel van Hulpmiddelen**, navigeer aan **[!UICONTROL Deployment]** > **[!UICONTROL Replication]**.
1. Klik op **[!UICONTROL `Agents on author`]** op de pagina Replicatie. U kunt de vier replicatieagenten voor uw huurder van Brand Portal zien.
1. Klik de replicatieagent URL om de agentendetails te openen.
1. Klik op **[!UICONTROL Edit]** om de instellingen van de replicatieagent te bewerken.
1. Klik op de tab **[!UICONTROL Extended]** in de agentinstellingen.
1. Schakel het selectievakje **[!UICONTROL Close Connection]** in.
1. Herhaal stap 4 door 7 om alle vier replicatieagenten te vormen.
1. Start de server opnieuw en controleer de verbinding.


## Brand Portal 6.4.5 - Veelgestelde vragen {#faqs-bp645}

**Vraag: Wat is de belangrijkste verandering in Brand Portal 6.4.5 versie?**

**Antwoord:** Experience Manager Assets Brand Portal 6.4.5 laat gebruikers inhoud uploaden en de omslag van de Bijdrage terug naar Experience Manager Assets direct van Brand Portal publiceren, zonder beheerderrechten te vereisen. Voor meer informatie, zie [ Middelen van Activa in Brand Portal ](brand-portal-asset-sourcing.md).



**Vraag: Heb ik toegang tot om het even welke bestaande activa, eigenschappen, of configuraties verloren ik heb gecreeerd?**

**Antwoord:** Alle bestaande eigenschappen en configuraties blijven intact. Uw eindgebruikers worden niet beïnvloed en uw inhoud blijft intact.



**Vraag: Wanneer verplaats ik naar de nieuwe versie van Brand Portal?**

**Antwoord:** Brand Portal 6.4.5 werd vrijgegeven aan productie in Oktober 2019. En de volgende Brand Portal-versie wordt verwacht voor maart 2020.
Voor updates en versieverandering, adviseert de Adobe u de [ Nota&#39;s van de Versie ](brand-portal-release-notes.md) volgen en [ wat in Brand Portal ](whats-new.md) nieuw is.



**Vraag: Zijn mijn gebruikers beïnvloed?**

**Antwoord:** Brand Portal 6.4.5 versie is exclusief binnen Brand Portal, zodat is er geen effect aan uw eind - gebruikers.



**Vraag: Is er om het even welke actie die op mijn deel als gebruiker van Brand Portal wordt vereist?**

**Antwoord:** versie van Brand Portal 6.4.5 komt met een nieuwe eigenschap genoemd Middel. De beheerder moet de functie Asset Sourcing in Experience Manager Assets configureren om deze functie in te schakelen voor de Brand Portal-gebruikers. Voor meer informatie, verwijs naar [ Enable Activa die ](brand-portal-asset-sourcing.md).



**Vraag: Wie kan een omslag van de Bijdrage tot stand brengen?**

**Antwoord:** Om het even welke gebruiker van Experience Manager Assets die toestemmingen heeft om een omslag in Experience Manager Assets tot stand te brengen kan a **tot de omslag van de Bijdrage** leiden. Om de omslag van de a **Bijdrage** tot stand te brengen, creeer een omslag van type **Bijdrage van Activa**.
Deze map wordt gedeeld met de actieve Brand Portal-gebruikers voor een bijdrage.



**Vraag: Wat bevat een omslag van de Bijdrage?**

**Antwoord:** **3} omslag van de Bijdrage {bevat twee subfolders** NIEUW **en** GEDEELD **.** In eerste instantie is de map NEW leeg en bevat de map SHARED de referentie-inhoud (herbruikbare elementen) voor de Brand Portal-gebruikers.
De gebruikers van Brand Portal hebben toegang tot de **omslag van de Bijdrage** en uploaden inhoud in de **NIEUWE** omslag.



**Vraag: Kan ik de naam van een bestaande omslag van de Bijdrage wijzigen?**

**Antwoord:** **Nr**, kunt u niet de naam van een bestaande **omslag van de Bijdrage** wijzigen.



**Vraag: Wat zijn activa vereisten met r.t bijdrage?**

**Antwoord:** het **Korte** document in de **omslag van de Bijdrage** en de verwijzingsinhoud in de **GEDEELDE** omslag helpen de gebruikers van Brand Portal de bijdragebehoeften en de verwachtingen begrijpen. Samen staan ze bekend als de vereisten inzake activa.

**Vraag: Kan ik activa aan om het even welke toegelaten omslag uploaden?**

**Antwoord:** niet alle toegelaten omslagen. Een gebruiker van Brand Portal kan inhoud slechts aan de **omslag uploaden van de Bijdrage** die Experience Manager Assets of de beheerder van Brand Portal deelt.



**Vraag: Hoe krijg ik toegang tot een omslag van de Bijdrage?**

**Antwoord:** u kunt tot de omslag van de a **Bijdrage** toegang hebben slechts als het met u is gedeeld. U krijgt een e-mail-/pulsmelding wanneer een map met bijdragen met u wordt gedeeld. U kunt de map Contribution openen via de koppeling die u in de e-mail deelt. U kunt zich ook aanmelden bij uw Brand Portal-exemplaar en naar het belpictogram gaan voor meldingen voor toegang tot de map Contribution.

>[!NOTE]
>
>Als u geen Brand Portal-gebruiker bent, vraagt u de Experience Manager Assets-beheerder om uw gebruiker in de Admin Console te maken. Voeg vervolgens uw profiel toe aan het gebruikersconfiguratiebestand in de gebruikerslijst van Brand Portal.


**Vraag: Wat is het Formaat van het Csv- dossier voor gebruikersimport?**

**Antwoord:** het formaat past aan welke Admin Console voor bulkgebruikersimport steunt. E-mail, voornaam en achternaam zijn verplicht.



**Vraag: Wat bevolkt de lijst van gebruikers (Brand Portal contributors) in de de gebruikersdrop-down van de Bijdrage van Activa?**

**Antwoord:** de gebruikers in drop-down zijn bevolkt van het dossier van de de gebruikersconfiguratie van Brand Portal (.csv) dat in Experience Manager Assets wordt geupload.



**Vraag: Waar kan ik het statuut van invoer zien en banen publiceren?**

**Antwoord:** in Experience Manager Assets, kunt u het statuut van de invoer in de **async** baanpagina zien. In Brand Portal kunt u de status van een publicatietaak zien in **[!UICONTROL Tools > Asset Contribution status]** .



**Vraag: Wat is de frequentie van een de invoerbaan die periodiek in Experience Manager loopt?**

**Antwoord:** in Experience Manager Assets, wordt de opiniepeiling in werking gesteld om de vijf minuten.



**Vraag: Is er een drempel op het aantal tijden een omslag van Brand Portal aan Experience Manager Assets kan worden gepubliceerd?**

**Antwoord:** Nr, worden alle activa in de **NIEUWE** omslag gepubliceerd aan Experience Manager Assets ongeacht het feit zij vroeger werden gepubliceerd. Telkens als de omslag van de a **Bijdrage** van Brand Portal aan Experience Manager Assets wordt gepubliceerd, vervangt het de inhoud van de **NIEUWE** omslag.



**Vraag: Hoe te om nieuwe activa in een omslag van de Bijdrage te uploaden?**

**Antwoord:** verwijs naar de gedetailleerde documentatie voor [ Uploading activa aan de omslag van de Bijdrage ](brand-portal-publish-contribution-folder-to-brand-portal.md).



**Vraag: Ik kan geen duimnagels of voorproeven voor de activa zien die aan de NIEUWE omslag worden geupload.**

**Antwoord:** het is zoals ontworpen, omdat er geen werkschema in werking wordt gesteld aan het eind van Brand Portal.



**Vraag: Wat gebeurt als een omslag van Experience Manager Assets aan Brand Portal wordt gepubliceerd die in flux is?**

**Antwoord:** in Experience Manager Assets, worden de logboeken gehandhaafd telkens als een omslag aan Brand Portal wordt gepubliceerd. Op het moment van publicatie worden alle elementen die niet naar Brand Portal zijn gepubliceerd, toegevoegd aan een replicatiewachtrij. Middelen die aan de map worden toegevoegd nadat de publicatietaak is geactiveerd, worden niet gepubliceerd naar Brand Portal. Wanneer een Experience Manager Assets-gebruiker de map opnieuw publiceert, worden alleen de elementen die niet eerder zijn gepubliceerd (in de replicatiewachtrij), gepubliceerd naar Brand Portal. Dit proces geldt voor alle mappen die van Experience Manager Assets naar Brand Portal worden gepubliceerd en voor de map SHARED in de map Contribution.

**Vraag: Wie contacteer ik met vragen?**

**Antwoord:** contacteer uw Manager van de Rekening van de Adobe of Klantenondersteuning.

>[!NOTE]
>
>De releaseplanning is tijdelijk en kan worden gewijzigd. Neem contact op met de accountmanager of de klantenondersteuning van de Adobe voor het bijgewerkte releaseprogramma.


## Toegang tot en ondersteuning voor producten (beperkt aantal sites) {#product-access-and-support-restricted-sites}

Deze sites zijn alleen beschikbaar voor klanten. Neem contact op met de accountmanager van de Adobe als u een klant bent en toegang nodig hebt.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
