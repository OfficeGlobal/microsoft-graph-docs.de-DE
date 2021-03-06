---
title: groupPolicyDefinition-Ressourcentyp
description: Die Entität beschreibt alle Informationen zu einer einzelnen Gruppenrichtlinie.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c5062fda984dbe1dda518e77ff271750d30adb8
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644286"
---
# <a name="grouppolicydefinition-resource-type"></a>groupPolicyDefinition-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Entität beschreibt alle Informationen zu einer einzelnen Gruppenrichtlinie.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[GroupPolicyDefinition abrufen](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Lesen von Eigenschaften und Beziehungen des [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekts.|
|[GroupPolicyDefinition aktualisieren](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Aktualisieren der Eigenschaften eines [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Gibt den Typ der Gruppen an, auf die die Richtlinie angewendet werden kann. Mögliche Werte sind: `user` und `machine`.|
|displayName|Zeichenfolge|Der Name der lokalisierten Richtlinie.|
|explainText|Zeichenfolge|Die lokalisierte Erläuterung oder der Hilfe Text, der der Richtlinie zugeordnet ist. Der Standardwert ist leer.|
|categoryPath|Zeichenfolge|Der lokalisierte vollständige Kategorie-Pfad für die Richtlinie.|
|supportedOn|Zeichenfolge|Lokalisierte Zeichenfolge, die verwendet wird, um anzugeben, welche Betriebssystem-oder Anwendungsversion von der Richtlinie betroffen ist.|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Gibt den Typ der Gruppenrichtlinie an. Mögliche Werte: `admxBacked`, `admxIngested`.|
|id|String|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Entität.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Die der Definition zugeordnete Gruppenrichtliniendatei.|
|Präsentationen|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Sammlung|Die der Definition zugeordneten Gruppenrichtlinien Präsentationen.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




