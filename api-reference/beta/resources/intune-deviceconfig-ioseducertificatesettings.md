---
title: Ressourcentyp iosEduCertificateSettings
description: Vertrauenswürdige Stamm und PFX-Zertifikate für iOS EDU.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8c48883caa9479638b1a727272abdd0bc5762db9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948675"
---
# <a name="ioseducertificatesettings-resource-type"></a>Ressourcentyp iosEduCertificateSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.

Vertrauenswürdige Stamm und PFX-Zertifikate für iOS EDU.
## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|trustedRootCertificate|Binär|Zertifikat der vertrauenswürdigen Stammzertifizierungsstellen.|
|Aus|Zeichenfolge|Der Dateiname in der Benutzeroberfläche angezeigt.|
|certificationAuthority|Zeichenfolge|PKCS Zertifizierungsstelle.|
|certificationAuthorityName|Zeichenfolge|Name der Zertifizierungsstelle PKCS.|
|certificateTemplateName|Zeichenfolge|Name der PKCS Zertifikatsvorlage.|
|renewalThresholdPercentage|Int32|Zertifikat Erneuerung Schwellenwertprozentsatz. Gültige Werte 1 bis 99|
|certificateValidityPeriodValue|Int32|Wert für die Gültigkeitsdauer des Zertifikats.|
|certificateValidityPeriodScale|[certificateValidityPeriodScale](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Skalierung für die Gültigkeitsdauer des Zertifikats. Mögliche Werte sind: `days`, `months` und `years`.|

## <a name="relationships"></a>Beziehungen
Keine
## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```





