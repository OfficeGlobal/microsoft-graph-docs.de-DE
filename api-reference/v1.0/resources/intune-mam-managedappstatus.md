---
title: managedAppStatus-Ressourcentyp
description: Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bc6982161e204a4f2e5cac38b62d351ab417482
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258863"
---
# <a name="managedappstatus-resource-type"></a>managedAppStatus-Ressourcentyp

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



