---
title: groupPolicyPresentationMultiTextBox-Ressourcentyp
description: Stellt ein ADMX-multiTextbox-Element und ein ADMX-multiText-Element dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 70656a4922227371c1f4aa795b851acd4a8f5de9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163847"
---
# <a name="grouppolicypresentationmultitextbox-resource-type"></a>groupPolicyPresentationMultiTextBox-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt ein ADMX-multiTextbox-Element und ein ADMX-multiText-Element dar.


Erbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[GroupPolicyPresentationMultiTextBoxes aufListen](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-list.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekte.|
|[GroupPolicyPresentationMultiTextBox abrufen](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-get.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Lesen von Eigenschaften und Beziehungen des [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekts.|
|[GroupPolicyPresentationMultiTextBox erstellen](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-create.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Erstellen eines neuen [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekts.|
|[GroupPolicyPresentationMultiTextBox löschen](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-delete.md)|Keine|Löscht eine [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md).|
|[GroupPolicyPresentationMultiTextBox aktualisieren](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-update.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|Aktualisieren der Eigenschaften eines [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|label|String|Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität. Der Standardwert ist Empty. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Entität. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|erforderlich|Boolescher Wert|Anforderung zur Eingabe eines Werts in das Textfeld. Der Standardwert ist "false".|
|maxLength|Int64|Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Textzeichen angibt. Der Standardwert ist 1023.|
|maxStrings|Int64|Eine ganze Zahl ohne Vorzeichen, die die maximale Anzahl von Zeichenfolgen angibt. Der Standardwert ist 0.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Die der Präsentation zugeordnete Gruppenrichtlinien Definition. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationMultiTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "required": true,
  "maxLength": 1024,
  "maxStrings": 1024
}
```




