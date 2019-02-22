---
title: managedAppStatusRaw-Ressourcentyp
description: Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34c70a268c3940843759844c27de7f31bfab002e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154194"
---
# <a name="managedappstatusraw-resource-type"></a>managedAppStatusRaw-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.


Erbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedAppStatusRaws auflisten](../api/intune-mam-managedappstatusraw-list.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Objekte.|
|[ManagedAppStatusRaw abrufen](../api/intune-mam-managedappstatusraw-get.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)|Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Anzeigename des Statusberichts. Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).|
|id|string|Schlüssel der Entität. Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).|
|version|Zeichenfolge|Version der Entität Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).|
|content|[Json](../resources/intune-mam-json.md)|Inhalt des Statusberichts.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```




