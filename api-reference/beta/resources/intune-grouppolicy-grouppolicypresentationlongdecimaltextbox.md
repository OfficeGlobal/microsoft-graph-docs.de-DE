---
title: groupPolicyPresentationLongDecimalTextBox-Ressourcentyp
description: Stellt ein ADMX-longDecimalTextBox-Element und ein ADMX-longDecimal-Element dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09fbefc6bf261895976096f91000570f5fc539ca
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164694"
---
# <a name="grouppolicypresentationlongdecimaltextbox-resource-type"></a>groupPolicyPresentationLongDecimalTextBox-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt ein ADMX-longDecimalTextBox-Element und ein ADMX-longDecimal-Element dar.


Erbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[GroupPolicyPresentationLongDecimalTextBoxes aufListen](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-list.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) -Objekte.|
|[GroupPolicyPresentationLongDecimalTextBox abrufen](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-get.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Lesen von Eigenschaften und Beziehungen des [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) -Objekts.|
|[GroupPolicyPresentationLongDecimalTextBox erstellen](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-create.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Erstellen eines neuen [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) -Objekts.|
|[GroupPolicyPresentationLongDecimalTextBox löschen](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-delete.md)|Keine|Löscht eine [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md).|
|[GroupPolicyPresentationLongDecimalTextBox aktualisieren](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-update.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|Aktualisieren der Eigenschaften eines [groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|label|String|Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität. Der Standardwert ist Empty. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Entität. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|Int64|Eine ganze Zahl ohne Vorzeichen, die den Anfangswert für das Dezimal Textfeld angibt. Der Standardwert ist 1.|
|Spin|Boolescher Wert|Wenn true, erstellen Sie ein Drehfeld-Steuerelement; Erstellen Sie andernfalls ein Textfeld für die numerische Eingabe. Der Standardwert ist true.|
|spinStep|Int64|Eine ganze Zahl ohne Vorzeichen, die die Schrittweite der Änderung für das Drehfeld-Steuerelement angibt. Der Standardwert ist 1.|
|erforderlich|Boolescher Wert|Anforderung zur Eingabe eines Werts im Parameterfeld. Der Standardwert ist false.|
|minValue|Int64|Eine unsigned long, die den minimal zulässigen Wert angibt. Der Standardwert ist 0.|
|maxValue|Int64|Eine unsigned long, die den maximal zulässigen Wert angibt. Der Standardwert ist 9999.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Die der Präsentation zugeordnete Gruppenrichtlinien Definition. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationLongDecimalTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": 1024,
  "spin": true,
  "spinStep": 1024,
  "required": true,
  "minValue": 1024,
  "maxValue": 1024
}
```




