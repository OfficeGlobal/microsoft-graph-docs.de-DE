---
title: Ressourcentyp privilegedRole
description: 'Stellt eine Azure AD-Administratorrolle z. B.: **globaler Administrator, Abrechnungsadministrator, Dienstadministrator, Benutzer-Administrator, Kennwort-Administrator**usw..'
ms.openlocfilehash: 0c04ab9de13732e4ac9eecb943a10945bec59d02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059079"
---
# <a name="privilegedrole-resource-type"></a>Ressourcentyp privilegedRole

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Azure AD-Administratorrolle z. B.: **globaler Administrator, Abrechnungsadministrator, Dienstadministrator, Benutzer-Administrator, Kennwort-Administrator**usw..


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Objekte in der Liste privilegedRole](../api/privilegedrole-list.md) | [PrivilegedRole](privilegedrole.md) -Auflistung|Ruft die Auflistung der PrivilegedRole.|
|[Abrufen von privilegedRole](../api/privilegedrole-get.md) | [privilegedRole](privilegedrole.md) |Lesen Sie Eigenschaften und Beziehungen des PrivilegedRole-Objekts.|
|[Liste Zuordnungen](../api/privilegedrole-list-assignments.md) |[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung| Rufen Sie eine Assignment-Objekt-Auflistung für diese Rolle.|
|[selfActivate](../api/privilegedrole-selfactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Aktivieren Sie die zugeordnete Rolle.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md)|[privilegedRoleAssignment](privilegedroleassignment.md)|Deaktivieren Sie die zugeordnete Rolle.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|id|string|Der eindeutige Bezeichner für Administratorrolle. Es ist eine GUID-Zeichenfolge und hat den gleichen Wert wie der Rolle Vorlagen-Id aus dem Azure Active Directory für die gegebene Rolle. Schreibgeschützt.|
|name|string|Rollenname.|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|assignments|[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung| Die Zuordnungen für diese Rolle. Schreibgeschützt. Lässt Nullwerte zu.|
|settings|[privilegedRoleSettings](privilegedrolesettings.md)| Die Einstellungen für diese Rolle. Schreibgeschützt. Lässt Nullwerte zu.|
|Zusammenfassung|[privilegedRoleSummary](privilegedrolesummary.md)| Der zusammenfassende Informationen für diese Rolle. Schreibgeschützt. Lässt Nullwerte zu.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRole"
}-->

```json
{
  "id": "string (identifier)",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->