---
title: appLogCollectionDownloadDetails-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3449e1f1a2b8651cea407690019d458d5ac24fa9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147754"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a>appLogCollectionDownloadDetails-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Noch nicht dokumentiert

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|downloadUrl|Zeichenfolge|Download der SAS-URL für completed AppLogUploadRequest|
|decryptionKey|Zeichenfolge|DecryptionKey als Zeichenfolge|
|appLogDecryptionAlgorithm|[appLogDecryptionAlgorithm](../resources/intune-devices-applogdecryptionalgorithm.md)|DecryptionAlgorithm für Inhalt. Mögliche Werte sind: `aes256`.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionDownloadDetails",
  "downloadUrl": "String",
  "decryptionKey": "String",
  "appLogDecryptionAlgorithm": "String"
}
```




