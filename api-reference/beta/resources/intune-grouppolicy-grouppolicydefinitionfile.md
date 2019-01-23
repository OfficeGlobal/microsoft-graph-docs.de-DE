---
title: Ressourcentyp groupPolicyDefinitionFile
description: Die Entität stellt eine ADMX (ADM) XML-Datei. Die ADMX-Datei enthält eine Auflistung von Group Policy-Definitionen und deren Speicherorte nach Kategoriepfad. Die Gruppenrichtlinie-Definitionsdatei enthält auch die Sprachen unterstützt, wie durch die Sprachdateien abhängigen ADML (ADM) Sprache bestimmt.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac5206321047dd4cd54732103e4adb70221e860
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431531"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>Ressourcentyp groupPolicyDefinitionFile

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Die Entität stellt eine ADMX (ADM) XML-Datei. Die ADMX-Datei enthält eine Auflistung von Group Policy-Definitionen und deren Speicherorte nach Kategoriepfad. Die Gruppenrichtlinie-Definitionsdatei enthält auch die Sprachen unterstützt, wie durch die Sprachdateien abhängigen ADML (ADM) Sprache bestimmt.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Lesen Sie Eigenschaften und Beziehungen des [GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekts.|
|[GroupPolicyDefinitionFile aktualisieren](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Aktualisieren Sie die Eigenschaften eines [GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|displayName|Zeichenfolge|Die lokalisierten Anzeigenamen der ADMX-Datei.|
|description|Zeichenfolge|Die lokalisierte Beschreibung der Richtlinieneinstellungen in der ADMX-Datei. Der Standardwert ist leer.|
|languageCodes|Zeichenfolgenauflistung|Die unterstützten Sprachcodes für die ADMX-Datei.|
|targetPrefix|Zeichenfolge|Gibt den logischen Namen, der auf den Namespace innerhalb der ADMX-Datei verweist.|
|targetNamespace|Zeichenfolge|Gibt den URI verwendet, um den Namespace innerhalb der ADMX-Datei zu identifizieren.|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Gibt den Typ von Gruppenrichtlinien. Mögliche Werte sind: `admxBacked` und `admxIngested`.|
|id|Zeichenfolge|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung die Entität.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|Definitionen|[GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) -Auflistung|Der Gruppenrichtlinie Definitionen im Zusammenhang mit der Datei.|

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




