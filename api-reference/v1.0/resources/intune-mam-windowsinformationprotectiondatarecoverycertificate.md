---
title: windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp
description: Windows Information Protection – Datenwiederherstellungszertifikat
author: tfitzmac
ms.openlocfilehash: a66c1eeae6d405aa8d0546ac0143e2a8b3404231
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361663"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a>windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Windows Information Protection – Datenwiederherstellungszertifikat
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|subjectName|Zeichenfolge|Antragstellername des Datenwiederherstellungszertifikats|
|description|Zeichenfolge|Beschreibung des Datenwiederherstellungszertifikats|
|expirationDateTime|DateTimeOffset|Ablaufdatum des Datenwiederherstellungszertifikats|
|certificate|Binär|Datenwiederherstellungszertifikat|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



