---
title: AEM Assets configureren met Brand Portal
seo-title: AEM Assets configureren met Brand Portal
description: Krijg inzicht in het vormen van AEM Assets met het Portaal van het Merk.
seo-description: Krijg inzicht in het vormen van AEM Assets met het Portaal van het Merk.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: ba8a1f09573766643f6a5013a8d181f0f0dbb4f2
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 9%

---


# AEM Assets configureren met Brand Portal {#configure-integration}

Adobe Experience Manager-elementen (AEM) worden geconfigureerd met het Brand Portal via de Adobe Developer Console, die een IMS-token aanschaft voor goedkeuring door uw Pandhouder. Brand Portal wordt nu ondersteund op AEM Assets-cloudservice, AEM Assets 6.3 en hoger.

Het vormen AEM Assets kon met het Portaal van het Merk dienst doen staat u toe om activa met de gebruikers van het Portaal van het Merk te publiceren en te verspreiden. Terwijl het Vormen van het Portaal van het Merk op AEM 6.3 (en hierboven) activa het uitgeven, activadistributie en activa bijdrageeigenschappen voor de gebruikers van het Portaal van het Merk toelaat.

>[!NOTE]
>
>***Voor de AEM Assets 6.3 en hoger***
>
>Eerder, werd het Portaal van het Merk gevormd in Klassieke UI via Verouderde Gateway OAuth, die de het symbolenuitwisseling van JWT gebruikt om een token van de Toegang te verkrijgen IMS voor vergunning.
>
>Configuratie via verouderde OAuth wordt vanaf 6 april 2020 niet meer ondersteund en wordt gewijzigd in configuratie via Adobe Developer Console.


>[!TIP]
>
>***Alleen voor bestaande klanten***
>
>De verouderde configuratie van de Gateway OAuth zal blijven werkend voor bestaande klanten.
>
>Als u problemen ondervindt met de oudere configuratie van OAuth Gateway, verwijdert u de bestaande configuratie en maakt u een nieuwe configuratie via de Adobe Developer Console.


De stappen om AEM Assets met het Portaal van het Merk te vormen zijn verschillend afhankelijk van uw versie AEM, en of u voor het eerst vormt, of de bestaande configuraties bevordert:

| **AEM-versie** | **Nieuwe configuratie** | **Upgradeconfiguratie** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 en hoger)** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgradeconfiguratie](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 en hoger)** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgradeconfiguratie](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 en hoger)** | [Configuratie maken](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Upgradeconfiguratie](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contact opnemen met ondersteuning | Contact opnemen met ondersteuning |


