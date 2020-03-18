---
title: Gasttoegang tot Brand Portal
seo-title: Gasttoegang tot Brand Portal
description: Gasttoegang toestaan en de moeite besparen om aan boord van een groot aantal gebruikers te gaan die niet hoeven te worden geverifieerd.
seo-description: Gasttoegang toestaan en de moeite besparen om aan boord van een groot aantal gebruikers te gaan die niet hoeven te worden geverifieerd.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: mgulati
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
translation-type: tm+mt
source-git-commit: 8554b9768040b59d2b1a03a3703b2d7235e63bcb

---


# Gasttoegang tot Brand Portal {#guest-access-to-brand-portal}

Het portaal van het Merk AEM staat gasttoegang tot het portaal toe. Een gastgebruiker heeft geen geloofsbrieven nodig om het portaal in te gaan en heeft toegang tot de openbare activa (en inzamelingen) van het portaal. De gebruikers in de gastzitting kunnen activa aan hun lichtbak (privé inzameling) toevoegen en het zelfde downloaden tot hun zitting duurt, die 2 uren van het begin van de zitting is tenzij de gastgebruiker aan [[!UICONTROL Sessie van het Eind]](#exit-guest-session)verkiest.

Dankzij de functie voor toegang van gasten kunnen organisaties [snel goedgekeurde middelen](../using/brand-portal-sharing-folders.md#how-to-share-folders) delen met het beoogde publiek op schaal zonder dat ze zich aan boord hoeven te bevinden. Brand Portal 6.4.2 en hoger is uitgerust voor meerdere gelijktijdige gastgebruikers, hetgeen 10% van de totale gebruikersquota per organisatie is. Door gasttoegang toe te staan, bespaart u tijd om scores van gebruikers aan boord te beheren en te installeren die beperkte functies op het Brand Portal moeten gebruiken.\
Organisaties kunnen gasttoegang inschakelen (of uitschakelen) op de Brand Portal-account van de organisatie met **[!UICONTROL Allow Guest Access]** optie van de **[!UICONTROL Access]** instellingen in het deelvenster met beheergereedschappen.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Beginnen met gastsessie {#begin-guest-session}

Als u het Brand Portal anoniem wilt openen, selecteert u **[!UICONTROL Click here]** de optie die hoort bij het welkomstscherm van **[!UICONTROL Guest Access?]** Brand Portal. Ga de veiligheidscontrole van de catcha in om toegang te verlenen om het Portaal van het Merk te gebruiken.

![](assets/bp-login-screen.png)

## Duur gastsessie {#guest-session-duration}

Een gastgebruikerssessie blijft 2 uur actief. Dit betekent dat de staat van de **[!UICONTROL Lightbox]** wordt bewaard tot 1 uur van de tijd van het zittingsbegin, en na 2 uur de huidige gastzitting opnieuw begint zodat wordt de Lichtbakstaat verloren.\
Bijvoorbeeld, meldt een gastgebruiker zich bij 1500 uren aan het Portaal van het Merk aan en voegt activa aan Lichtbak voor download bij 16:50 uren toe. Als de gebruiker de **[!UICONTROL Lightbox]** verzameling (of zijn middelen) niet vóór 17.00 uur downloadt, **[!UICONTROL Lightbox]** wordt de verzameling leeg omdat de gebruiker de sessie aan het einde van 1 uur (dat is 1700 uur) opnieuw moet starten.

## Gelijktijdige gastsessies toegestaan {#concurrent-guest-sessions-allowed}

Het aantal gelijktijdige gastsessies is beperkt tot 10% van de totale gebruikersquota per organisatie. Dit betekent voor een organisatie met gebruikersquota van 200, maximaal 20 gastgebruikers kunnen tezelfdertijd werken. De 21ste gebruiker wordt ontzegd toegang, en kan als gast slechts toegang hebben als de zitting van om het even welke 20 actieve gastgebruikers beëindigt.

## Gebruikersinteractie van gasten met Brand Portal {#guest-user-interaction-with-brand-portal}

### Navigatie gastinterface

Bij het ingaan van het Portaal van het Merk als gast, kunnen de gebruikers alle [activa en omslagen zien die openbaar of met gastgebruikers uitsluitend worden gedeeld](../using/brand-portal-sharing-folders.md#sharefolders) . Deze weergave is de weergave alleen voor inhoud. In deze weergave worden elementen in de kaart-, lijst- of kolomindeling weergegeven.

![](assets/disabled-folder-hierarchy1.png)

Nochtans, zien de gastgebruikers de omslagboom (die van de wortelomslag) begint en de gedeelde omslagen die binnen hun respectieve ouderomslagen bij het aanmelden bij het Portaal van het Merk worden geschikt, als de beheerders de configuratie van de Hiërarchie van de [Enable Omslag](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) hebben toegelaten.

Deze bovenliggende mappen zijn de virtuele mappen en er kunnen geen handelingen op worden uitgevoerd. U kunt deze virtuele mappen herkennen met een vergrendelingspictogram.

In tegenstelling tot de gedeelde mappen zijn er geen actietaken zichtbaar bij het aanwijzen of selecteren van deze taken **[!UICONTROL Card View]**. **[!UICONTROL Overview]** wordt weergegeven bij het selecteren van een virtuele map in **[!UICONTROL Column View]** en **[!UICONTROL List View]**.

>[!NOTE]
>
>De standaardminiatuur van de virtuele mappen is de miniatuurafbeelding van de eerste gedeelde map.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL View Settings]** optie staat de gastgebruikers toe om kaartgrootte in **[!UICONTROL Card View]** of kolommen aan vertoning binnen aan te passen **[!UICONTROL List View]**.

![](assets/nav-guest-user.png)

Met **[!UICONTROL Content tree]** deze opties kunt u de hiërarchie van elementen doorlopen.

![](assets/guest-login-ui.png)

Het Portaal van het merk verstrekt **[!UICONTROL Overview]** **[!UICONTROL Asset Properties]** optie aan gastgebruikers om geselecteerde activa/omslagen te bekijken. De **[!UICONTROL Overview]** optie is zichtbaar:

* Selecteer bovenaan op de werkbalk een middel/map.
* In de vervolgkeuzelijst selecteert u de spoorkiezer.
Als gebruikers de **[!UICONTROL Overview]** optie selecteren terwijl een element/map is geselecteerd, kunnen ze de titel, het pad en het tijdstip van het maken van het element zien. Terwijl de gebruiker met de optie Pagina met elementdetails selecteren **[!UICONTROL Overview]** metagegevens van het element kan bekijken.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)<br />

**[!UICONTROL Navigation]** met de optie in het linkerspoor kunt u van bestanden naar verzamelingen navigeren en in de gastsessie teruggaan, zodat gebruikers door elementen in bestanden of verzamelingen kunnen bladeren.

**[!UICONTROL Filter]** gastgebruikers kunnen middelenbestanden en mappen filteren met behulp van zoekvoorspelden die door de beheerder zijn ingesteld.

### Mogelijkheden voor gastgebruikers

Gastgebruikers hebben toegang tot publieke middelen op het Brand Portal en hebben ook weinig beperkingen zoals verder wordt besproken.

**Gastgebruikers kunnen**:

* Open alle openbare mappen en verzamelingen die voor alle gebruikers van het Brand Portal zijn bedoeld.
* Blader door leden, detailpagina en bekijk de volledige elementenweergave van de leden van alle openbare mappen en verzamelingen.
* Middelen zoeken in openbare mappen en verzamelingen.
* Elementen toevoegen aan lichtbakverzameling. Deze veranderingen in de inzameling blijven tijdens de zitting bestaan.
* Download elementen rechtstreeks of via lichtbakverzameling.

**Gastgebruikers kunnen dit niet**:

* Maak verzamelingen en opgeslagen zoekopdrachten of deel deze verder.
* Toegang tot de instellingen voor mappen en verzamelingen.
* Elementen delen als koppelingen.

### Elementen downloaden in gastsessie

Gastgebruikers kunnen elementen die algemeen of exclusief met gastgebruikers worden gedeeld, rechtstreeks downloaden naar Brand Portal. De gebruikers van de gast kunnen activa aan **[!UICONTROL Lightbox]** (openbare inzameling) ook toevoegen, en de **[!UICONTROL Lightbox]** inzameling downloaden alvorens hun zitting verloopt.

Gebruik het downloadpictogram van:

* Miniaturen van snelle handelingen die worden weergegeven wanneer u de muisaanwijzer op het element of de verzameling plaatst
* De werkbalk bovenaan, die wordt weergegeven bij het selecteren van het element of de verzameling

![](assets/download-on-guest.png)

Als u **[!UICONTROL Enable download acceleration]** in het [!UICONTROL Download] dialoogvenster selecteert, kunt u de downloadprestaties [](../using/accelerated-download.md)verbeteren.

## Bezoekerssessie afsluiten {#exit-guest-session}

Om een gastzitting weg te gaan, gebruik **[!UICONTROL End Session]** van de opties beschikbaar in de kopbal. Nochtans, als browser lusje-gebruikt voor gast zitting-inactief dan de zitting na twee uren van inactiviteit automatisch verloopt.

![](assets/end-guest-session.png)

## Bewaking van activiteiten van gastgebruikers {#monitoring-guest-user-activities}

De beheerders kunnen gastgebruikersinteractie met het Portaal van het Merk controleren. De rapporten die in het Portaal van het Merk worden geproduceerd kunnen zeer belangrijke inzichten in gastgebruikersactiviteiten verstrekken. Bijvoorbeeld, kan het **[!UICONTROL Download]** rapport worden gebruikt om de telling van activa te volgen die door de gastgebruiker worden gedownload. **[!UICONTROL User Logins]** het rapport kan informeren wanneer de gastgebruiker het laatst bij het portaal en de frequentie van logins in een gespecificeerde duur het programma heeft geopend.