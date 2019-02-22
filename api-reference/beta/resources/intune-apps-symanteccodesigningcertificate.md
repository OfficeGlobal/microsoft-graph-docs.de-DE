---
title: symantecCodeSigningCertificate-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 550ba33f81db9fb38f6d19f3b756a67d7c3b9aa1
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158716"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>symantecCodeSigningCertificate-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Noch nicht dokumentiert.

## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[SymantecCodeSigningCertificate abrufen](../api/intune-apps-symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Lesen von Eigenschaften und Beziehungen des [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) -Objekts.|
|[SymantecCodeSigningCertificate aktualisieren](../api/intune-apps-symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Aktualisieren der Eigenschaften eines [symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|content|Binär|Das Windows Symantec Code Signing Certificate im RAW-Datenformat.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|Der CERT-Status, der für die Einrichtung oder nicht-Einrichtung vorgesehen ist. Mögliche Werte sind: `notProvisioned` und `provisioned`.|
|password|String|Das für die PFX-Datei erforderliche Kennwort.|
|subjectName|Zeichenfolge|Der AntragsTeller Name für das Zertifikat.|
|subject|Zeichenfolge|Der Subject-Wert für das Zertifikat.|
|issuerName|Zeichenfolge|Der Aussteller Name für das Zertifikat.|
|Aussteller|Zeichenfolge|Der Aussteller Wert für das Zertifikat.|
|expirationDateTime|DateTimeOffset|Das Ablaufdatum des Zertifikats.|
|uploadDateTime|DateTimeOffset|Der Typ des deSign Zertifikats als Symantec cert.|

## <a name="relationships"></a>Beziehungen
Keine

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.symantecCodeSigningCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.symantecCodeSigningCertificate",
  "id": "String (identifier)",
  "content": "binary",
  "status": "String",
  "password": "String",
  "subjectName": "String",
  "subject": "String",
  "issuerName": "String",
  "issuer": "String",
  "expirationDateTime": "String (timestamp)",
  "uploadDateTime": "String (timestamp)"
}
```




