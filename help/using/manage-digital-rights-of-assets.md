---
title: Digitale rechten van middelen beheren
seo-title: Digitale rechten van middelen beheren
description: Het verlenen van vergunningen activa en het plaatsen van vervaldatum voor activa en gedeelde verbindingen verzekeren gecontroleerd gebruik van deze activa en beschermen hen.
seo-description: Het verlenen van vergunningen activa en het plaatsen van vervaldatum voor activa en gedeelde verbindingen verzekeren gecontroleerd gebruik van deze activa en beschermen hen.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Digitale rechten van middelen beheren {#manage-digital-rights-of-assets}

Een veilige distributie en veilig gebruik van creatieve middelen en merkmateriaal is van essentieel belang om uw merk te beschermen. Dit kan binnen de organisatie en buiten de organisatie worden afgedwongen door een vervaldatum (en tijd) te koppelen aan goedgekeurde activa die van AEM aan Brand Portal zijn gepubliceerd, of door deze activa voor voorwaardelijk gebruik in licentie te geven. Ook, staat het Portaal van het Merk u toe om een vervaldatum voor verbindingen aan de activa te specificeren die van het Portaal van het Merk worden gedeeld.

Lees verder om te weten hoe de activa op het Portaal van het Merk worden beveiligd en de bijbehorende gebruikstoestemmingen begrijpen.

## Vervaldatum van element {#asset-expiration}

Vervaldatum van bedrijfsmiddelen is een effectieve manier om het gebruik van goedgekeurde bedrijfsmiddelen op Brand Portal in een organisatie te controleren. Alle activa die van activa AEM aan het Portaal van het Merk worden gepubliceerd kunnen een vervaldatum hebben, die het gebruik van deze activa door verschillende gebruikersrollen beperkt.

### Gebruiksmachtigingen met betrekking tot verlopen elementen {#usage-permissions-expired-assets}

In Brand Portal kunnen beheerders verlopen elementen weergeven, downloaden en toevoegen aan verzamelingen. Editors en Viewers kunnen echter alleen verlopen elementen weergeven en toevoegen aan verzamelingen.

Beheerders kunnen verlopen middelen van AEM Assets naar Brand Portal publiceren. Verlopen middelen kunnen echter niet via inkt worden gedeeld vanuit Brand Portal. Als u verlopen middelen selecteert uit een map met verlopen en niet-verlopen elementen, is de **[!UICONTROL Share Link]** actie niet beschikbaar. Maar als u een map selecteert die verlopen en niet-verlopen elementen bevat, zijn de [!UICONTROL Share] **[!UICONTROL Share Link]** acties en de acties beschikbaar.

>[!NOTE]
>
>Een map kan nog steeds als een koppeling worden gedeeld, zelfs als deze verlopen elementen bevat. In dit geval vermeldt de koppeling geen verlopen elementen en worden alleen de niet-verlopen elementen gedeeld.

In de volgende tabel worden de gebruiksmachtigingen van verlopen elementen weergegeven:

|  | **[!UICONTROL Link share]** | **[!UICONTROL Download]** | **[!UICONTROL Properties]** | **[!UICONTROL Add to collection]** | **[!UICONTROL Delete]** |
|---|---|---|---|---|---|
| **[!UICONTROL Administrator]** | Niet beschikbaar | Beschikbaar | Beschikbaar | Beschikbaar | Beschikbaar |
| **[!UICONTROL Editor]** | Niet beschikbaar | Niet beschikbaar | Beschikbaar | Beschikbaar | Niet beschikbaar |
| **[!UICONTROL Viewer]** | Niet beschikbaar | Niet beschikbaar | Beschikbaar | Beschikbaar | Niet beschikbaar |
| **[!UICONTROL Guest user]** | Niet beschikbaar | Niet beschikbaar | Beschikbaar | Beschikbaar | Niet beschikbaar |

>[!NOTE]
>
>Als Viewers en Editors een map met verlopen en niet-verlopen elementen downloaden, worden alleen de niet-verlopen elementen gedownload. Als een map alleen verlopen elementen bevat, wordt een lege map gedownload.

### Vervalstatus van activa {#expiration-status-of-assets}

U kunt de vervalstatus van elementen in hun **[!UICONTROL Card View]** lijst weergeven. Een rode markering op de kaart geeft aan dat het element is verlopen.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>In de lijst- en kolomweergaven wordt de vervalstatus van elementen niet weergegeven.

## Vervaldatum van middelenkoppeling {#asset-link-expiration}

Tijdens het delen van elementen via koppelingen kunnen beheerders en editors een vervaldatum en -tijd instellen met het **[!UICONTROL Expiration]** veld in het **[!UICONTROL Link Sharing]** dialoogvenster. De standaardvervaldatum van verbinding is zeven dagen vanaf de datum waarop de verbinding wordt gedeeld.

![](assets/asset-link-sharing.png)

Het zorgt ervoor dat de activa die als verbindingen worden gedeeld verlopen op de datum en de tijd die door de Beheerders en de Redacteurs van het Portaal van het Merk worden geplaatst, en kunnen niet meer na de vervaldatum worden bekeken en worden gedownload. Aangezien de elementen die via koppelingen worden gedeeld, ook kunnen worden bekeken door externe gebruikers die geen deel uitmaken van de organisatie, kunt u door het opgeven van de vervaldatum ervoor zorgen dat uw goedgekeurde elementen worden beveiligd en niet langer dan een bepaalde tijd aan onbekende entiteiten worden blootgesteld.

Zie Elementen [delen als een koppeling](../using/brand-portal-link-share.md)voor meer informatie over het delen van koppelingen.

## Gelicentieerde activa {#licensed-assets}

Voor gelicentieerde activa moet een licentieovereenkomst worden geaccepteerd voordat deze van Brand Portal kunnen worden gedownload. Deze overeenkomst voor gelicentieerde activa komt wanneer u het middel van Brand Portal of via een gedeelde verbinding direct downloadt. Alle gebruikers kunnen de door een licentie beveiligde middelen bekijken, ongeacht of deze zijn verlopen of niet. Het downloaden en gebruiken van verlopen gelicentieerde middelen is echter beperkt. Raadpleeg de [gebruiksmachtigingen van verlopen elementen](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)voor informatie over het gedrag van verlopen, in licentie gegeven elementen en toegestane activiteiten op basis van gebruikersrollen.

Bij voor licentie beveiligde elementen is een [licentieovereenkomst gekoppeld](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) , die wordt uitgevoerd door de eigenschap [](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) metadata van het element in te stellen in AEM Assets.

Als u met licentie beveiligde middelen wilt downloaden, wordt u omgeleid naar de **[!UICONTROL Copyright Management]** pagina.

![](assets/asset-copyright-mgmt.png)

Hier moet u het element selecteren om de bijbehorende licentieovereenkomst te downloaden en te accepteren. Als u de licentieovereenkomst niet accepteert, wordt de **[!UICONTROL Download]** knop niet ingeschakeld.

![](assets/licensed-asset-download-2.png)

Als de selectie meerdere beveiligde elementen bevat, selecteert u één element tegelijk, accepteert u de licentieovereenkomst en gaat u verder met het downloaden van het element.

## Rapport genereren over verlopen elementen {#generate-report-about-expired-assets}

Beheerders kunnen een rapport genereren en downloaden waarin alle elementen worden vermeld die binnen een bepaalde tijd zijn verlopen. Dit rapport bevat gedetailleerde informatie— zoals grootte, type, pad die de locatie van de elementen in de hiërarchie van de elementen aangeeft, wanneer het actief verviel en wanneer het actief werd gepubliceerd— over de verlopen elementen. De kolommen van dit rapport kunnen worden aangepast om meer gegevens te tonen die op gebruikersvereisten worden gebaseerd.

![](assets/assets-expired.png)

Raadpleeg [Werken met rapporten](../using/brand-portal-reports.md#work-with-reports)voor meer informatie over de functie Rapporten.
