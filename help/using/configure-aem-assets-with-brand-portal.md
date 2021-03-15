---
title: AEM Assets configureren met Brand Portal
seo-title: AEM Assets configureren met Brand Portal
description: Bekijk de configuratie van AEM Assets met Brand Portal.
seo-description: Bekijk de configuratie van AEM Assets met Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: bfb0c38bf8d5b542caf9d0d20d3168cdcac649b3
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 8%

---


# AEM Assets configureren met Brand Portal {#configure-integration}

Als u Adobe Experience Manager Assets configureert met Brand Portal, kunt u functies voor het publiceren van bedrijfsmiddelen, het distribueren van bedrijfsmiddelen en het leveren van bedrijfsmiddelen gebruiken voor de gebruikers van het Brand Portal. Hiermee kunnen AEM Assets-gebruikers elementen publiceren en distribueren met de gebruikers van het Brand Portal. De gebruikers van het Brand Portal hebben toegang tot de gedeelde elementen en kunnen een bijdrage leveren door nieuwe elementen te uploaden naar de mappen voor middelenbijdragen en deze weer te publiceren naar AEM Assets.

Het configureren van AEM Assets met Brand Portal wordt ondersteund op:
* AEM Assets as a Cloud Service
* AEM Assets (ter plaatse en Managed Services) 6.3 en hoger

AEM Assets als Cloud Service wordt automatisch geconfigureerd met Brand Portal door Brand Portal te activeren vanuit Cloud Manager. De activeringsworkflow maakt de vereiste configuraties op de achtergrond en activeert Brand Portal op dezelfde IMS-org als de AEM Assets als een Cloud Service-instantie.

Terwijl AEM Assets (op-gebouw en Managed Services) manueel met het Portaal van het Merk gebruikend de Console van de Ontwikkelaar van Adobe wordt gevormd, die een teken van de Diensten van Adobe Identity Management (IMS) voor toestemming van de huurder van het Portaal van het Merk koopt.

>[!NOTE]
>
>***Voor AEM Assets 6.3 en hoger***
>
>Eerder, werd het Portaal van het Merk gevormd in klassieke interface via de Gateway van de Oudheid OAuth, die het token van JSON Web (JWT) gebruikt om een teken IMS voor vergunning te verkrijgen.
>
>Configuratie via verouderde OAuth wordt vanaf 6 april 2020 niet meer ondersteund en wordt gewijzigd in configuratie via Adobe Developer Console.


>[!TIP]
>
>***Alleen voor bestaande klanten (op locatie en Managed Services)***
>
>De verouderde configuratie van de Gateway OAuth zal blijven werkend voor bestaande klanten.
>
>Voor het geval u problemen met erfenisOAuth configuratie tegenkomt, schrap de bestaande configuratie en creeer nieuwe configuratie via de Console van de Ontwikkelaar van Adobe.

De stappen voor het configureren van AEM Assets met Brand Portal verschillen afhankelijk van uw AEM versie en of u voor het eerst configureert of de bestaande configuraties bijwerkt:

| **AEM** | **Nieuwe configuratie** | **Upgradeconfiguratie** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Merkportal activeren](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 en hoger)** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgradeconfiguratie](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 en hoger)** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgradeconfiguratie](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 en hoger)** | [Configuratie maken](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Upgradeconfiguratie](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6,2** | Contact opnemen met ondersteuning | Contact opnemen met ondersteuning |
