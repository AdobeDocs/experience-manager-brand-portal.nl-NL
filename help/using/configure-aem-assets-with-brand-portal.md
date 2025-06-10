---
title: Experience Manager Assets configureren met Brand Portal
description: Insight wordt nu in staat gesteld Experience Manager Assets met Brand Portal te configureren.
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: f4add370fd3242f5506e5cc4d921362e2b14141a
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 1%

---

# Experience Manager Assets configureren met Brand Portal {#configure-integration}

Als u Adobe Experience Manager Assets configureert met Brand Portal, kunt u functies voor het publiceren van bedrijfsmiddelen, het distribueren van bedrijfsmiddelen en het leveren van bedrijfsmiddelen inschakelen voor de Brand Portal-gebruikers. Hiermee kunnen Experience Manager Assets-gebruikers elementen publiceren en distribueren met Brand Portal-gebruikers. De Brand Portal-gebruikers hebben toegang tot de gedeelde elementen en kunnen een bijdrage leveren door nieuwe elementen te uploaden naar de mappen voor middelenbijdragen en deze weer te publiceren naar Experience Manager Assets.

Het configureren van Experience Manager Assets met Brand Portal wordt ondersteund op:

* Experience Manager Assets as a Cloud Service
* Experience Manager Assets (on-premisse en beheerde service) 6.5 en hoger

Experience Manager Assets as a Cloud Service wordt automatisch geconfigureerd met Brand Portal door Brand Portal vanuit de Cloud Manager te activeren. De activeringsworkflow maakt de vereiste configuraties op de achtergrond en activeert Brand Portal op dezelfde IMS org als de Experience Manager Assets as a Cloud Service-instantie.

Terwijl Experience Manager Assets (op gebouw en beheerde dienst) manueel met Brand Portal gebruikend Adobe Developer Console wordt gevormd, die een teken van de Diensten van Adobe Identity Management (IMS) voor vergunning van de huurder van Brand Portal koopt.

>[!NOTE]
>
>***voor Experience Manager Assets, 6.5 en hierboven***
>
>Eerder, vormde de klassieke interface Brand Portal gebruikend de Oudere Gateway OAuth, die de uitwisseling JSON Web Token (JWT) aanwendt om een teken IMS voor vergunning te verkrijgen.
>
>Configuratie via Legacy OAuth wordt vanaf 6 april 2020 niet meer ondersteund en wordt gewijzigd in configuratie via Adobe Developer Console.


>[!TIP]
>
>***voor bestaande klanten slechts (op gebouw en beheerde dienst)***
>
>De verouderde configuratie van de Gateway OAuth blijft werkend voor bestaande klanten.
>
>Voor het geval dat u problemen met de configuratie van de Gateway van de Legacy OAuth tegenkomt, schrap de bestaande configuratie en creeer een nieuwe configuratie door Adobe Developer Console.

De stappen voor het configureren van AEM Assets met Brand Portal zijn afhankelijk van uw AEM-versie en of u de configuratie voor het eerst configureert of de bestaande configuraties bijwerkt:

| **Versie van AEM** | **Nieuwe Configuratie** | **Configuratie van de Verbetering** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [ activeer Brand Portal ](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/brand-portal/configure-aem-assets-with-brand-portal) | - |
| **AEM 6.5 (6.5.4.0 en hierboven)** | [ creeer configuratie ](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal) | [ de configuratie van de Verbetering ](https://experienceleague.adobe.com/en/docs/experience-manager-65/content/assets/brandportal/configure-aem-assets-with-brand-portal#upgrade-integration-65) |
