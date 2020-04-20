---
title: Release-opmerkingen
seo-title: Release-opmerkingen
description: Lees meer over de functies, verbeteringen, kritieke problemen die zijn opgelost en bekende problemen in de release van Adobe Experience Manager Assets Brand Portal 6.4.6.
seo-description: Bekijk de verbeteringen, kritieke problemen die zijn opgelost en bekende problemen in de release van Adobe Experience Manager Assets Brand Portal 6.4.6.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 9bb1538165030f7f9e78af99bb89ea38897c3967

---


# Release-opmerkingen {#release-notes}

Bekijk de nieuwe functies, verbeteringen, kritieke problemen die zijn opgelost en bekende problemen in de release van Adobe Experience Manager Assets Brand Portal 6.4.6.

## Geen informatie {#release-information}

| Product | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versie | 6.4.6 |
| Date | maart 2020 |

## Overzicht {#overview}

Met de Adobe Experience Manager (AEM) Assets Brand Portal kunt u eenvoudig goedgekeurde creatieve middelen aanschaffen, beheren en veilig distribueren aan externe partijen en interne zakelijke gebruikers op verschillende apparaten. Het draagt bij tot een efficiëntere verdeling van activa, versnelt de marktintroductie van activa en vermindert het risico van niet-naleving en ongeoorloofde toegang. Merkportal biedt gebruikers de mogelijkheid om in door het bedrijf goedgekeurde indelingen te zoeken, te bekijken, voor te vertonen, te downloaden en te exporteren, altijd en overal.

## Nieuwe functies in 6.4.6 {#what-s-new-in-646}

### Nieuwe functies {#new-feature}

Deze release bevat de volgende nieuwe functies:

* Captcha voor gastaanmelding bij Brand Portal. Zie, de toegang [van de gast van het Portaal van het](../using/guest-access.md) Merk voor meer informatie.

* Brand Portal wordt nu ondersteund door de cloudservice van AEM Assets. U kunt AEM Assets vormen kon met het Portaal van het Merk dienst doen om activa met de gebruikers van het Portaal van het Merk te delen en te verspreiden.
Zie AEM Assets Cloud Service [configureren met Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html)voor meer informatie.

### Verbeteringen {#enhancements-646}

Deze release van Brand Portal bevat de volgende verbeteringen:

* In AEM 6.3 en hoger wordt het machtigingskanaal tussen AEM Assets en Brand Portal gewijzigd. AEM Assets is nu geconfigureerd met Brand Portal via Adobe I/O, dat een IMS token aanschaft voor toestemming van uw Pantaarn voor merken.

   >[!NOTE]
   >
   >Configuratie via verouderde OAuth wordt vanaf 6 april 2020 niet meer ondersteund en wordt gewijzigd in configureren via Adobe I/O.


>[!TIP]
>
>***Alleen voor bestaande klanten***
>
>Het wordt geadviseerd om bestaande oudere configuratie van de Gateway te blijven gebruiken OAuth. Als u problemen ondervindt met de oudere OAuth Gateway-configuratie, verwijdert u de bestaande configuratie en maakt u een nieuwe configuratie via Adobe I/O.


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

* Gebruikers van Brand Portal kunnen geen middelen uit de bijdragemap publiceren naar AEM Assets bij de upgrade naar Adobe I/O op AEM 6.5.4.

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

## Gecertificeerde platforms {#certified-platforms}

Als u wilt weten welke platforms zijn gecertificeerd voor uitvoering met deze versie van Brand Portal, raadpleegt u de kolom **Ondersteuning voor voor voor touch geoptimaliseerde interface** in de tabel in het gedeelte **Ondersteunde browsers voor ontwerpen van gebruikersinterface** van [Technische vereisten](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Koppelingen {#links}

* [Productpagina van Adobe Experience Manager op adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Merknaam van bedrijfsmiddelen — Documentatie](https://helpx.adobe.com/nl/experience-manager/brand-portal/user-guide.html)

## Toegang tot en ondersteuning voor producten (beperkt aantal sites) {#product-access-and-support-restricted-sites}

Deze sites zijn alleen beschikbaar voor klanten. Neem contact op met uw accountmanager van Adobe als u een klant bent en toegang nodig hebt.

* [https://daycare.day.com](https://daycare.day.com)

* [Producttoegang](https://login.marketing.adobe.com)

* [Adobe Klantenservice](https://helpx.adobe.com/contact.html)
