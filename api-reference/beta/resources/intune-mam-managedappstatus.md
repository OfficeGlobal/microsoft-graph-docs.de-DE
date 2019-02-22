---
title: managedAppStatus-Ressourcentyp
description: Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cc9f6596e9d9361a8c211809bf0f621fe36bcd4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153158"
---
# <a name="managedappstatus-resource-type"></a>managedAppStatus-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedAppStatuses auflisten](../api/intune-mam-managedappstatus-list.md)|[managedAppStatus](../resources/intune-mam-managedappstatus.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedAppStatus](../resources/intune-mam-managedappstatus.md)-Objekte.|
|[managedAppStatus abrufen](../api/intune-mam-managedappstatus-get.md)|[managedAppStatus](../resources/intune-mam-managedappstatus.md)|Lesen von Eigenschaften und Beziehungen des [managedAppStatus](../resources/intune-mam-managedappstatus.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Anzeigename des Statusberichts|
|id|string|Schlüssel der Entität|
|Version|Zeichenfolge|Version der Entität|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```




