---
title: deviceEnrollmentConfiguration-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc515f291e2ab32b744756063869ca3ca0c86cb5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259577"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a>deviceEnrollmentConfiguration-Ressourcentyp

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Noch nicht dokumentiert

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[deviceEnrollmentConfigurations auflisten](../api/intune-onboarding-deviceenrollmentconfiguration-list.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Sammlung|Auflisten von Eigenschaften und Beziehungen der [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Objekte.|
|[deviceEnrollmentConfiguration abrufen](../api/intune-onboarding-deviceenrollmentconfiguration-get.md)|[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)|Lesen von Eigenschaften und Beziehungen des [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)-Objekts.|
|[setPriority-Aktion](../api/intune-onboarding-deviceenrollmentconfiguration-setpriority.md)|Keine|Noch nicht dokumentiert|
|[Aktion zuweisen](../api/intune-onboarding-deviceenrollmentconfiguration-assign.md)|Keine|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Noch nicht dokumentiert|
|displayName|Zeichenfolge|Noch nicht dokumentiert|
|description|Zeichenfolge|Noch nicht dokumentiert|
|priority|Int32|Noch nicht dokumentiert|
|createdDateTime|DateTimeOffset|Noch nicht dokumentiert|
|lastModifiedDateTime|DateTimeOffset|Noch nicht dokumentiert.|
|version|Int32|Noch nicht dokumentiert|

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



