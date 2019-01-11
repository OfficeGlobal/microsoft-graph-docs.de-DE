---
title: Ressourcentyp intuneBrandingProfile
description: Diese Entität enthält Daten, die bei der Anpassung der Mandant Ebene das Unternehmensportal Applications als auch die Endbenutzer Webportal verwendet werden.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2ee2fee902b4aca542810dc058b7d16aaedb9c6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820608"
---
# <a name="intunebrandingprofile-resource-type"></a>Ressourcentyp intuneBrandingProfile

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Diese Entität enthält Daten, die bei der Anpassung der Mandant Ebene das Unternehmensportal Applications als auch die Endbenutzer Webportal verwendet werden.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste intuneBrandingProfiles](../api/intune-wip-intunebrandingprofile-list.md)|[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Auflistung|Listeneigenschaften und Beziehungen der [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekte.|
|[Abrufen von intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Lesen Sie Eigenschaften und Beziehungen des [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.|
|[Erstellen von intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Erstellen eines neuen [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.|
|[IntuneBrandingProfile löschen](../api/intune-wip-intunebrandingprofile-delete.md)|Keine|Löscht eine [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).|
|[IntuneBrandingProfile aktualisieren](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Aktualisieren Sie die Eigenschaften eines [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Profil-Taste|
|Profilname|String|Name des Profils|
|profileDescription|String|Beschreibung des Profils|
|isDefaultProfile|Boolean|Zeigt an, wenn das Profil für standardmäßig verwendet wird.|
|createdDateTime|DateTimeOffset|Wenn die BrandingProfile erstellt wurde.|
|lastModifiedDateTime|DateTimeOffset|Wann die BrandingProfile zuletzt geändert wurde.|
|displayName|String|Unternehmensname/Organisationsname, der Endbenutzern angezeigt wird|
|contactITName|String|Name der für den IT-Support zuständigen Person/Organisation|
|contactITPhoneNumber|String|Telefonnummer der für den IT-Support zuständigen Person/Organisation|
|contactITEmailAddress|String|E-Mail-Adresse der für den IT-Support zuständigen Person/Organisation|
|contactITNotes|String|Textkommentare zu der für den IT-Support zuständigen Person/Organisation|
|privacyUrl|String|URL zur Datenschutzrichtlinie des Unternehmens/der Organisation|
|onlineSupportSiteUrl|String|URL zur IT-Helpdesk-Website des Unternehmens/der Organisation|
|onlineSupportSiteName|String|Anzeigename der IT-Helpdesk-Website des Unternehmens/der Organisation|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Primäres Farbdesign für die Unternehmensportal-Anwendungen und das Webportal|
|showLogo|Boolean|Boolescher Wert, der angibt, ob die vom Administrator bereitgestellten Logobilder angezeigt werden sollen|
|showDisplayNameNextToLogo|Boolean|Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Logo-Bilds im Unternehmensportal apps auf Design farbigen Hintergrund angezeigt.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Logo-Bilds im Unternehmensportal apps heller Hintergrund angezeigt.|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Angepasste Bild im Unternehmensportal apps Zielseite|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrandingProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "String (identifier)",
  "profileName": "String",
  "profileDescription": "String",
  "isDefaultProfile": true,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```





