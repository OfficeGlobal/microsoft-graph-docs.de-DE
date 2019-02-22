---
title: groupPolicyPresentationValueText-Ressourcentyp
description: Die Entität stellt einen Zeichenfolgenwert für eine Dropdownliste, ein Kombinationsfeld oder eine Text Feld Präsentation für eine Richtliniendefinition dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9af7b417f64787d0a9d4977f404d3e3ad97fc543
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171652"
---
# <a name="grouppolicypresentationvaluetext-resource-type"></a>groupPolicyPresentationValueText-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Die Entität stellt einen Zeichenfolgenwert für eine Dropdownliste, ein Kombinationsfeld oder eine Text Feld Präsentation für eine Richtliniendefinition dar.


Erbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[GroupPolicyPresentationValueTexts aufListen](../api/intune-grouppolicy-grouppolicypresentationvaluetext-list.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) -Objekte.|
|[GroupPolicyPresentationValueText abrufen](../api/intune-grouppolicy-grouppolicypresentationvaluetext-get.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|Lesen von Eigenschaften und Beziehungen des [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) -Objekts.|
|[GroupPolicyPresentationValueText erstellen](../api/intune-grouppolicy-grouppolicypresentationvaluetext-create.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|Erstellen eines neuen [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) -Objekts.|
|[GroupPolicyPresentationValueText löschen](../api/intune-grouppolicy-grouppolicypresentationvaluetext-delete.md)|Keine|Löscht eine [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md).|
|[GroupPolicyPresentationValueText aktualisieren](../api/intune-grouppolicy-grouppolicypresentationvaluetext-update.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|Aktualisieren der Eigenschaften eines [groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung des Objekts. Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|createdDateTime|DateTimeOffset|Das Datum und die Uhrzeit der Erstellung des Objekts. Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|id|String|Schlüssel der Entität Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|Wert|Zeichenfolge|Ein String-Wert für die zugeordnete Präsentation.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|Definitions|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|Der Wert der Gruppenrichtlinien Definition, der dem Präsentations Wert zugeordnet ist. Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|Präsentation|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|Die dem Präsentations Wert zugeordnete Gruppenrichtlinien Präsentation. Geerbt von [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": "String"
}
```




