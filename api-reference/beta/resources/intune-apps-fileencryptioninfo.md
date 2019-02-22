---
title: fileEncryptionInfo-Ressourcentyp
description: Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 060f8eac1bfff3f0d2e18d52428deb884da4a759
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168572"
---
# <a name="fileencryptioninfo-resource-type"></a>fileEncryptionInfo-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Enthält Eigenschaften für Dateiverschlüsselungsinformationen für die Inhaltsversion einer branchenspezifischen App.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|encryptionKey|Binär|Der Schlüssel, der zum Verschlüsseln des Inhalts der Datei verwendet wurde.|
|initializationVector|Binär|Der Initialisierungsvektor, der für den Verschlüsselungsalgorithmus verwendet wurde.|
|mac|Binär|Der Hash aus dem verschlüsselten Dateiinhalt + IV (Inhaltshash).|
|macKey|Binär|Der Schlüssel, der für den Abruf von mac verwendet wurde.|
|profileIdentifier|Zeichenfolge|Die Bezeichner des Profils.|
|fileDigest|Binary|Der Digest der Datei vor der Verschlüsselung.|
|fileDigestAlgorithm|String|Der Dateidigestalgorithmus.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```




