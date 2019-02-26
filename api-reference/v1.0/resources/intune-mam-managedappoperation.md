---
title: managedAppOperation-Ressourcentyp
description: Steht für einen Vorgang, der auf eine App-Registrierung angewendet wird.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe7416c5357b83bd9dc7eb82d94aae6a6d740667
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253470"
---
# <a name="managedappoperation-resource-type"></a>managedAppOperation-Ressourcentyp

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



