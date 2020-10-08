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
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 9%

---


# AEM Assets configureren met Brand Portal {#configure-integration}

Als u Adobe Experience Manager Assets configureert als Cloud Service met Adobe Experience Manager Assets Brand Portal, kunt u elementen publiceren en distribueren met de gebruikers van het Brand Portal. Terwijl het Vormen van AEM 6.3 (en hoger) met het Portaal van het Merk activa het publiceren, de distributie van activa, en de eigenschappen van de activabijdrage voor de gebruikers van het Portaal van het Merk toelaat.

Adobe Experience Manager Assets wordt geconfigureerd met Brand Portal via Adobe Developer Console, die een Adobe Identity Management Services (IMS)-token aanschaft voor toestemming van uw Brand Portal-huurder.

>[!NOTE]
>
>***Voor AEM Assets 6.3 en hoger***
>
>Eerder, werd het Portaal van het Merk gevormd in klassieke interface via de Gateway van de Oudheid OAuth, die het token van JSON Web (JWT) gebruikt om een teken IMS voor vergunning te verkrijgen.
>
>Configuratie via verouderde OAuth wordt vanaf 6 april 2020 niet meer ondersteund en wordt gewijzigd in configuratie via Adobe Developer Console.

>[!TIP]
>
>***Alleen voor bestaande klanten***
>
>De verouderde configuratie van de Gateway OAuth zal blijven werkend voor bestaande klanten.
>
>Voor het geval u problemen met erfenisOAuth configuratie tegenkomt, schrap de bestaande configuratie en creeer nieuwe configuratie via de Console van de Ontwikkelaar van Adobe.

De stappen voor het configureren van AEM Assets met Brand Portal verschillen afhankelijk van uw AEM versie en of u voor het eerst configureert of de bestaande configuraties bijwerkt:

| **AEM** | **Nieuwe configuratie** | **Upgradeconfiguratie** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 en hoger)** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgradeconfiguratie](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 en hoger)** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgradeconfiguratie](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 en hoger)** | [Configuratie maken](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Upgradeconfiguratie](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6,2** | Contact opnemen met ondersteuning | Contact opnemen met ondersteuning |
