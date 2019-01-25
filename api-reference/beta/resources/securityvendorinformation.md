---
title: Ressourcentyp securityVendorInformation
description: " > **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e67a5306b1dd08933877dbe3e64cab766ccd6a96
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512178"
---
# <a name="securityvendorinformation-resource-type"></a>Ressourcentyp securityVendorInformation

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Enthält Details über die Produkt-Dienst Sicherheitsanbieter, Anbieter und Subprovider (beispielsweise Hersteller = Microsoft; Provider = Windows Defender ATP; SubProvider = AppLocker).

## <a name="properties"></a>Eigenschaften

| Eigenschaft   | Typ|Beschreibung|
|:---------------|:--------|:----------|
|Provider |String|Bestimmte Anbieter (Product/Service - nicht Hersteller Unternehmen); beispielsweise WindowsDefenderATP.|
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
