---
title: deviceEnrollmentConfiguration-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 8dd622f0a59f1364d91bb2c8f410d0bc1edd1188
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349133"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a>deviceEnrollmentConfiguration-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceEnrollmentConfigurations auflisten](../api/intune-onboarding-deviceenrollmentconfiguration-list.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Objekte.|
|[deviceEnrollmentConfiguration abrufen](../api/intune-onboarding-deviceenrollmentconfiguration-get.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Objekts.|
|[setPriority-Aktion](../api/intune-onboarding-deviceenrollmentconfiguration-setpriority.md)|Keine|Noch nicht dokumentiert.|
|[Aktion zuweisen](../api/intune-onboarding-deviceenrollmentconfiguration-assign.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Noch nicht dokumentiert|
|displayName|String|Noch nicht dokumentiert.|
|description|String|Noch nicht dokumentiert.|
|priority|Int32|Noch nicht dokumentiert.|
|createdDateTime|DateTimeOffset|Noch nicht dokumentiert.|
|lastModifiedDateTime|DateTimeOffset|Noch nicht dokumentiert.|
|version|Int32|Noch nicht dokumentiert.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)-Sammlung|Die Liste derGruppenzuweisungen für das Gerätekonfigurationsprofil.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```





