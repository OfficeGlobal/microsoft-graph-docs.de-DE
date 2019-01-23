---
title: Ressourcentyp intuneBrandingProfile
description: Diese Entität enthält Daten, die bei der Anpassung der Mandant Ebene das Unternehmensportal Applications als auch die Endbenutzer Webportal verwendet werden.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b299964627a89598c28f15dfeed8ce6e13bede8c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411099"
---
# <a name="intunebrandingprofile-resource-type"></a>Ressourcentyp intuneBrandingProfile

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Diese Entität enthält Daten, die bei der Anpassung der Mandant Ebene das Unternehmensportal Applications als auch die Endbenutzer Webportal verwendet werden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste intuneBrandingProfiles](../api/intune-wip-intunebrandingprofile-list.md)|[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Auflistung|Listeneigenschaften und Beziehungen der [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekte.|
|[Abrufen von intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Lesen Sie Eigenschaften und Beziehungen des [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.|
|[Erstellen von intuneBrandingProfile](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Erstellen eines neuen [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.|
|[IntuneBrandingProfile löschen](../api/intune-wip-intunebrandingprofile-delete.md)|Keine|Löscht eine [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).|
|[IntuneBrandingProfile aktualisieren](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Aktualisieren Sie die Eigenschaften eines [IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.|
|[assign-Aktion](../api/intune-wip-intunebrandingprofile-assign.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Profil-Taste|
|Profilname|Zeichenfolge|Name des Profils|
|profileDescription|Zeichenfolge|Beschreibung des Profils|
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
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[IntuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Auflistung|Die Liste der Gruppe Zuordnungen für das branding Profil.|

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




