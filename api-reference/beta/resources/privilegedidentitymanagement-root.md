---
title: Identitätsmanagement Azure AD-Berechtigungen
description: Hier wird die Liste der Methoden, die vom privilegierten Identity Management-Dienst bereitgestellt werden.
localization_priority: Priority
ms.openlocfilehash: c1108711c96dd253f784a418a396ca30507c5f7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884063"
---
# <a name="azure-ad-privileged-identity-management"></a>Identitätsmanagement Azure AD-Berechtigungen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Hier wird die Liste der Methoden, die vom [Privilegierten Identity Management](https://azure.microsoft.com/en-us/documentation/articles/active-directory-privileged-identity-management-configure/) -Dienst bereitgestellt werden.

Der Dienst wird auf der Basis OData erstellt. Verwenden Sie zum Filtern der Ergebnisse der Abfrage, die standard-OData ``$filter`` Ausdrücke in die URIs.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [PrivilegedOperationEvent](privilegedoperationevent.md) -Auflistung |Rufen Sie PrivilegedOperationEvent-Auflistung-Objekts. |
|[Abrufen von privilegedRole](../api/privilegedrole-get.md) |[privilegedRole](privilegedrole.md)| Rufen Sie ein PrivilegedRole-Objekt.|
|[Liste privilegedRole](../api/privilegedrole-list.md) | [PrivilegedRole](privilegedrole.md) -Auflistung |Rufen Sie PrivilegedRole-Auflistung-Objekts. |
|[Liste von rollenzuweisungen](../api/privilegedrole-list-assignments.md) | [PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung |PrivilegedRoleAssignment-Auflistung für die bestimmten Rolle abrufen. Jeder PrivilegedRoleAssignment stellt eine rollenzuweisung an einen Benutzer.|
|[selfActivate](../api/privilegedrole-selfactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Aktivieren Sie die Rolle, die an den Requestor zugewiesen ist.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Deaktivieren Sie die Rolle, die an den Requestor zugewiesen ist.|
|[Erstellen von privilegedRoleAssignment](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Erstellen Sie eine neue PrivilegedRoleAssignment (rollenzuweisung), durch die Veröffentlichung auf der PrivilegedRoleAssignments-Auflistung.|
|[Liste privilegedRoleAssignment](../api/privilegedroleassignment-list.md) | [PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung |Rufen Sie PrivilegedRoleAssignment-Auflistung-Objekts. Die Auflistung enthält alle rollenzuweisungen für die Organisation. Jeder PrivilegedRoleAssignment stellt eine rollenzuweisung an einen Benutzer. |
|[Abrufen von privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md)|Rufen Sie PrivilegedRoleAssignment-Objekt mit der Id angegebenen Zuweisung. |
|[PrivilegedRoleAssignment löschen](../api/privilegedroleassignment-delete.md) | Keine. |PrivilegedRoleAssignment-Objekt zu löschen. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Stellen Sie die rollenzuweisung als dauerhaft entfernt. |
|[makeEligible](../api/privilegedroleassignment-makeeligible.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Stellen Sie die rollenzuweisung als geeignet. |
|[Meine](../api/privilegedroleassignment-my.md) | [PrivilegedRoleAssignment](privilegedroleassignment.md) -Auflistung|Rufen Sie das jeweilige rollenzuweisungen. |
|[Abrufen von privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](../resources/privilegedrolesettings.md)|Rufen Sie die Eigenschaften des PrivilegedRoleSettings-Objekts ab. |
|[Abrufen von privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](../resources/privilegedrolesummary.md)|Rufen Sie das PrivilegedRoleSummary-Objekt. |
|[Abrufen von privilegedApproval](../api/privilegedapproval-get.md) |[privilegedApproval](privilegedapproval.md)| Rufen Sie ein PrivilegedApproval-Objekt.|
|[Liste privilegedApproval](../api/privilegedapproval-list.md) | [PrivilegedApproval](privilegedapproval.md) -Auflistung |Rufen Sie PrivilegedApproval-Auflistung-Objekts. |
|[Erstellen von privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |PrivilegedApproval-Objekt zu erstellen. |
|[PrivilegedApproval aktualisieren](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |PrivilegedApproval-Objekt zu aktualisieren. |
|[myrequests](../api/privilegedapproval-myrequests.md) | [PrivilegedApproval](privilegedapproval.md) -Auflistung|Get-Anforderungen für das jeweilige Genehmigung. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
