---
title: Digitale rechten van middelen beheren
description: Het verlenen van vergunningen activa en het plaatsen van vervaldatum voor activa en gedeelde verbindingen verzekeren gecontroleerd gebruik van deze activa en beschermen hen.
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
role: Admin
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: 10f89ded6febb1a024cbe181fa48a290d90223f0
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# Digitale rechten van middelen beheren {#manage-digital-rights-of-assets}

Een veilige distributie en veilig gebruik van creatieve middelen en merkmateriaal is van essentieel belang om uw merk te beschermen. Dit proces kan worden afgedwongen door een vervaldatum (en -tijd) te koppelen aan goedgekeurde activa die van AEM naar Brand Portal zijn gepubliceerd, of door deze activa in licentie te geven voor voorwaardelijk gebruik. Bovendien kunt u met Brand Portal een vervaldatum opgeven voor koppelingen naar de elementen die door Brand Portal worden gedeeld.

Lees verder om te weten hoe de middelen op Brand Portal zijn beveiligd en de bijbehorende gebruiksrechten te begrijpen.

## Vervaldatum van element {#asset-expiration}

Vervaldatum van bedrijfsmiddelen is een effectieve manier om het gebruik van goedgekeurde bedrijfsmiddelen op Brand Portal binnen een organisatie te controleren. Alle van AEM Assets naar Brand Portal gepubliceerde activa kunnen een vervaldatum hebben, die het gebruik van deze activa door verschillende gebruikersrollen beperkt.

### Gebruiksmachtigingen met betrekking tot verlopen elementen {#usage-permissions-expired-assets}

In Brand Portal kunnen beheerders verlopen elementen weergeven, downloaden en toevoegen aan verzamelingen. Editors en Viewers kunnen echter alleen verlopen elementen weergeven en toevoegen aan verzamelingen.

Beheerders kunnen verlopen middelen van AEM Assets naar Brand Portal publiceren. Verlopen elementen kunnen echter niet worden gedeeld via een koppeling vanuit Brand Portal. Als u verlopen elementen selecteert in een map met verlopen en niet-verlopen elementen, is de handeling **[!UICONTROL Share Link]** niet beschikbaar. Maar als u een map selecteert die verlopen en niet-verlopen elementen bevat, zijn de acties [!UICONTROL Share] en **[!UICONTROL Share Link]** beschikbaar.

>[!NOTE]
>
>Een map kan nog steeds als een koppeling worden gedeeld, zelfs als deze verlopen elementen bevat. In dit geval vermeldt de koppeling geen verlopen elementen en worden alleen de niet-verlopen elementen gedeeld.

In de volgende tabel worden de gebruiksmachtigingen van verlopen elementen weergegeven:

|   | **[!UICONTROL Link share]** | **[!UICONTROL Download]** | **[!UICONTROL Properties]** | **[!UICONTROL Add to collection]** | **[!UICONTROL Delete]** |
|---|---|---|---|---|---|
| **[!UICONTROL Administrator]** | Niet beschikbaar | Beschikbaar | Beschikbaar | Beschikbaar | Beschikbaar |
| **[!UICONTROL Editor]** | Niet beschikbaar | Niet beschikbaar | Beschikbaar | Beschikbaar | Niet beschikbaar |
| **[!UICONTROL Viewer]** | Niet beschikbaar | Niet beschikbaar | Beschikbaar | Beschikbaar | Niet beschikbaar |
| **[!UICONTROL Guest user]** | Niet beschikbaar | Niet beschikbaar | Beschikbaar | Beschikbaar | Niet beschikbaar |

>[!NOTE]
>
>Als Viewers en Editors een map met verlopen en niet-verlopen elementen downloaden, worden alleen de niet-verlopen elementen gedownload. Als een map alleen verlopen elementen bevat, wordt een lege map gedownload.

### Vervalstatus van activa {#expiration-status-of-assets}

U kunt de vervalstatus van elementen weergeven in de **[!UICONTROL Card View]** ervan. Een rode markering op de kaart geeft aan dat het element is verlopen.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>In de lijst- en kolomweergaven wordt de vervalstatus van elementen niet weergegeven.

## Vervaldatum van asset-koppeling {#asset-link-expiration}

Tijdens het delen van elementen via koppelingen kunnen beheerders en editors een vervaldatum en -tijd instellen met het veld **[!UICONTROL Expiration]** in het dialoogvenster **[!UICONTROL Link Sharing]** . De standaardvervaldatum van een koppeling is zeven dagen vanaf de datum waarop de koppeling wordt gedeeld.

