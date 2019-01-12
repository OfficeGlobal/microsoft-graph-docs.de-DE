---
title: Ressourcentyp symantecCodeSigningCertificate
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9c195a31dae12c1a67d8226a219fe57a68bf905d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965936"
---
# <a name="symanteccodesigningcertificate-resource-type"></a>Ressourcentyp symantecCodeSigningCertificate

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Noch nicht dokumentiert.
## <a name="methods"></a>Methoden
|Methode|Rückgabetyp|Beschreibung|
|:---|:---|:---|
|[Abrufen von symantecCodeSigningCertificate](../api/intune-apps-symanteccodesigningcertificate-get.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Lesen Sie Eigenschaften und Beziehungen des [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) -Objekts.|
|[SymantecCodeSigningCertificate aktualisieren](../api/intune-apps-symanteccodesigningcertificate-update.md)|[symantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md)|Aktualisieren Sie die Eigenschaften eines [SymantecCodeSigningCertificate](../resources/intune-apps-symanteccodesigningcertificate.md) -Objekts.|

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|id|String|Schlüssel der Entität|
|content|Binär|Das Windows Symantec Codesignierung-Zertifikat im Format Rohdaten.|
|status|[certificateStatus](../resources/intune-apps-certificatestatus.md)|Der Status Cert bereitgestellt oder nicht bereitgestellt. Mögliche Werte sind: `notProvisioned` und `provisioned`.|
|password|Zeichenfolge|Das Kennwort für die PFX-Datei.|
|subjectName|Zeichenfolge|Der Antragstellername für das Zertifikat.|
|Betreff|Zeichenfolge|Der Wert der Betreff für das Zertifikat.|
|issuerName|Zeichenfolge|Der Name der Aussteller für das Zertifikat.|
|Aussteller|Zeichenfolge|Der Wert der Aussteller für das Zertifikat.|
|expirationDateTime|DateTimeOffset|Das Ablaufdatum des Zertifikats.|
|uploadDateTime|DateTimeOffset|Der Typ des der Cert CodeSigning als Symantec Cert.|

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





