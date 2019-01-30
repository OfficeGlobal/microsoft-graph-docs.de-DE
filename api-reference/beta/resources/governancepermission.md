---
title: Ressourcentyp governancePermission
description: 'Stellt die Berechtigung, die ein GovernanceSubject hat für eine bestimmte GovernanceResource dar.  '
localization_priority: Normal
ms.openlocfilehash: 255cd4c25a957a40e5e5ac765ed446f516c51607
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643783"
---
# <a name="governancepermission-resource-type"></a>Ressourcentyp governancePermission

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Stellt die Berechtigung, die ein [GovernanceSubject](../resources/governancesubject.md) hat für eine bestimmte [GovernanceResource](../resources/governanceresource.md)dar.  


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|accessLevel|String|Die Zugriffsebene. Gültige Werte: ``None``, ``UserRead``, ``AdminRead``, und ``AdminReadWrite``.|
|isActive|Boolean|Gibt an, ob der anfordernden Person hat aktiven rollenzuweisung für die Zugriffsebene.|
|isEligible|Boolean|Geben Sie an, ob der Requestor alle qualifizierten rollenzuweisung für die Zugriffsebene hat.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancepermission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
