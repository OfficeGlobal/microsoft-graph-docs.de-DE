---
title: managedAppOperation-Ressourcentyp
description: Steht für einen Vorgang, der auf eine App-Registrierung angewendet wird.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 962468c4d1464b827e234b0aac5452bbd0be576a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859038"
---
# <a name="managedappoperation-resource-type"></a>managedAppOperation-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Steht für einen Vorgang, der auf eine App-Registrierung angewendet wird.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[managedAppOperations auflisten](../api/intune-mam-managedappoperation-list.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [managedAppOperation](../resources/intune-mam-managedappoperation.md)-Objekte.|
|[managedAppOperation abrufen](../api/intune-mam-managedappoperation-get.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|Lesen von Eigenschaften und Beziehungen des [managedAppOperation](../resources/intune-mam-managedappoperation.md)-Objekts.|
|[managedAppOperation erstellen](../api/intune-mam-managedappoperation-create.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|Erstellen eines neuen [managedAppOperation](../resources/intune-mam-managedappoperation.md)-Objekts.|
|[managedAppOperation löschen](../api/intune-mam-managedappoperation-delete.md)|Keine|Löscht ein [managedAppOperation](../resources/intune-mam-managedappoperation.md)-Objekt.|
|[managedAppOperation aktualisieren](../api/intune-mam-managedappoperation-update.md)|[managedAppOperation](../resources/intune-mam-managedappoperation.md)|Aktualisieren der Eigenschaften eines [managedAppOperation](../resources/intune-mam-managedappoperation.md)-Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|String|Name des Vorgangs|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des App-Vorgangs|
|state|String|Aktueller Status des Vorgangs|
|id|String|Schlüssel der Entität|
|Version|String|Version der Entität|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```





