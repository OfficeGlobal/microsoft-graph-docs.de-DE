---
title: Azure AD Privileged Identity Management
description: Es folgt eine Liste der vom Privileged Identity Management-Dienst bereitgestellten Methoden.
localization_priority: Priority
ms.openlocfilehash: 59a049a299faf0b90baefef8eb44f0365fafa35e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515055"
---
# <a name="azure-ad-privileged-identity-management"></a>Azure AD Privileged Identity Management

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Es folgt eine Liste der vom [Privileged Identity Management](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-privileged-identity-management-configure/)-Dienst bereitgestellten Methoden.

Der Dienst baut auf OData auf. Um die Ergebnisse aus der Abfrage zu filtern, verwenden Sie die standardmäßigen OData-``$filter``-Ausdrücke in den URLs.

## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[privilegedOperationEvent auflisten](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md)-Sammlung |Dient zum Abrufen einer privilegedOperationEvent-Objektsammlung. |
|[privilegedRole abrufen](../api/privilegedrole-get.md) |[privilegedRole](privilegedrole.md)| Dient zum Abrufen eines privilegedRole-Objekts.|
|[privilegedRole auflisten](../api/privilegedrole-list.md) | [privilegedRole](privilegedrole.md)-Sammlung |Dient zum Abrufen einer privilegedRole-Sammlung. |
|[Rollenzuweisungen auflisten](../api/privilegedrole-list-assignments.md) | [privilegedRoleAssignment](privilegedroleassignment.md)-Sammlung |Dient zum Abrufen der privilegedRoleAssignment-Sammlung der jeweiligen Rolle. Jede privilegedRoleAssignment stellt eine Rollenzuweisung für einen Benutzer dar.|
|[selfActivate](../api/privilegedrole-selfactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Aktivieren der Rolle, die dem Anforderer zugewiesen ist.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Deaktivieren der Rolle, die dem Anforderer zugewiesen ist.|
|[privilegedRoleAssignment erstellen](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Erstellen einer neuen privilegedRoleAssignment (Rollenzuweisung) durch Veröffentlichen in der privilegedRoleAssignments-Sammlung.|
|[privilegedRoleAssignment auflisten](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md)-Sammlung |Dient zum Abrufen einer privilegedRoleAssignment-Sammlung. Die Sammlung enthält alle Rollenzuweisungen für die Organisation. Jede privilegedRoleAssignment stellt eine Rollenzuweisung für einen Benutzer dar. |
|[privilegedRoleAssignment abrufen](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md)|Abrufen des privilegedRoleAssignment-Objekts mit der angegebenen Zuweisungs-ID. |
|[privilegedRoleAssignment löschen](../api/privilegedroleassignment-delete.md) | Keine. |Löschen eines privilegedRoleAssignment-Objekts. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Legt die Rollenzuweisung als dauerhaft fest. |
|[makeEligible](../api/privilegedroleassignment-makeeligible.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Legt die Rollenzuweisung als berechtigt fest. |
|[my](../api/privilegedroleassignment-my.md) | [privilegedRoleAssignment](privilegedroleassignment.md)-Sammlung|Abrufen der Rollenzuweisungen des Anforderers. |
|[privilegedRoleSettings abrufen](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](../resources/privilegedrolesettings.md)|Abrufen der Eigenschaften des privilegedRoleSettings-Objekts. |
|[privilegedRoleSummary abrufen](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](../resources/privilegedrolesummary.md)|Abrufen des privilegedRoleSummary-Objekts. |
|[privilegedApproval abrufen](../api/privilegedapproval-get.md) |[privilegedApproval](privilegedapproval.md)| Abrufen eines privilegedApproval-Objekts.|
|[privilegedApproval auflisten](../api/privilegedapproval-list.md) | [privilegedApproval](privilegedapproval.md)-Sammlung |Abrufen einer privilegedApproval-Objektsammlung. |
|[privilegedApproval erstellen](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |Erstellen eines privilegedApproval-Objekts. |
|[privilegedApproval aktualisieren](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |Aktualisieren eines privilegedApproval-Objekts. |
|[myrequests](../api/privilegedapproval-myrequests.md) | [privilegedApproval](privilegedapproval.md)-Sammlung|Erhalten Sie die Genehmigungsanforderungen des Anforderers. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedidentitymanagement-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
