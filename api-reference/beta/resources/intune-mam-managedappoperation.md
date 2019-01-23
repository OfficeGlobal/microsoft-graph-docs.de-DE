---
title: managedAppOperation-Ressourcentyp
description: Steht für einen Vorgang, der auf eine App-Registrierung angewendet wird.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cb72c4bf8cf7f2a4a55790087c3d46746c46a84a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424658"
---
# <a name="managedappoperation-resource-type"></a>managedAppOperation-Ressourcentyp

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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
|id|Zeichenfolge|Schlüssel der Entität|
|Version|Zeichenfolge|Version der Entität|

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




