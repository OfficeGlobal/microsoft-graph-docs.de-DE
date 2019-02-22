---
title: groupPolicyPresentationListBox-Ressourcentyp
description: Stellt ein ADMX-listBox-Element und ein ADMX-Listenelement dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ca35283c20008264d7c2922ad137a7ba2c1c4f6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170917"
---
# <a name="grouppolicypresentationlistbox-resource-type"></a>groupPolicyPresentationListBox-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Stellt ein ADMX-listBox-Element und ein ADMX-Listenelement dar.


Erbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[GroupPolicyPresentationListBoxes aufListen](../api/intune-grouppolicy-grouppolicypresentationlistbox-list.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekte.|
|[GroupPolicyPresentationListBox abrufen](../api/intune-grouppolicy-grouppolicypresentationlistbox-get.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Lesen von Eigenschaften und Beziehungen des [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekts.|
|[GroupPolicyPresentationListBox erstellen](../api/intune-grouppolicy-grouppolicypresentationlistbox-create.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Erstellen eines neuen [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekts.|
|[GroupPolicyPresentationListBox löschen](../api/intune-grouppolicy-grouppolicypresentationlistbox-delete.md)|Keine|Löscht eine [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md).|
|[GroupPolicyPresentationListBox aktualisieren](../api/intune-grouppolicy-grouppolicypresentationlistbox-update.md)|[groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md)|Aktualisieren der Eigenschaften eines [groupPolicyPresentationListBox](../resources/intune-grouppolicy-grouppolicypresentationlistbox.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|label|String|Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität. Der Standardwert ist Empty. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Zeichenfolge|Schlüssel der Entität Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung der Entität. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|explicitValue|Boolescher Wert|Wenn diese Option auf true festgelegt ist, muss der Benutzer den Registrierungsunterschlüssel-Wert und den Registrierungsunterschlüssel Namen angeben. Das Listenfeld enthält zwei Spalten, eine für den Namen und einen für die Daten. Der Standardwert ist false.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Die der Präsentation zugeordnete Gruppenrichtlinien Definition. Geerbt von [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationListBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationListBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "explicitValue": true
}
```




