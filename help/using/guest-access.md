---
title: Toegang voor gasten tot Brand Portal
description: Gasttoegang toestaan en de moeite besparen om aan boord van een groot aantal gebruikers te gaan zonder verificatie.
contentOwner: VG
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
exl-id: ecce0a45-abae-41c4-9ea7-5dfdcf19e5ea
source-git-commit: 4c701781e7dc62b9d2b018fd13b1ae9616bbb840
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 0%

---

# Toegang voor gasten tot Brand Portal {#guest-access-to-brand-portal}

Experience Manager Assets Brand Portal biedt gasttoegang tot het portaal. Een gastgebruiker heeft geen geloofsbrieven nodig om het portaal in te gaan en heeft toegang tot de openbare activa (en inzamelingen) van het portaal. De gebruikers in de gastzitting kunnen activa aan lichtbak (privé inzameling) toevoegen en het zelfde downloaden tot hun zitting duurt of tenzij de gastgebruiker aan [[!UICONTROL End Session]](#exit-guest-session) verkiest. Een gastgebruikerssessie blijft 15 minuten actief.

De de toegangsfunctionaliteit van de gast laat organisaties toe om [&#x200B; goedgekeurde activa snel &#x200B;](../using/brand-portal-sharing-folders.md#how-to-share-folders) met het voorgenomen publiek aan schaal te delen zonder het moeten hen aan boord hebben. Brand Portal 6.4.2 en hoger is uitgerust om meerdere gelijktijdige gastgebruikers te bedienen, wat 10% van de totale gebruikersquota per organisatie is. Door gasttoegang toe te staan, bespaart u tijd om scores van gebruikers met beperkte functionaliteit op Brand Portal te beheren en aan boord te hebben.\
Organisaties kunnen toegang voor gasten inschakelen (of uitschakelen) in de Brand Portal-account van de organisatie met de optie **[!UICONTROL Allow Guest Access]** in de instellingen van **[!UICONTROL Access]** in het deelvenster met beheergereedschappen.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Beginnen met gastsessie {#begin-guest-session}

Als u Brand Portal anoniem wilt invoeren, selecteert u **[!UICONTROL Click here]** voor **[!UICONTROL `Guest Access?`]** in het welkomstscherm van Brand Portal. Voer de beveiligingscontrole van Captcha in om toegang te verlenen tot het gebruik van de Brand Portal.

![](assets/bp-login-screen.png)

## Duur gastsessie {#guest-session-duration}

Een gastgebruikerssessie blijft 15 minuten actief.
Bij dit proces blijft de status van de **[!UICONTROL Lightbox]** gedurende 15 minuten vanaf de begintijd van de sessie behouden. Daarna, begint de huidige gastzitting opnieuw, veroorzakend de Lichtbakstaat om worden verloren.

Een gastgebruiker meldt zich bijvoorbeeld om 1500 uur aan bij Brand Portal en voegt middelen toe aan **[!UICONTROL Lightbox]** voor download om 15:05 uur. Als de gebruiker de **[!UICONTROL Lightbox]** -verzameling (of de bijbehorende elementen) niet vóór 15:15 uur downloadt (binnen 15 minuten na aanmelden), moet de gebruiker de sessie opnieuw starten. **[!UICONTROL Lightbox]** is leeg, wat betekent dat de geüploade elementen niet meer beschikbaar zijn als de sessie is verloren.

## Gelijktijdige gastsessies toegestaan {#concurrent-guest-sessions-allowed}

Het aantal gelijktijdige gastsessies is beperkt tot 10% van de totale gebruikersquota per organisatie. Het betekent dat voor een organisatie die een gebruikersquotum van 200 heeft, een maximum van 20 gastgebruikers tezelfdertijd kunnen werken. De 21ste gebruiker wordt ontzegd toegang, en kan als gast slechts toegang hebben als de zitting van om het even welke 20 actieve gastgebruikers beëindigt.

>[!NOTE]
>
>Brand Portal verzendt geen melding als het aantal gebruikers met licentie de contractueel vastgelegde waarde (quota) overschrijdt. Bovendien worden de activiteiten van de gebruikers met een licentie niet beperkt.

## Gebruikersinteractie Gast met Brand Portal {#guest-user-interaction-with-brand-portal}

### Navigatie gastinterface

Bij het ingaan van Brand Portal als gast, kunnen de gebruikers alle [&#x200B; activa en omslagen zien die &#x200B;](../using/brand-portal-sharing-folders.md#sharefolders) openbaar of met gastgebruikers exclusief worden gedeeld. Deze weergave is de weergave alleen voor inhoud. In deze weergave worden elementen in de kaart-, lijst- of kolomindeling weergegeven.

![](assets/disabled-folder-hierarchy1.png)


Als de beheerders [&#x200B; toelaten laat de Hiërarchie van de Omslag &#x200B;](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) toe, zien de gastgebruikers de omslagboom van de wortel en gedeelde omslagen binnen hun ouderomslagen op het registreren in Brand Portal.

Deze bovenliggende mappen zijn virtuele mappen en er kunnen geen handelingen op worden uitgevoerd. U kunt deze virtuele mappen herkennen met een vergrendelingspictogram.

In tegenstelling tot de gedeelde mappen zijn er geen actietaken zichtbaar wanneer u deze in **[!UICONTROL Card View]** aanwijst of selecteert. De knop **[!UICONTROL Overview]** wordt weergegeven bij het selecteren van een virtuele map in **[!UICONTROL Column View]** en **[!UICONTROL List View]** .

>[!NOTE]
>
>De standaardminiatuur van de virtuele mappen is de miniatuurafbeelding van de eerste gedeelde map.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

Met de optie **[!UICONTROL View Settings]** kunnen gastgebruikers de kaartgrootten in **[!UICONTROL Card View]** of kolommen aanpassen en deze weergeven in **[!UICONTROL List View]** .

![](assets/nav-guest-user.png)

Met **[!UICONTROL Content tree]** kunt u door de hiërarchie van elementen navigeren.

![](assets/guest-login-ui.png)

Brand Portal biedt een **[!UICONTROL Overview]** -optie voor gastgebruikers om **[!UICONTROL Asset Properties]** van geselecteerde elementen/mappen weer te geven. De optie **[!UICONTROL Overview]** is zichtbaar:

* Kies bovenaan op de werkbalk een element of map.
* In de vervolgkeuzelijst selecteert u de spoorkiezer.

Wanneer u de optie **[!UICONTROL Overview]** selecteert terwijl een element of map is geselecteerd, kunnen gebruikers de titel, het pad en het tijdstip zien waarop het element is gemaakt. Terwijl de gebruiker op de pagina met elementdetails de optie **[!UICONTROL Overview]** selecteert, kunnen de metagegevens van het element worden weergegeven.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

Met de optie **[!UICONTROL Navigation]** in de linkertrack kunt u van bestanden naar verzamelingen navigeren en terug in de gastsessie, zodat gebruikers door elementen in bestanden of verzamelingen kunnen bladeren.

Met de optie **[!UICONTROL Filter]** kunnen gastgebruikers elementbestanden en mappen filteren met behulp van zoekvoorspelling die is ingesteld door de beheerder.

### Mogelijkheden voor gastgebruikers

Gastgebruikers hebben toegang tot openbare middelen op Brand Portal en hebben ook weinig beperkingen, zoals verder wordt besproken.

**de gebruikers van de Gast kunnen**:

* Open alle openbare mappen en verzamelingen die voor alle Brand Portal-gebruikers zijn bedoeld.
* Blader door leden, detailpagina en heb een volledige elementweergave van de leden van alle openbare mappen en verzamelingen.
* Middelen zoeken in openbare mappen en verzamelingen.
* Elementen toevoegen aan lichtbakverzameling. Deze veranderingen in de inzameling blijven tijdens de zitting bestaan.
* Download elementen rechtstreeks of via lichtbakverzameling.

**de gebruikers van de Gast kunnen niet**:

* Maak verzamelingen en opgeslagen zoekopdrachten of deel deze verder.
* Toegang tot de instellingen voor mappen en verzamelingen.
* Elementen delen als koppelingen.

### Elementen downloaden in gastsessie

Gastgebruikers kunnen elementen die algemeen of exclusief met gastgebruikers worden gedeeld, rechtstreeks downloaden op Brand Portal. Gastgebruikers kunnen ook elementen toevoegen aan **[!UICONTROL Lightbox]** (openbare verzameling) en de **[!UICONTROL Lightbox]** -verzameling downloaden voordat hun sessie verloopt.

Gebruik het downloadpictogram van:

* Miniaturen van snelle handelingen die worden weergegeven wanneer u de muisaanwijzer op het element of de verzameling plaatst
* De werkbalk bovenaan, die wordt weergegeven bij het selecteren van het element of de verzameling

![](assets/download-on-guest.png)

Het selecteren **[!UICONTROL Enable download acceleration]** in het [!UICONTROL Download] dialoogvakje laat u [&#x200B; de downloadprestaties &#x200B;](../using/accelerated-download.md) verbeteren.

## Bezoekerssessie afsluiten {#exit-guest-session}

Als u een gastsessie wilt afsluiten, gebruikt u **[!UICONTROL End Session]** van de opties in de koptekst. Nochtans, als browser lusje-gebruikt voor gast zitting-inactief dan de zitting na twee uren van inactiviteit automatisch verloopt.

![](assets/end-guest-session.png)

## Bewaking van activiteiten van gastgebruikers {#monitoring-guest-user-activities}

Beheerders kunnen de interactie van gastgebruikers met de Brand Portal controleren. Rapporten die in Brand Portal worden gegenereerd, kunnen belangrijke inzichten bieden in activiteiten van gastgebruikers. Het rapport **[!UICONTROL Download]** kan bijvoorbeeld worden gebruikt om het aantal elementen bij te houden dat door de gastgebruiker is gedownload. Het **[!UICONTROL User Logins]** -rapport kan aangeven wanneer de gastgebruiker zich voor het laatst heeft aangemeld bij het portal en hoe vaak hij zich heeft aangemeld voor een bepaalde duur.
