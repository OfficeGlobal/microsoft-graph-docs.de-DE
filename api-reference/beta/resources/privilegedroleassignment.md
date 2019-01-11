---
title: Ressourcentyp privilegedRoleAssignment
description: 'Stellt eine privilegierten rollenzuweisung für einen bestimmten Benutzer. '
localization_priority: Normal
ms.openlocfilehash: ec6bc34ecd56839c764592ff298475e8648f300b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823317"
---
# <a name="privilegedroleassignment-resource-type"></a>Ressourcentyp privilegedRoleAssignment

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine privilegierten rollenzuweisung für einen bestimmten Benutzer. 


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste PrivilegedRoleAssignment-Auflistung](../api/privilegedroleassignment-list.md) | [PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung|Rufen Sie die Auflistung von PrivilegedRoleAssignment-Objekten.|
|[Abrufen von privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Lesen Sie Eigenschaften und Beziehungen des PrivilegedRoleAssignment-Objekts.|
|[Erstellen der Zuordnung](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Erstellen Sie eine neue Zuordnung, indem Sie das Veröffentlichen in der Assignments-Auflistung.|
|[Delete](../api/privilegedroleassignment-delete.md) | Keine |PrivilegedRoleAssignment-Objekt zu löschen. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Stellen Sie die rollenzuweisung als dauerhaft entfernt.|
|[makeEligible](../api/privilegedroleassignment-makeeligible.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Stellen Sie die rollenzuweisung als geeignet.|
|[Meine](../api/privilegedroleassignment-my.md)|[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung|Abrufen des aktuellen Benutzers privilegierten rollenzuweisungen.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|expirationDateTime|dateTimeOffset|Die UTC-DateTime, die temporäre privilegierten rollenzuweisung abgelaufen sein wird. Für permanente rollenzuweisung ist der Wert null.|
|id|string| Der eindeutige Bezeichner für die privilegierten rollenzuweisung. Schreibgeschützt. Es ist im Format "UserId_roleId", wobei Benutzer-ID ist die GUID-Zeichenfolge für Azure AD-Benutzer-Id und RoleId ist die GUID für Azure Administrator Rollen-Id-Zeichenfolge.|
|isElevated|Boolean|**true,** Wenn die rollenzuweisung aktiviert ist. **false,** Wenn die rollenzuweisung deaktiviert wird.|
|resultMessage|string|Ergebnisnachricht vom Dienst festgelegt.|
|roleId|string|Rollenbezeichner. Im Zeichenformat GUID.|
|userId|string|Benutzer-ID. Im Zeichenformat GUID.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|roleInfo|[privilegedRole](privilegedrole.md)| Schreibgeschützt. Lässt Nullwerte zu. Die zugehörige Rolle-Informationen.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
}-->

```json
{
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isElevated": true,
  "resultMessage": "string",
  "roleId": "string",
  "userId": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