![](assets/asset-link-sharing.png)

Het zorgt ervoor dat elementen die als koppelingen worden gedeeld, verlopen op de datum en tijd die door Brand Portal-beheerders en -editors zijn ingesteld. En de elementen kunnen na de vervaldatum niet meer worden weergegeven en gedownload. Om uw goedgekeurde middelen tegen externe gebruikers te beschermen, plaatst een vervaldatum op gedeelde verbindingen om ervoor te zorgen zij niet aan onbekende entiteiten na een gespecificeerde tijd worden blootgesteld.

Voor meer informatie over verbinding het delen, verwijs naar [ activa van het Aandeel als verbinding ](../using/brand-portal-link-share.md).

## Gelicentieerde Assets {#licensed-assets}

Voor gelicentieerde activa moet een licentieovereenkomst worden geaccepteerd voordat ze van Brand Portal kunnen worden gedownload. Deze overeenkomst voor gelicentieerde activa komt wanneer u direct het middel van Brand Portal of door middel van een gedeelde verbinding downloadt. Alle gebruikers kunnen met een licentie beveiligde elementen weergeven, ongeacht of deze zijn verlopen of niet. Het downloaden en gebruiken van verlopen gelicentieerde middelen is echter beperkt. Om over het gedrag van verlopen in licentie gegeven activa en toelaatbare activiteiten te weten die op gebruikersrollen worden gebaseerd, verwijs naar [ gebruikstoestemmingen van verlopen activa ](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

De vergunning-beschermde activa hebben a [ vergunningsovereenkomst in bijlage ](https://experienceleague.adobe.com/nl/docs/experience-manager-65/content/assets/administer/drm) aan hen, die door het de meta-gegevensbezit van activa in [!DNL Experience Manager Assets] te plaatsen wordt gedaan.

Een element wordt als beveiligd beschouwd als het een van de volgende (of beide) metagegevenseigenschappen bevat:

* `xmpRights:WebStatement`: Deze eigenschap verwijst naar het pad van de pagina die de licentieovereenkomst voor het element bevat. `xmpRights:WebStatement` moet een geldig pad zijn in de opslagplaats.
* `adobe_dam:restrictions`: de waarde van deze eigenschap is een onbewerkte HTML die de licentieovereenkomst opgeeft.


Als u met een licentie beveiligde elementen wilt downloaden, wordt u naar de pagina **[!UICONTROL Copyright Management]** omgeleid, afhankelijk van de eigenschappen van de metagegevens.

| `adobe_dam:restrictions` | `xmpRights:WebStatement` | Copyrightbeheer |
| --- | --- | --- |
| Ja | - | De interface wordt weergegeven in zowel Assets als Brand Portal |
| - | Ja (ongeldig pad) | Geen interface |
| Ja | Ja (ongeldig pad) | Geen interface |
| Ja | Ja (geldig pad) | De interface verschijnt in Assets of Brand Portal </br> afhankelijk van of de weg voor Assets of Brand Portal (of allebei) geldig is. |

![](assets/asset-copyright-mgmt.png)

Hier moet u het element selecteren om de bijbehorende licentieovereenkomst te downloaden en te accepteren. Als u de licentieovereenkomst niet accepteert, wordt de knop **[!UICONTROL Download]** niet ingeschakeld.

![](assets/licensed-asset-download-2.png)

Als de selectie meerdere beveiligde elementen bevat, selecteert u één element tegelijk, accepteert u de licentieovereenkomst en gaat u verder met het downloaden van het element.

## Rapport genereren over verlopen elementen {#generate-report-about-expired-assets}

Beheerders kunnen een rapport genereren en downloaden waarin alle elementen worden vermeld die binnen een bepaalde tijd zijn verlopen. Dit rapport bevat gedetailleerde informatie— zoals grootte, type, pad die de locatie van de elementen in de hiërarchie van de elementen aangeeft, wanneer het actief verviel en wanneer het actief werd gepubliceerd— over de verlopen elementen. De kolommen van dit rapport kunnen worden aangepast om meer gegevens te tonen die op gebruikersvereisten worden gebaseerd.

![](assets/assets-expired.png)

Voor meer informatie over de rapporteigenschap, ga naar [ Werk met rapporten ](../using/brand-portal-reports.md#work-with-reports).
