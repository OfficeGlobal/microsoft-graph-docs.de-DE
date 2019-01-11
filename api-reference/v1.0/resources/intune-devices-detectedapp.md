---
title: detectedApp-Ressourcentyp
description: Eine verwaltete oder nicht verwaltete App, die auf einem verwalteten Gerät installiert ist. Nicht verwaltete Apps werden nur für als unternehmenseigen gekennzeichnete Geräte angezeigt.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8b28965cb506075c8caf7d983ddf41eafcdda78d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27881424"
---
# <a name="detectedapp-resource-type"></a>detectedApp-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Eine verwaltete oder nicht verwaltete App, die auf einem verwalteten Gerät installiert ist. Nicht verwaltete Apps werden nur für als unternehmenseigen gekennzeichnete Geräte angezeigt.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[detectedApps auflisten](../api/intune-devices-detectedapp-list.md)|[detectedApp](../resources/intune-devices-detectedapp.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [detectedApp](../resources/intune-devices-detectedapp.md)-Objekte.|
|[detectedApp abrufen](../api/intune-devices-detectedapp-get.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|Auflisten von Eigenschaften und Beziehungen des [detectedApp](../resources/intune-devices-detectedapp.md)-Objekts.|
|[detectedApp erstellen](../api/intune-devices-detectedapp-create.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|Erstellen eines neuen [detectedApp](../resources/intune-devices-detectedapp.md)-Objekts.|
|[detectedApp löschen](../api/intune-devices-detectedapp-delete.md)|Keine|Löscht ein [detectedApp](../resources/intune-devices-detectedapp.md)-Objekt.|
|[detectedApp aktualisieren](../api/intune-devices-detectedapp-update.md)|[detectedApp](../resources/intune-devices-detectedapp.md)|Aktualisieren der Eigenschaften eines [detectedApp](../resources/intune-devices-detectedapp.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für die erkannte Anwendung. Dieser wird automatisch von Intune generiert, wenn die Anwendung erstellt wird. Schreibgeschützt.|
|displayName|String|Name der ermittelten Anwendung. Schreibgeschützt.|
|version|String|Version der ermittelten Anwendung. Schreibgeschützt.|
|sizeInByte|Int64|Größe der ermittelten Anwendung in Byte. Schreibgeschützt.|
|deviceCount|Int32|Die Anzahl von Geräten, auf denen diese Anwendung installiert ist.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managedDevices|[managedDevice](../resources/intune-devices-manageddevice.md)-Sammlung|Die Geräte, auf denen die ermittelte Anwendung installiert ist.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.detectedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "String (identifier)",
  "displayName": "String",
  "version": "String",
  "sizeInByte": 1024,
  "deviceCount": 1024
}
```



