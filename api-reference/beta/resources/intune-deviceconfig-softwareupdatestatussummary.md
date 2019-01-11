---
title: softwareUpdateStatusSummary-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 79022d0f47f08d27a9b3d517267d0a32534916a8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854586"
---
# <a name="softwareupdatestatussummary-resource-type"></a>softwareUpdateStatusSummary-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[SoftwareUpdateStatusSummary abrufen](../api/intune-deviceconfig-softwareupdatestatussummary-get.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Lesen von Beziehungen und Eigenschaften des [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)-Objekts.|
|[SoftwareUpdateStatusSummary aktualisieren](../api/intune-deviceconfig-softwareupdatestatussummary-update.md)|[softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)|Aktualisieren der Eigenschaften eines [softwareUpdateStatusSummary](../resources/intune-deviceconfig-softwareupdatestatussummary.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
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





