---
title: Ressourcentyp governancePermission
description: 'Stellt die Berechtigung, die ein GovernanceSubject hat für eine bestimmte GovernanceResource dar.  '
localization_priority: Normal
ms.openlocfilehash: e082ca50e5642e865b3e30859eea607df63a03b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882873"
---
# <a name="governancepermission-resource-type"></a>Ressourcentyp governancePermission

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Berechtigung, die ein [GovernanceSubject](../resources/governancesubject.md) hat für eine bestimmte [GovernanceResource](../resources/governanceresource.md)dar.  


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|accessLevel|Zeichenfolge|Die Zugriffsebene. Gültige Werte: ``None``, ``UserRead``, ``AdminRead``, und ``AdminReadWrite``.|
|isActive|Boolescher Wert|Gibt an, ob der anfordernden Person hat aktiven rollenzuweisung für die Zugriffsebene.|
|isEligible|Boolescher Wert|Geben Sie an, ob der Requestor alle qualifizierten rollenzuweisung für die Zugriffsebene hat.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
