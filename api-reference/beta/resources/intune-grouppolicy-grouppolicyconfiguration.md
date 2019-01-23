---
title: Ressourcentyp groupPolicyConfiguration
description: Die Gruppenrichtlinie Konfigurationsentität enthält die konfigurierten Werte für eine oder mehrere Group Policy-Definitionen.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be3b43ab0e9e3f87f53ed0dae144f2b6f4dce7b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431575"
---
# <a name="grouppolicyconfiguration-resource-type"></a>Ressourcentyp groupPolicyConfiguration

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

Die Gruppenrichtlinie Konfigurationsentität enthält die konfigurierten Werte für eine oder mehrere Group Policy-Definitionen.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste groupPolicyConfigurations](../api/intune-grouppolicy-grouppolicyconfiguration-list.md)|[GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Auflistung|Listeneigenschaften und Beziehungen der [GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekte.|
|[Abrufen von groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-get.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Lesen Sie Eigenschaften und Beziehungen des [GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.|
|[Erstellen von groupPolicyConfiguration](../api/intune-grouppolicy-grouppolicyconfiguration-create.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Erstellen eines neuen [GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.|
|[GroupPolicyConfiguration löschen](../api/intune-grouppolicy-grouppolicyconfiguration-delete.md)|Keine|Löscht eine [GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md).|
|[GroupPolicyConfiguration aktualisieren](../api/intune-grouppolicy-grouppolicyconfiguration-update.md)|[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)|Aktualisieren Sie die Eigenschaften eines [GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) -Objekts.|
|[assign-Aktion](../api/intune-grouppolicy-grouppolicyconfiguration-assign.md)|[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Auflistung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Das Datum und die Zeit, die das Objekt erstellt wurde.|
|displayName|Zeichenfolge|Der vom Benutzer bereitgestellte Name für das Resource-Objekt.|
|description|Zeichenfolge|Vom Benutzer bereitgestellte Beschreibung für das Resource-Objekt.|
|id|Zeichenfolge|Schlüssel der Entität|
|lastModifiedDateTime|DateTimeOffset|Datum und Uhrzeit der letzten Änderung die Entität.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|definitionValues|[GroupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md) -Auflistung|Die Liste der aktiviert oder deaktiviert Group Policy Definition Werte für die Konfiguration.|
|assignments|[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) -Auflistung|Die Liste der Gruppe Aufgaben für die Konfiguration.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




