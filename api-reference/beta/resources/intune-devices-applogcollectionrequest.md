---
title: appLogCollectionRequest-Ressourcentyp
description: AppLogCollectionRequest-Entität.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed0512340431be0456ebbbc5a3bffbb2713fda89
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151702"
---
# <a name="applogcollectionrequest-resource-type"></a>appLogCollectionRequest-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

AppLogCollectionRequest-Entität.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[AppLogCollectionRequests aufListen](../api/intune-devices-applogcollectionrequest-list.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Sammlung|AufListen von Eigenschaften und Beziehungen der [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekte.|
|[AppLogCollectionRequest abrufen](../api/intune-devices-applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Lesen von Eigenschaften und Beziehungen des [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekts.|
|[AppLogCollectionRequest erstellen](../api/intune-devices-applogcollectionrequest-create.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Erstellen eines neuen [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekts.|
|[AppLogCollectionRequest löschen](../api/intune-devices-applogcollectionrequest-delete.md)|Keine|Löscht eine [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).|
|[AppLogCollectionRequest aktualisieren](../api/intune-devices-applogcollectionrequest-update.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Aktualisieren der Eigenschaften eines [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekts.|
|[createDownloadUrl-Aktion](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md)|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Der eindeutige Bezeichner. Dies ist userId_DeviceId_AppId-ID.|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|Protokoll Uploadstatus. Mögliche Werte sind: `pending`, `completed` und `failed`.|
|errorMessage|Zeichenfolge|Fehlermeldung, falls vorhanden, während des Uploads|
|customLogFolders|String collection|Liste der Protokollordner. |
|completedDateTime|DateTimeOffset|Zeitpunkt, zu dem die Upload-Protokollanforderung einen Terminalstatus erreicht hat|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "String (identifier)",
  "status": "String",
  "errorMessage": "String",
  "customLogFolders": [
    "String"
  ],
  "completedDateTime": "String (timestamp)"
}
```




