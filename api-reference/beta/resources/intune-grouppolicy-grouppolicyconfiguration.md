---
title: groupPolicyConfiguration-Ressourcentyp
description: Die Gruppenrichtlinien-Konfigurationsentität enthält die konfigurierten Werte für eine oder mehrere Gruppenrichtlinien Definitionen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 540da94d92f3056a6699b7112f3589f6da4b7144
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160753"
---
# <a name="grouppolicyconfiguration-resource-type"></a>groupPolicyConfiguration-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Gruppenrichtlinien-Konfigurationsentität enthält die konfigurierten Werte für eine oder mehrere Gruppenrichtlinien Definitionen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[GroupPolicyConfigurations aufListen](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekte.|
|[GroupPolicyConfiguration abrufen](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.|
|[GroupPolicyConfiguration erstellen](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Erstellen eines neuen [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.|
|[GroupPolicyConfiguration löschen](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|Keine|Löscht eine [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).|
|[GroupPolicyConfiguration aktualisieren](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Aktualisieren der Eigenschaften eines [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.|
|[assign-Aktion](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit der Erstellung des Objekts.|
|displayName|Zeichenfolge|Vom Benutzer bereitgestellter Name für das Resource-Objekt.|
|description|Zeichenfolge|Vom Benutzer bereitgestellte Beschreibung für das Resource-Objekt.|
|id|Zeichenfolge|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Entität.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|definitionValues|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Sammlung|Die Liste der aktivierten oder deaktivierten Gruppenrichtlinien definitionswerte für die Konfiguration.|
|assignments|[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Sammlung|Die Liste der Gruppenzuweisungen für die Konfiguration.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




