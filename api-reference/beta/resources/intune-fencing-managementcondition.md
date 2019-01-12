---
title: Ressourcentyp managementCondition
description: Management Bedingungen sind Ereignisse, die dynamisch wie Geo-Klammern, ausgelöst werden, können Zeit Klammern und Netzwerk Klammern.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: e0aeb73a93cd4c61b6d4680f73c2a9b8cee830c6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986741"
---
# <a name="managementcondition-resource-type"></a>Ressourcentyp managementCondition

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Management Bedingungen sind Ereignisse, die dynamisch wie Geo-Klammern, ausgelöst werden, können Zeit Klammern und Netzwerk Klammern.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste managementConditions](../api/intune-fencing-managementcondition-list.md)|[ManagementCondition](../resources/intune-fencing-managementcondition.md) -Auflistung|Listeneigenschaften und Beziehungen der [ManagementCondition](../resources/intune-fencing-managementcondition.md) -Objekte.|
|[Abrufen von managementCondition](../api/intune-fencing-managementcondition-get.md)|[managementCondition](../resources/intune-fencing-managementcondition.md)|Lesen Sie Eigenschaften und Beziehungen des [ManagementCondition](../resources/intune-fencing-managementcondition.md) -Objekts.|
|[GetManagementConditionsForPlatform-Funktion](../api/intune-fencing-managementcondition-getmanagementconditionsforplatform.md)|[ManagementCondition](../resources/intune-fencing-managementcondition.md) -Auflistung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für die Bedingung Management. System generierten Wert, die beim Erstellen zugewiesen.|
|uniqueName|Zeichenfolge|Eindeutiger Name für die Bedingung Management. In Management Bedingung Ausdrücken verwendet.|
|displayName|Zeichenfolge|Der Administrator definierter Name der Bedingung Management.|
|description|Zeichenfolge|Der Administrator definiert die Beschreibung der Bedingung Management.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, an die Bedingung Management erstellt wurde. Generierte Service-Seite.|
|modifiedDateTime|DateTimeOffset|Die Zeit, die die Bedingung Management zuletzt geändert wurde. Aktualisierte Service-Seite.|
|eTag|Zeichenfolge|ETag der Bedingung Management. Aktualisierte Service-Seite.|
|applicablePlatforms|[DevicePlatformType](../resources/intune-shared-deviceplatformtype.md) -Auflistung|Die entsprechenden Plattformen für diese Bedingung Management.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|managementConditionStatements|[ManagementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) -Auflistung|Die Bedingung Management Anweisungen, die Bedingung Management zugeordnet ist.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





