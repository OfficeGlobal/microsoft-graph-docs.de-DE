---
title: intuneBrandingProfile-Ressourcentyp
description: Diese Entität enthält Daten, die beim Anpassen der Darstellung der Mandantenebene der Unternehmensportal Anwendungen sowie des Webportals für Endbenutzer verwendet werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f21cc97cd701f9826743475c4055aed6bafe9ca
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144702"
---
# <a name="intunebrandingprofile-resource-type"></a>intuneBrandingProfile-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Diese Entität enthält Daten, die beim Anpassen der Darstellung der Mandantenebene der Unternehmensportal Anwendungen sowie des Webportals für Endbenutzer verwendet werden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[IntuneBrandingProfiles aufListen](../api/intune-wip-intunebrandingprofile-list.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekte.|
|[IntuneBrandingProfile abrufen](../api/intune-wip-intunebrandingprofile-get.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Lesen von Eigenschaften und Beziehungen des [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.|
|[IntuneBrandingProfile erstellen](../api/intune-wip-intunebrandingprofile-create.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Erstellen eines neuen [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.|
|[IntuneBrandingProfile löschen](../api/intune-wip-intunebrandingprofile-delete.md)|Keine|Löscht eine [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).|
|[IntuneBrandingProfile aktualisieren](../api/intune-wip-intunebrandingprofile-update.md)|[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)|Aktualisieren der Eigenschaften eines [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) -Objekts.|
|[assign-Aktion](../api/intune-wip-intunebrandingprofile-assign.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Profilschlüssel|
|Profilname|Zeichenfolge|Name des Profils|
|profileDescription|Zeichenfolge|Beschreibung des Profils|
|isDefaultProfile|Boolescher Wert|Zeigt an, ob das Profil standardmäßig verwendet wird.|
|createdDateTime|DateTimeOffset|Bei der Erstellung des BrandingProfile.|
|lastModifiedDateTime|DateTimeOffset|Wenn die BrandingProfile zuletzt geändert wurde.|
|displayName|Zeichenfolge|Unternehmensname/Organisationsname, der Endbenutzern angezeigt wird|
|contactITName|Zeichenfolge|Name der für den IT-Support zuständigen Person/Organisation|
|contactITPhoneNumber|Zeichenfolge|Telefonnummer der für den IT-Support zuständigen Person/Organisation|
|contactITEmailAddress|Zeichenfolge|E-Mail-Adresse der für den IT-Support zuständigen Person/Organisation|
|contactITNotes|Zeichenfolge|Textkommentare zu der für den IT-Support zuständigen Person/Organisation|
|privacyUrl|Zeichenfolge|URL zur Datenschutzrichtlinie des Unternehmens/der Organisation|
|onlineSupportSiteUrl|Zeichenfolge|URL zur IT-Helpdesk-Website des Unternehmens/der Organisation|
|onlineSupportSiteName|String|Anzeigename der IT-Helpdesk-Website des Unternehmens/der Organisation|
|themeColor|[rgbColor](../resources/intune-shared-rgbcolor.md)|Primäres Farbdesign für die Unternehmensportal-Anwendungen und das Webportal|
|showLogo|Boolescher Wert|Boolescher Wert, der angibt, ob die vom Administrator bereitgestellten Logobilder angezeigt werden sollen|
|showDisplayNameNextToLogo|Boolean|Boolescher Wert, der angibt, ob der vom Administrator angegebene Anzeigename neben dem Logobild angezeigt werden soll|
|themeColorLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Logobild, das in Unternehmens Portal-apps auf Design Farbhintergründen angezeigt wird.|
|lightBackgroundLogo|[mimeContent](../resources/intune-shared-mimecontent.md)|Logobild, das in Unternehmens Portal-apps auf hellen Hintergründen angezeigt wird.|
|landingPageCustomizedImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Angepasstes Bild, das auf der Startseite der Unternehmens Portal-apps angezeigt wird|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) -Sammlung|Die Liste der Gruppenzuweisungen für das Branding-Profil.|

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




