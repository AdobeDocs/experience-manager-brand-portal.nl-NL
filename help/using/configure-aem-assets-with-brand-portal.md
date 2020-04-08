---
title: AEM-middelen configureren met Brand Portal
seo-title: AEM-middelen configureren met Brand Portal
description: Krijg inzicht in het configureren van AEM Assets met Brand Portal.
seo-description: Krijg inzicht in het configureren van AEM Assets met Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: dc10879caf91b81deda08682548143c60500fd1b

---


# AEM-middelen configureren met Brand Portal {#configure-integration}

Adobe Experience Manager-middelen (AEM) worden geconfigureerd met Brand Portal via Adobe I/O, dat een IMS-token aanschaft voor toestemming van uw Brand Portal-huurder. Brand Portal wordt nu ondersteund op AEM Assets Cloud Service, AEM Assets 6.3 en hoger.

Als u AEM-middelen configureert, kunt u deze gebruiken met het Brand Portal, zodat u elementen kunt publiceren en distribueren met de gebruikers van het Brand Portal. Terwijl het Vormen van het Portaal van het Merk op AEM 6.3 (en hierboven) activa het uitgeven, activadistributie en activa bijdrageeigenschappen voor de gebruikers van het Portaal van het Merk toelaat.

>[!NOTE]
>
>***Voor AEM-activa 6.3 en hoger***
>
>Eerder, werd het Portaal van het Merk gevormd in Klassieke UI via Verouderde Gateway OAuth, die de het symbolenuitwisseling van JWT gebruikt om een token van de Toegang te verkrijgen IMS voor vergunning.
>
>Configuratie via verouderde OAuth wordt vanaf 6 april 2020 niet meer ondersteund en wordt gewijzigd in configureren via Adobe I/O.


>[!TIP]
>
>***Alleen voor bestaande klanten***
>
>Het wordt geadviseerd om bestaande oudere configuratie van de Gateway te blijven gebruiken OAuth. Als er problemen optreden met de oudere OAuth Gateway-configuratie, verwijdert u de bestaande configuratie en maakt u een nieuwe configuratie via Adobe I/O.


De stappen om AEM Middelen met het Portaal van het Merk te vormen zijn verschillend afhankelijk van uw versie AEM, en of u voor het eerst vormt, of de bestaande configuraties bevordert:

| **AEM-versie** | **Nieuwe configuratie** | **Upgradeconfiguratie** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 en hoger)** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgradeconfiguratie](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 en hoger)** | [Configuratie maken](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgradeconfiguratie](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 en hoger)** | [Configuratie maken](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Upgradeconfiguratie](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contact opnemen met ondersteuning | Contact opnemen met ondersteuning |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
