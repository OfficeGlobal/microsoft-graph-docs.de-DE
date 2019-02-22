---
title: androidEnrollmentCompanyCode-Ressourcentyp
description: Eine Klasse zum Speichern von Spezialdaten für die Registrierung über die Android-Verwaltungs-API von Google, wie Token-, URL-und QR-Code Inhalte
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0cd3ede4193ea3fdb33d33010349812150848e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169342"
---
# <a name="androidenrollmentcompanycode-resource-type"></a>androidEnrollmentCompanyCode-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Eine Klasse zum Speichern von Spezialdaten für die Registrierung über die Android-Verwaltungs-API von Google, wie Token-, URL-und QR-Code Inhalte

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|enrollmentToken|Zeichenfolge|Vom Benutzer zum Registrieren des Geräts verwendete Registrierungs Token.|
|qrCodeContent|Zeichenfolge|Zeichenfolge, die zur Generierung eines QR-Codes für das Token verwendet wird|
|qrCodeImage|[mimeContent](../resources/intune-shared-mimecontent.md)|Generierter QR-Code für das Token.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```




