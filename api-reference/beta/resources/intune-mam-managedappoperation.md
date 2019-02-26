---
title: managedAppOperation-Ressourcentyp
description: Steht für einen Vorgang, der auf eine App-Registrierung angewendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fb8ad24a86822b657e4f0239f78ab8f08656ee4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162209"
---
# <a name="managedappoperation-resource-type"></a>managedAppOperation-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

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
|displayName|Zeichenfolge|Name des Vorgangs|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des App-Vorgangs|
|state|Zeichenfolge|Aktueller Status des Vorgangs|
|id|string|Schlüssel der Entität|
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




