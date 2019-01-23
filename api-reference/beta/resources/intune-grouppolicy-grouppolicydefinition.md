---
title: Ressourcentyp groupPolicyDefinition
description: Die Entität beschreibt alle Informationen über eine einzelne Gruppenrichtlinie.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 502312f7a39dd5dc93fd8e39203f56d47a9ebf27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430167"
---
# <a name="grouppolicydefinition-resource-type"></a>Ressourcentyp groupPolicyDefinition

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Die Entität beschreibt alle Informationen über eine einzelne Gruppenrichtlinie.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Lesen Sie Eigenschaften und Beziehungen des [GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekts.|
|[GroupPolicyDefinition aktualisieren](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Aktualisieren Sie die Eigenschaften eines [GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Identifiziert den Typ von Gruppen, denen auf die Richtlinie angewendet werden kann. Mögliche Werte sind: `user`, `machine` und `both`.|
|displayName|Zeichenfolge|Die lokalisierten Richtliniennamen.|
|explainText|Zeichenfolge|Die lokalisierten Erläuterung oder Hilfe Text mit der Richtlinie verknüpft ist. Der Standardwert ist leer.|
|categoryPath|Zeichenfolge|Der Pfad der lokalisierte vollständige Kategorie für die Richtlinie ein.|
|supportedOn|Zeichenfolge|Lokalisierte Zeichenfolge verwendet, um anzugeben, welche Version der Anwendung oder das Betriebssystem durch die Richtlinie betroffen ist.|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Gibt den Typ von Gruppenrichtlinien. Mögliche Werte sind: `admxBacked` und `admxIngested`.|
|id|Zeichenfolge|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung die Entität.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|­DefinitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Die Gruppe Richtliniendatei für die Definition zugeordnet.|
|Präsentationen|[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Auflistung|Die Gruppenrichtlinie Präsentationen mit der Definition von verknüpft ist.|

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




