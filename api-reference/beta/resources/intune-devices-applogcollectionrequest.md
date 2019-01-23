---
title: Ressourcentyp appLogCollectionRequest
description: AppLogCollectionRequest-Entität.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 795b80b0194f2c3a1d314cbb317af954fb675063
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431528"
---
# <a name="applogcollectionrequest-resource-type"></a>Ressourcentyp appLogCollectionRequest

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

AppLogCollectionRequest-Entität.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Liste appLogCollectionRequests](../api/intune-devices-applogcollectionrequest-list.md)|[AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Auflistung|Listeneigenschaften und Beziehungen der [AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekte.|
|[Abrufen von appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Lesen Sie Eigenschaften und Beziehungen des [AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekts.|
|[Erstellen von appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-create.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Erstellen eines neuen [AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekts.|
|[AppLogCollectionRequest löschen](../api/intune-devices-applogcollectionrequest-delete.md)|Keine|Löscht eine [AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).|
|[AppLogCollectionRequest aktualisieren](../api/intune-devices-applogcollectionrequest-update.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Aktualisieren Sie die Eigenschaften eines [AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) -Objekts.|
|[CreateDownloadUrl Aktion](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md)|Noch nicht dokumentiert|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|Zeichenfolge|Der eindeutige Bezeichner. Dies ist die Id der UserId_DeviceId_AppId.|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|Melden Sie sich Upload-Status. Mögliche Werte sind: `pending`, `completed` und `failed`.|
|errorMessage|Zeichenfolge|Fehlermeldung gegebenenfalls beim Hochladen|
|customLogFolders|Zeichenfolgenauflistung|Liste der Protokollordner. |
|completedDateTime|DateTimeOffset|Zeit an, die die Upload Protokoll Anforderung einen Endzustand erreicht|

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




