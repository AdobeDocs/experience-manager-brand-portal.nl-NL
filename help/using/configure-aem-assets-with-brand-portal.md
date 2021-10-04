---
title: Experience Manager-elementen configureren met Brand Portal
seo-title: Configure Experience Manager Assets with Brand Portal
description: Meer informatie over het configureren van Experience Manager Assets met Brand Portal.
seo-description: Get an insight into configuring Experience Manager Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 2%

---

# Experience Manager-elementen configureren met Brand Portal {#configure-integration}

Als u Adobe Experience Manager Assets configureert met Brand Portal, kunt u functies voor het publiceren van bedrijfsmiddelen, het distribueren van bedrijfsmiddelen en het leveren van bedrijfsmiddelen voor Brand Portal-gebruikers inschakelen. Hiermee kunnen gebruikers van Experience Manager Assets elementen publiceren en distribueren met Brand Portal-gebruikers. De Brand Portal-gebruikers hebben toegang tot de gedeelde elementen en kunnen een bijdrage leveren door nieuwe elementen te uploaden naar de mappen voor de bijdrage van elementen en deze weer te publiceren naar Experience Manager Assets.

Het configureren van Experience Manager Assets met Brand Portal wordt ondersteund op:

* Elementen Experience Managers als Cloud Service
* Experience Manager Assets (on-premisse en beheerde service) 6.3 en hoger

Elementen als Cloud Service Experience Managers wordt automatisch geconfigureerd met Brand Portal door Brand Portal te activeren vanuit Cloud Manager. De activeringsworkflow maakt de vereiste configuraties op de achtergrond en activeert Brand Portal op dezelfde IMS org als de Experience Manager Assets als een Cloud Service-instantie.

Terwijl, de Middelen van de Experience Manager (op gebouw en beheerde dienst) manueel met Brand Portal gebruikend de Console van de Ontwikkelaar van Adobe wordt gevormd, die een teken van de Diensten van Adobe Identity Management (IMS) voor vergunning van de huurder van Brand Portal aanschaft.

>[!NOTE]
>
>***Voor Experience Manager Activa 6.3 en hoger***
>
>Eerder, werd Brand Portal gevormd in klassieke interface via de Gateway van Legacy OAuth, die het token van het Web JSON (JWT) gebruikt om een teken IMS voor vergunning te verkrijgen.
>
>Configuratie via verouderde OAuth wordt vanaf 6 april 2020 niet meer ondersteund en wordt gewijzigd in configuratie via Adobe Developer Console.


>[!TIP]
>
>***Alleen voor bestaande klanten (op locatie en beheerde service)***
>
>De verouderde configuratie van de Gateway OAuth zal blijven werkend voor bestaande klanten.
>
>Voor het geval u problemen met erfenisOAuth configuratie tegenkomt, schrap de bestaande configuratie en creeer nieuwe configuratie via de Console van de Ontwikkelaar van Adobe.

De stappen voor het configureren van AEM Assets met Brand Portal zijn afhankelijk van uw AEM en of u de configuratie voor het eerst configureert of de bestaande configuraties bijwerkt:

| **AEM** | **Nieuwe configuratie** | **Upgradeconfiguratie** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Brand Portal activeren](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 en hoger)** | [Configuratie maken](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgradeconfiguratie](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 en hoger)** | [Configuratie maken](https://experienceleague.adobe.com/docs/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Upgradeconfiguratie](https://experienceleague.adobe.com/docs/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 en hoger)** | [Configuratie maken](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Upgradeconfiguratie](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6,2** | Contact opnemen met ondersteuning | Contact opnemen met ondersteuning |
