---
title: embeddedSIMActivationCodePool-Ressourcentyp
description: Ein Pool stellt eine Gruppe von eingebetteten SIM-Aktivierungscodes dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 55cd515bf57dedf4cac2826000d7bc8e9764e3dd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158982"
---
# <a name="embeddedsimactivationcodepool-resource-type"></a>embeddedSIMActivationCodePool-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Ein Pool stellt eine Gruppe von eingebetteten SIM-Aktivierungscodes dar.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[EmbeddedSIMActivationCodePools aufListen](../api/intune-esim-embeddedsimactivationcodepool-list.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekte.|
|[EmbeddedSIMActivationCodePool abrufen](../api/intune-esim-embeddedsimactivationcodepool-get.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Lesen von Eigenschaften und Beziehungen des [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts.|
|[EmbeddedSIMActivationCodePool erstellen](../api/intune-esim-embeddedsimactivationcodepool-create.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Erstellen eines neuen [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts.|
|[EmbeddedSIMActivationCodePool löschen](../api/intune-esim-embeddedsimactivationcodepool-delete.md)|Keine|Löscht eine [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).|
|[EmbeddedSIMActivationCodePool aktualisieren](../api/intune-esim-embeddedsimactivationcodepool-update.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Aktualisieren der Eigenschaften eines [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts.|
|[assign-Aktion](../api/intune-esim-embeddedsimactivationcodepool-assign.md)|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Sammlung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Eindeutiger Bezeichner für den eingebetteten SIM-Aktivierungscode Pool. Vom System generierter Wert, der bei der Erstellung zugewiesen wird.|
|displayName|Zeichenfolge|Der vom Administrator definierte Name des eingebetteten SIM-Aktivierungscode Pools.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, zu dem der eingebettete SIM-Aktivierungscode Pool erstellt wurde. Generierte Dienstseite.|
|modifiedDateTime|DateTimeOffset|Zeitpunkt, zu dem der eingebettete SIM-Aktivierungscode Pool zuletzt geändert wurde. Aktualisierte Dienstseite.|
|activationCodes|[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) -Sammlung|Die Aktivierungscodes, die zu diesem Pool gehören. Diese Navigationseigenschaft wird verwendet, um Aktivierungscodes in InTune bereitzustellen, kann jedoch nicht zum Lesen von Aktivierungscodes aus InTune verwendet werden.|
|activationCodeCount|Int32|Die Gesamtanzahl der Aktivierungscodes, die zu diesem Pool gehören.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Sammlung|Navigationseigenschaft zu einer Liste der Ziele, denen dieser Pool zugeordnet ist.|
|deviceStates|[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Sammlung|Navigationseigenschaft zu einer Liste von Gerätestatus für diesen Pool.|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.embeddedSIMActivationCodePool"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "String",
      "matchingIdentifier": "String",
      "smdpPlusServerAddress": "String"
    }
  ],
  "activationCodeCount": 1024
}
```




