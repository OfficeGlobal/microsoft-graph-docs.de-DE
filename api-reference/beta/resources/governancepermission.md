---
title: Ressourcentyp governancePermission
description: 'Stellt die Berechtigung, die ein GovernanceSubject hat für eine bestimmte GovernanceResource dar.  '
ms.openlocfilehash: d7b3e1eb70c89c278ccc2a8b3e9a16e265e4ae97
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062738"
---
# <a name="governancepermission-resource-type"></a>Ressourcentyp governancePermission

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Berechtigung, die ein [GovernanceSubject](../resources/governancesubject.md) hat für eine bestimmte [GovernanceResource](../resources/governanceresource.md)dar.  


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|accessLevel|String|Die Zugriffsebene. Gültige Werte: ``None``, ``UserRead``, ``AdminRead``, und ``AdminReadWrite``.|
|isActive|Boolesch|Gibt an, ob der anfordernden Person hat aktiven rollenzuweisung für die Zugriffsebene.|
|isEligible|Boolesch|Geben Sie an, ob der Requestor alle qualifizierten rollenzuweisung für die Zugriffsebene hat.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```