---
title: Ressourcentyp iosEduCertificateSettings
description: Vertrauenswürdige Stamm und PFX-Zertifikate für iOS EDU.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d23b379dea7a75e4ae79029845cd6e9f956503c0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423552"
---
# <a name="ioseducertificatesettings-resource-type"></a>Ressourcentyp iosEduCertificateSettings

> **Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.

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




