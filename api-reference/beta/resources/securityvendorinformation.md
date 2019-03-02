---
title: securityVendorInformation-Ressourcentyp
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 7f48c27ba94d8419ce244143a48cf6ab04dd080e
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30364584"
---
# <a name="securityvendorinformation-resource-type"></a>securityVendorInformation-Ressourcentyp

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enthält Details zum Sicherheitsprodukt/-Dienstanbieter,-Anbieter und-subprovider (beispielsweise Vendor = Microsoft; Provider = Windows Defender-ATP; subProvider = AppLocker).

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|Anbieter |Zeichenfolge|Bestimmter Anbieter (Product/Service-not Vendor Company); Beispiel: WindowsDefenderATP.|
|Provider Version|Zeichenfolge|Die Version des Anbieters oder subproviders, sofern vorhanden, die die Warnung generiert hat. **Erforderlich**|
|Sekundären Anbieter|Zeichenfolge|Bestimmter subprovider (unter Aggregations Anbieter); Beispiel: WindowsDefenderATP. SmartScreen.|
|Hersteller |Zeichenfolge|Name des Warnungs Anbieters (beispielsweise Microsoft, Dell, FireEye arbeitete). **Erforderlich**|

## <a name="json-representation"></a>JSON-Darstellung

Folllowing ist eine JSON-Darstellung der Ressource.
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
<!--
{
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/securityvendorinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
