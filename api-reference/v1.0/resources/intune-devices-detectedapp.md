---
title: detectedApp-Ressourcentyp
description: Eine verwaltete oder nicht verwaltete App, die auf einem verwalteten Gerät installiert ist. Nicht verwaltete Apps werden nur für als unternehmenseigen gekennzeichnete Geräte angezeigt.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a9a31245676dfba465de61aca6527d112ce0b6d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252602"
---
# <a name="detectedapp-resource-type"></a>detectedApp-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|id|string|Eindeutiger Bezeichner für die erkannte Anwendung. Dieser wird automatisch von Intune generiert, wenn die Anwendung erstellt wird. Schreibgeschützt.|
|displayName|Zeichenfolge|Name der ermittelten Anwendung. Schreibgeschützt|
|version|String|Version der ermittelten Anwendung. Schreibgeschützt|
|sizeInByte|Int64|Größe der ermittelten Anwendung in Byte. Schreibgeschützt|
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



