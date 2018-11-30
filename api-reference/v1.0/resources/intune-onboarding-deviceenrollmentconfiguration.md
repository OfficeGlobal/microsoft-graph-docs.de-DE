---
title: deviceEnrollmentConfiguration-Ressourcentyp
description: Noch nicht dokumentiert
ms.openlocfilehash: a748419edcecaeeafae96828048cf74929cb3f94
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019859"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a>deviceEnrollmentConfiguration-Ressourcentyp

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



