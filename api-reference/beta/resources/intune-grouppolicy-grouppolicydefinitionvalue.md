---
title: groupPolicyDefinitionValue-Ressourcentyp
description: Die Definitionswert Entität speichert den Wert für eine einzelne Gruppenrichtlinien Definition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e822cb4ce46a0fa9492f7624904588fd1b10a7c3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142616"
---
# <a name="grouppolicydefinitionvalue-resource-type"></a>groupPolicyDefinitionValue-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Definitionswert Entität speichert den Wert für eine einzelne Gruppenrichtlinien Definition.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[GroupPolicyDefinitionValues aufListen](../api/intune-grouppolicy-grouppolicydefinitionvalue-list.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Objekte.|
|[GroupPolicyDefinitionValue abrufen](../api/intune-grouppolicy-grouppolicydefinitionvalue-get.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Lesen von Eigenschaften und Beziehungen des [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Objekts.|
|[GroupPolicyDefinitionValue erstellen](../api/intune-grouppolicy-grouppolicydefinitionvalue-create.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Erstellen eines neuen [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Objekts.|
|[GroupPolicyDefinitionValue löschen](../api/intune-grouppolicy-grouppolicydefinitionvalue-delete.md)|Keine|Löscht eine [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md).|
|[GroupPolicyDefinitionValue aktualisieren](../api/intune-grouppolicy-grouppolicydefinitionvalue-update.md)|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Aktualisieren der Eigenschaften eines [groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit der Erstellung des Objekts.|
|enabled|Boolean|Aktiviert oder deaktiviert die zugeordnete Gruppenrichtlinien Definition.|
|configurationType|[groupPolicyConfigurationType](../resources/intune-grouppolicy-grouppolicyconfigurationtype.md)|Gibt an, wie der Wert konfiguriert werden soll. Dabei kann es sich entweder um eine Richtlinie oder eine Präferenz handeln. Mögliche Werte sind: `policy` und `preference`.|
|id|Zeichenfolge|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Entität.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|presentationValues|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) -Sammlung|Die zugeordneten Gruppenrichtlinien-Präsentations Werte mit dem Definitionswert.|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Die zugeordnete Gruppenrichtlinien Definition mit dem Wert.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionValue",
  "createdDateTime": "String (timestamp)",
  "enabled": true,
  "configurationType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




