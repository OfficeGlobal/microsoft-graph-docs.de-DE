---
title: iosEduCertificateSettings-Ressourcentyp
description: Vertrauenswürdige Stamm-und PFX-Zertifikate für iOS EDU.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c94b7bc75022f8338a41da3b3b9d135dff47ac3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142651"
---
# <a name="ioseducertificatesettings-resource-type"></a>iosEduCertificateSettings-Ressourcentyp

> **Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.

Vertrauenswürdige Stamm-und PFX-Zertifikate für iOS EDU.

## <a name="properties"></a>Eigenschaften
|Eigenschaft|Typ|Beschreibung|
|:---|:---|:---|
|trustedRootCertificate|Binär|Vertrauenswürdiges Stammzertifikat.|
|certFileName|Zeichenfolge|Dateiname, der in der Benutzeroberfläche angezeigt werden soll.|
|certificationAuthority|Zeichenfolge|PKCS-ZertifizierungsStelle.|
|certificationAuthorityName|Zeichenfolge|Name der PKCS-ZertifizierungsStelle.|
|certificateTemplateName|Zeichenfolge|Name der PKCS-Zertifikatvorlage.|
|Eigenschaften renewalthresholdpercentage|Int32|Schwellenwert für die Zertifikaterneuerung. Gültige Werte 1 bis 99|
|certificateValidityPeriodValue|Int32|Wert für den Gültigkeitszeitraum des Zertifikats.|
|Certificatevalidityperiodscale wurden|[Certificatevalidityperiodscale wurden](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|Skalierung für den Gültigkeitszeitraum des Zertifikats. Mögliche Werte sind: `days`, `months` und `years`.|

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




