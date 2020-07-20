---
title: Release-opmerkingen
seo-title: Release-opmerkingen
description: Krijg inzicht in de eigenschappen, de verhogingen, de kritieke kwesties die, en de bekende kwesties in de Adobe Experience Manager Middelen van het Merk Portal 6.4.6.2 versie worden opgelost.
seo-description: Krijg inzicht in de verhogingen, de kritieke kwesties die, en bekende kwesties in de Adobe Experience Manager Middelen van het Merk Portal 6.4.6.2 versie worden opgelost.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: ec588b0e9e1af5f813e13670a0616694aa9d5abe
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 3%

---


# Releaseopmerkingen {#release-notes}

Krijg inzicht in de nieuwe eigenschappen, de verhogingen, de kritieke kwesties die, en de bekende kwesties in de Adobe Experience Manager Middelen van het Merk Portal 6.4.6.2 versie worden opgelost.

## Geen informatie {#release-information}

| Product | Brandportal Adobe Experience Manager Assets |
|---|---|
| Versie | 6.4.6.2 |
| Date | juni 2020 |

## Overzicht {#overview}

Met behulp van de Adobe Experience Manager (AEM) Assets Brand Portal kunt u eenvoudig goedgekeurde creatieve elementen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten. Het draagt bij tot een efficiëntere verdeling van activa, versnelt de marktintroductie van activa en vermindert het risico van niet-naleving en ongeoorloofde toegang. Merkportal biedt gebruikers de mogelijkheid om in door het bedrijf goedgekeurde indelingen te zoeken, te bekijken, voor te vertonen, te downloaden en te exporteren, altijd en overal.

## Nieuwe functies in 6.4.6.2 {#what-s-new-in-6462}

### Kritieke problemen opgelost {#critical-issues-fixed-6462}

Deze release bevat oplossingen voor de volgende kritieke problemen:

* Als u een gepubliceerd metagegevensschema verwijdert uit Brand Portal, treedt er een fout op.

* Als de beheerder Experience Manager Assets 6.5.4 configureert met Brand Portal via Adobe Developer Console, kan de gebruiker van het Brand Portal de middelen van de map met bijdragen niet publiceren van Brand Portal naar Experience Manager.

* Dubbele replicatie van de bovenliggende mappen die conflicten veroorzaken.

* De gebruiker kan het rapport van het Aandeel van de Verbinding niet produceren.

* De gebruiker kan de geheimen van MAC voor een Poorteindpunt van het Merk kopiëren gebruikend copyPage bevel.

* cqTags die opnieuw indexeren op VA5-kloon.


### Bekende problemen {#known-issues-6462}

Deze release bevat de volgende bekende problemen:

* De koppeling Delen voor verzamelingen is momenteel zichtbaar voor de gebruikers van de viewer.

* Als de naam van een map in de hiërarchie wordt gewijzigd van AEM Assets en de geneste map met een element wordt gepubliceerd naar Brand Portal, wordt de titel van de map niet bijgewerkt in Brand Portal totdat de hoofdmap opnieuw wordt gepubliceerd.


## Nieuwe functies in 6.4.6 {#what-s-new-in-646}

### Nieuwe functies {#new-feature}

Deze release bevat de volgende nieuwe functies:

* Captcha voor gastaanmelding bij Brand Portal. See, [Brand Portal guest access](../using/guest-access.md) for more information.

* Brand Portal wordt nu ondersteund door de cloudservice AEM Assets. U kunt AEM Assets vormen kon met het Portaal van het Merk dienst doen om activa met de gebruikers van het Portaal van het Merk te delen en te verspreiden.
Voor meer informatie, zie de de wolkendienst van AEM Assets met het Portaal [van het Merk](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html)vormen.

### Verbeteringen {#enhancements-646}

Deze release van Brand Portal bevat de volgende verbeteringen:

* In AEM 6.3 en hoger wordt het machtigingskanaal tussen AEM Assets en Brand Portal gewijzigd. AEM Assets worden nu geconfigureerd met het Brand Portal via de Adobe Developer Console, die een IMS-token aanschaft voor goedkeuring door uw Pandhouder.

>[!NOTE]
>
>Configuratie via verouderde OAuth wordt vanaf 6 april 2020 niet meer ondersteund en wordt gewijzigd in configuratie via Adobe Developer Console.

>[!TIP]
>
>***Alleen voor bestaande klanten***
>
>De verouderde configuratie van de Gateway OAuth zal blijven werkend voor bestaande klanten.
>
>Als u problemen ondervindt met de oudere configuratie van OAuth Gateway, verwijdert u de bestaande configuratie en maakt u een nieuwe configuratie via de Adobe Developer Console.

For more information, see [Configure AEM Assets with Brand Portal](configure-aem-assets-with-brand-portal.md)

### Kritieke problemen opgelost {#critical-issues-fixed}

Deze release bevat oplossingen voor de volgende kritieke problemen:

* Vervolgkeuzemenu&#39;s van het metagegevensschema zijn niet zichtbaar in de eigenschappen van elementen.

* In het subschema Metagegevens worden geen tabbladen weergegeven die zijn gebaseerd op mimetype in eigenschappen van elementen.

* Als u het schema voor metagegevens niet publiceert, wordt een foutbericht weergegeven, maar wordt het schema op de achtergrond verwijderd.

* Voorvertoningsafbeelding wordt niet weergegeven voor een gepubliceerd element.

* De gebruiker kan geen activa publiceren of unpublish die één enkel citaat in de naam bevatten.

* De voorwaarden worden niet weergegeven tijdens het downloaden van meerdere elementen.

* Kleine beveiligingskwetsbaarheden verholpen.

### Bekende problemen {#known-issues}

Deze release bevat de volgende bekende problemen:

* Gebruikers van Brand Portal kunnen geen middelen uit de bijdragemap publiceren naar AEM Assets bij een upgrade naar Adobe Developer Console op AEM 6.5.4.

   Dit probleem wordt opgelost in het volgende servicepack 6.5.5.

   Voor directe correctie op AEM 6.5.4 wordt aangeraden de hotfix [te](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) downloaden en op de auteurinstantie te installeren.

* De optie Systeemuitvoeringen uitsluiten werkt niet correct tijdens het downloaden van een element.


## Talen {#languages}

De gebruikersinterface van het Merk Portal is beschikbaar in de volgende talen:

* Engels
* Duits
* Frans
* Spaans
* Italiaans
* Braziliaans Portugees
* Japans
* Vereenvoudigd Chinees
* Koreaans

## Gecertificeerde Platforms {#certified-platforms}

Als u wilt weten welke platforms zijn gecertificeerd voor uitvoering met deze versie van Brand Portal, raadpleegt u de kolom **Ondersteuning voor voor voor touch geoptimaliseerde interface** in de tabel in het gedeelte **Ondersteunde browsers voor ontwerpen van gebruikersinterface** van [Technische vereisten](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Koppelingen {#links}

* [Productpagina Adobe Experience Manager op adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Merknaam van bedrijfsmiddelen — Documentatie](https://helpx.adobe.com/nl/experience-manager/brand-portal/user-guide.html)

## Toegang tot en ondersteuning voor producten (beperkt aantal sites) {#product-access-and-support-restricted-sites}

Deze sites zijn alleen beschikbaar voor klanten. Neem contact op met uw accountmanager van Adobe als u een klant bent en toegang nodig hebt.

* [https://daycare.day.com](https://daycare.day.com)

* [Producttoegang](https://login.marketing.adobe.com)

* [Adobe Klantenservice](https://helpx.adobe.com/contact.html)
