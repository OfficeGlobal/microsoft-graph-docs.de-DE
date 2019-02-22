---
title: groupPolicyDefinitionFile-Ressourcentyp
description: Die Entität stellt eine ADMX-XML-Datei (administrative Vorlage) dar. Die ADMX-Datei enthält eine Sammlung von Gruppenrichtlinien Definitionen und ihre Standorte nach Kategorie-Pfad. Die Gruppenrichtlinien-Definitionsdatei enthält auch die unterstützten Sprachen, die von den sprachabhängigen Sprachdateien der ADML (administrative Template) bestimmt werden.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 494a2f8ff80b3a7f8ee9db9fea4d795494c19a92
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161334"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>groupPolicyDefinitionFile-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Entität stellt eine ADMX-XML-Datei (administrative Vorlage) dar. Die ADMX-Datei enthält eine Sammlung von Gruppenrichtlinien Definitionen und ihre Standorte nach Kategorie-Pfad. Die Gruppenrichtlinien-Definitionsdatei enthält auch die unterstützten Sprachen, die von den sprachabhängigen Sprachdateien der ADML (administrative Template) bestimmt werden.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[GroupPolicyDefinitionFile abrufen](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Lesen von Eigenschaften und Beziehungen des [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekts.|
|[GroupPolicyDefinitionFile aktualisieren](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Aktualisieren der Eigenschaften eines [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Der lokalisierte Anzeigename der ADMX-Datei.|
|description|Zeichenfolge|Die lokalisierte Beschreibung der Richtlinieneinstellungen in der ADMX-Datei. Der Standardwert ist Empty.|
|languageCodes|String collection|Die unterstützten Sprachcodes für die ADMX-Datei.|
|targetPrefix|Zeichenfolge|Gibt den logischen Namen an, der auf den Namespace innerhalb der ADMX-Datei verweist.|
|targetNamespace|Zeichenfolge|Gibt den URI an, der zum Identifizieren des Namespaces innerhalb der ADMX-Datei verwendet wird.|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Gibt den Typ der Gruppenrichtlinie an. Mögliche Werte sind: `admxBacked` und `admxIngested`.|
|id|Zeichenfolge|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Entität.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|Definitionen|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Sammlung|Die der Datei zugeordneten Gruppenrichtlinien Definitionen.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




