---
title: Ressourcentyp privilegedRole
description: 'Stellt eine Azure AD-Administratorrolle z. B.: **globaler Administrator, Abrechnungsadministrator, Dienstadministrator, Benutzer-Administrator, Kennwort-Administrator**usw..'
localization_priority: Normal
ms.openlocfilehash: 131999f52a583400b018e98d2319118f69ca87e8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513746"
---
# <a name="privilegedrole-resource-type"></a>Ressourcentyp privilegedRole

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|assignments|[PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung| Die Zuordnungen für diese Rolle. Schreibgeschützt. Nullwerte zulassend.|
|settings|[privilegedRoleSettings](privilegedrolesettings.md)| Die Einstellungen für diese Rolle. Schreibgeschützt. Nullwerte zulassend.|
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
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrole.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
