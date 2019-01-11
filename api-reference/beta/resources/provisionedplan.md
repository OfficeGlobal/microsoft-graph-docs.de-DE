---
title: provisionedPlan-Ressourcentyp
description: Die **ProvisionedPlans**-Eigenschaft der user-Entität und der oganization-Entität ist eine Sammlung von **provisionedPlan**.
localization_priority: Normal
ms.openlocfilehash: 7bed57761777e637fdc2e567d10aa7f741a86663
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837254"
---
# <a name="provisionedplan-resource-type"></a>provisionedPlan-Ressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die **ProvisionedPlans**-Eigenschaft der [user](user.md)-Entität und der [oganization](organization.md)-Entität ist eine Sammlung von **provisionedPlan**.


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|capabilityStatus|Zeichenfolge|Z. B. „Aktiviert“.|
|provisioningStatus|Zeichenfolge|Z. B. „Erfolgreich“.|
|service|Zeichenfolge|Der Name des Diensts. z. B. „AccessControlS2S“|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisionedplan"
}-->

```json
{
  "capabilityStatus": "string",
  "provisioningStatus": "string",
  "service": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisionedPlan resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
