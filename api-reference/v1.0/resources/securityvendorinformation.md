---
title: Ressourcentyp securityVendorInformation
description: " SubProvider = AppLocker)."
localization_priority: Normal
ms.openlocfilehash: e9d8551c085c05007388bf0c6e33143994c6969b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820146"
---
# <a name="securityvendorinformation-resource-type"></a>Ressourcentyp securityVendorInformation

Enthält Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|Anbieter |String|Bestimmte Anbieter (Product/Service - nicht Hersteller Unternehmen); beispielsweise WindowsDefenderATP.|
|providerVersion|String|Version des Anbieters oder Subprovider, falls vorhanden, die Warnung ausgelöst wurde. *Erforderlich*|
|subProvider|String|Bestimmte Subprovider (unter aggregieren Anbieter); beispielsweise WindowsDefenderATP.SmartScreen.|
|Hersteller |String|Name des Herstellers alert (beispielsweise Microsoft, Dell, FireEye). *Erforderlich*|


## <a name="json-representation"></a>JSON-Darstellung

Die folgenden ist eine JSON-Darstellung der Ressource.
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
