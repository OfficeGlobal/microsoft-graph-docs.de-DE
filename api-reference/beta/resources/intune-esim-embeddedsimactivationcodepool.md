---
title: Ressourcentyp embeddedSIMActivationCodePool
description: Ein Pool stellt eine Gruppe von eingebetteten SIM Aktivierungscodes.
ms.openlocfilehash: f6c80d82d4be6a794547e3ec0b93d4206d7edbe8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064468"
---
# <a name="embeddedsimactivationcodepool-resource-type"></a>Ressourcentyp embeddedSIMActivationCodePool

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Ein Pool stellt eine Gruppe von eingebetteten SIM Aktivierungscodes.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste embeddedSIMActivationCodePools](../api/intune-esim-embeddedsimactivationcodepool-list.md)|[EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Auflistung|Listeneigenschaften und Beziehungen der [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekte.|
|[Abrufen von embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-get.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Lesen Sie Eigenschaften und Beziehungen des [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts.|
|[Erstellen von embeddedSIMActivationCodePool](../api/intune-esim-embeddedsimactivationcodepool-create.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Erstellen eines neuen [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts.|
|[EmbeddedSIMActivationCodePool löschen](../api/intune-esim-embeddedsimactivationcodepool-delete.md)|Keines|Löscht eine [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).|
|[EmbeddedSIMActivationCodePool aktualisieren](../api/intune-esim-embeddedsimactivationcodepool-update.md)|[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)|Aktualisieren Sie die Eigenschaften eines [EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) -Objekts.|
|[assign-Aktion](../api/intune-esim-embeddedsimactivationcodepool-assign.md)|[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Auflistung|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Eindeutiger Bezeichner für den eingebetteten SIM Aktivierung Code Pool. System generierten Wert, die beim Erstellen zugewiesen.|
|displayName|String|Der Administrator definierten Namen des eingebetteten SIM Aktivierung Code Pools.|
|createdDateTime|DateTimeOffset|Der Zeitpunkt, zu der eingebettete SIM Aktivierung Code Pool erstellt wurde. Generierte Service-Seite.|
|modifiedDateTime|DateTimeOffset|Der Zeitpunkt der letzten Änderung der eingebettete SIM Aktivierung Code Pool. Aktualisierte Service-Seite.|
|activationCodes|[EmbeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) -Auflistung|Die Aktivierungscodes in diesem Pool angehören. Diese Navigationseigenschaft wird verwendet, um die Aktivierungscodes Intune buchen aber kann nicht zum Lesen von Aktivierungscodes aus Intune verwendet werden.|
|activationCodeCount|Int32|Die Gesamtzahl der Aktivierungscodes in diesem Pool angehören.|

## <a name="relationships"></a>Beziehungen
|Beziehung|Typ|Beschreibung|
|:---|:---|:---|
|assignments|[EmbeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) -Auflistung|Navigation-Eigenschaft, um eine Liste von Zielen, die dieser Pool zugeordnet ist.|
|deviceStates|[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) -Auflistung|Navigations-Eigenschaft, um eine Liste der Gerätestatus für diesen Pool.|

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




