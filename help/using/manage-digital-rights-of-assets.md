---
title: Digitale rechten van middelen beheren
seo-title: Manage digital rights of assets
description: Het verlenen van vergunningen activa en het plaatsen van vervaldatum voor activa en gedeelde verbindingen verzekeren gecontroleerd gebruik van deze activa en beschermen hen.
seo-description: Licensing assets and setting expiration for assets and shared links ensure controlled usage of these assets and safeguard them.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
role: Admin
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: d1487434b10b01eaf55f34672267490fd8fd907e
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 0%

---

# Digitale rechten van middelen beheren {#manage-digital-rights-of-assets}

Een veilige distributie en veilig gebruik van creatieve middelen en merkmateriaal is van essentieel belang om uw merk te beschermen. Dit kan binnen de organisatie en buiten de organisatie worden afgedwongen door een vervaldatum (en tijd) te koppelen aan goedgekeurde middelen die van AEM naar Brand Portal zijn gepubliceerd, of door deze activa voor voorwaardelijk gebruik in licentie te geven. Bovendien kunt u met Brand Portal een vervaldatum opgeven voor koppelingen naar de elementen die door Brand Portal worden gedeeld.

Lees verder om te weten hoe de middelen op Brand Portal zijn beveiligd en de bijbehorende gebruiksrechten te begrijpen.

## Vervaldatum van element {#asset-expiration}

Vervaldatum van bedrijfsmiddelen is een effectieve manier om het gebruik van goedgekeurde bedrijfsmiddelen op Brand Portal binnen een organisatie te controleren. Alle van AEM Assets naar Brand Portal gepubliceerde activa kunnen een vervaldatum hebben, die het gebruik van deze activa door verschillende gebruikersrollen beperkt.

### Gebruiksmachtigingen met betrekking tot verlopen elementen {#usage-permissions-expired-assets}

In Brand Portal kunnen beheerders verlopen elementen weergeven, downloaden en toevoegen aan verzamelingen. Editors en Viewers kunnen echter alleen verlopen elementen weergeven en toevoegen aan verzamelingen.

Beheerders kunnen verlopen middelen van AEM Assets naar Brand Portal publiceren. Verlopen elementen kunnen echter niet via inkt van Brand Portal worden gedeeld. Als u verlopen elementen selecteert in een map met verlopen en niet-verlopen elementen, is de handeling **[!UICONTROL Share Link]** niet beschikbaar. Maar als u een map selecteert die verlopen en niet-verlopen elementen bevat, zijn de acties [!UICONTROL Share] en **[!UICONTROL Share Link]** beschikbaar.

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

Tijdens het delen van elementen via koppelingen kunnen beheerders en editors een vervaldatum en -tijd instellen met het veld **[!UICONTROL Expiration]** in het dialoogvenster **[!UICONTROL Link Sharing]** . De standaardvervaldatum van verbinding is zeven dagen vanaf de datum waarop de verbinding wordt gedeeld.

![](assets/asset-link-sharing.png)

Het zorgt ervoor dat elementen die als koppelingen worden gedeeld, verlopen op de datum en tijd die door Brand Portal-beheerders en -editors zijn ingesteld, en dat ze niet langer na de vervaldatum kunnen worden weergegeven en gedownload. Aangezien de elementen die via koppelingen worden gedeeld, ook kunnen worden bekeken door externe gebruikers die geen deel uitmaken van de organisatie, kunt u door het opgeven van de vervaldatum ervoor zorgen dat uw goedgekeurde elementen worden beveiligd en niet langer dan een bepaalde tijd aan onbekende entiteiten worden blootgesteld.

Voor meer informatie over verbinding het delen, verwijs naar [ activa van het Aandeel als verbinding ](../using/brand-portal-link-share.md).

## Gelicentieerde Assets {#licensed-assets}

Voor gelicentieerde activa moet een licentieovereenkomst worden geaccepteerd voordat ze van Brand Portal kunnen worden gedownload. Deze overeenkomst voor gelicentieerde activa komt wanneer u direct het middel van Brand Portal of via een gedeelde verbinding downloadt. Alle gebruikers kunnen de door een licentie beveiligde middelen bekijken, ongeacht of deze zijn verlopen of niet. Het downloaden en gebruiken van verlopen gelicentieerde middelen is echter beperkt. Om over het gedrag van verlopen in licentie gegeven activa en toelaatbare activiteiten te weten die op gebruikersrollen worden gebaseerd, verwijs naar [ gebruikstoestemmingen van verlopen activa ](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

De vergunning-beschermde activa hebben [ vergunningsovereenkomst in bijlage ](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/drm.html) aan hen, die door het de meta-gegevensbezit van activa in [!DNL Experience Manager Assets] te plaatsen wordt gedaan.

Een element wordt als beveiligd beschouwd als het een van de volgende (of beide) metagegevenseigenschappen bevat:

* `xmpRights:WebStatement`: Deze eigenschap verwijst naar het pad van de pagina die de licentieovereenkomst voor het element bevat. `xmpRights:WebStatement` moet een geldig pad zijn in de opslagplaats.
* `adobe_dam:restrictions`: de waarde van deze eigenschap is een onbewerkte HTML die de licentieovereenkomst opgeeft.


Als u met licentie beveiligde elementen wilt downloaden, wordt u naar de pagina **[!UICONTROL Copyright Management]** omgeleid, afhankelijk van de eigenschappen van de metagegevens.

| `adobe_dam:restrictions` | `xmpRights:WebStatement` | Copyrightbeheer |
| --- | --- | --- |
| Ja | - | De interface wordt weergegeven in zowel Assets als Brand Portal |
| - | Ja (ongeldig pad) | Geen interface |
| Ja | Ja (ongeldig pad) | Geen interface |
| Ja | Ja (geldig pad) | De interface wordt weergegeven in Assets of Brand Portal </br> Afhankelijk van of het pad geldig is voor Assets of Brand Portal (of beide). |

![](assets/asset-copyright-mgmt.png)

Hier moet u het element selecteren om de bijbehorende licentieovereenkomst te downloaden en te accepteren. Als u de licentieovereenkomst niet accepteert, wordt de knop **[!UICONTROL Download]** niet ingeschakeld.

![](assets/licensed-asset-download-2.png)

Als de selectie meerdere beveiligde elementen bevat, selecteert u één element tegelijk, accepteert u de licentieovereenkomst en gaat u verder met het downloaden van het element.

## Rapport genereren over verlopen elementen {#generate-report-about-expired-assets}

Beheerders kunnen een rapport genereren en downloaden waarin alle elementen worden vermeld die binnen een bepaalde tijd zijn verlopen. Dit rapport bevat gedetailleerde informatie— zoals grootte, type, pad die de locatie van de elementen in de hiërarchie van de elementen aangeeft, wanneer het actief verviel en wanneer het actief werd gepubliceerd— over de verlopen elementen. De kolommen van dit rapport kunnen worden aangepast om meer gegevens te tonen die op gebruikersvereisten worden gebaseerd.

![](assets/assets-expired.png)

Voor meer informatie over de rapporteigenschap, verwijs [ Werk met rapporten ](../using/brand-portal-reports.md#work-with-reports).
