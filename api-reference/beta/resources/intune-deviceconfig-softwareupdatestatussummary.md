---
title: softwareUpdateStatusSummary-Ressourcentyp
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 382f771650c5c55f6ff38ae089a532a7603cf8e5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403518"
---
# <a name="softwareupdatestatussummary-resource-type"></a>softwareUpdateStatusSummary-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Noch nicht dokumentiert.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[SoftwareUpdateStatusSummary abrufen](../api/intune-deviceconfig-softwareupdatestatussummary-get.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Lesen von Beziehungen und Eigenschaften des [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)-Objekts.|
|[SoftwareUpdateStatusSummary aktualisieren](../api/intune-deviceconfig-softwareupdatestatussummary-update.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Aktualisieren der Eigenschaften eines [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Schlüssel der Entität|
|displayName|String|Der Name der Richtlinie|
|compliantDeviceCount|Int32|Anzahl der konformen Geräte|
|nonCompliantDeviceCount|Int32|Anzahl der nicht konformen Geräte|
|remediatedDeviceCount|Int32|Anzahl korrigierter Geräte|
|errorDeviceCount|Int32|Anzahl der Geräte mit Fehler|
|unknownDeviceCount|Int32|Anzahl unbekannter Geräte|
|conflictDeviceCount|Int32|Anzahl der Geräte mit Konflikten|
|notApplicableDeviceCount|Int32|Anzahl nicht anwendbarer Geräte|
|compliantUserCount|Int32|Anzahl der kompatiblen Benutzer|
|nonCompliantUserCount|Int32|Anzahl der nicht kompatiblen Benutzer|
|remediatedUserCount|Int32|Anzahl der korrigierten Benutzer|
|errorUserCount|Int32|Anzahl der Benutzer, bei denen ein Fehler aufgetreten ist.|
|unknownUserCount|Int32|Anzahl der unbekannten Benutzer|
|conflictUserCount|Int32|Anzahl der Benutzer mit Konflikt|
|notApplicableUserCount|Int32|Anzahl der nicht anwendbaren Benutzer.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```




