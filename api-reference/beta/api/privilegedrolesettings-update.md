---
title: PrivilegedRoleSettings aktualisieren
description: Aktualisieren Sie die Rolleneinstellungen für die angegebene Rollen Einstellung. Ein privilegedRoleSettings-Objekt wird zurückgegeben.
localization_priority: Normal
ms.openlocfilehash: f416656362c5be0ccdaa2b3aaa7812511e357875
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789606"
---
# <a name="update-privilegedrolesettings"></a>PrivilegedRoleSettings aktualisieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie die Rolleneinstellungen für die angegebene Rollen Einstellung. Ein [privilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekt wird zurückgegeben.
## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

>**Hinweis:** Der anfordernde muss eine der folgenden Rollen besitzen: Administrator für privilegierte Rollen, globaler Administrator, Sicherheitsadministrator oder Sicherheits Leser. 

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. all    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung eines [privilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekts an.

In der folgenden Tabelle sind die Eigenschaften aufgeführt, die Sie beim Aktualisieren einer Rollen Einstellung angeben können.

|Eigenschaft|Typ|Beschreibung|
|:---------------|:--------|:----------|
|elevationDuration|duration|Die Dauer der Aktivierung der Rolle. Erforderlich.|
|id|string|Der eindeutige Bezeichner für die Rolleneinstellungen. Schreibgeschützt. Erforderlich.|
|isMfaOnElevationConfigurable|Boolesch|**true** , wenn mfaOnElevation ist konfigurierbar. **false** , wenn mfaOnElevation nicht konfigurierbar ist. Erforderlich.|
|lastGlobalAdmin|Boolesch|Ausschließlich für interne Zwecke.|
|maxElavationDuration|duration|Maximale Dauer der aktivierten Rolle. Erforderlich.|
|mfaOnElevation|Boolesch|**true** , wenn MFA erforderlich ist, um die Rolle zu aktivieren. **false** , wenn MFA nicht erforderlich ist, um die Rolle zu aktivieren. Erforderlich.|
|minElevationDuration|duration|Mindestdauer für die aktivierte Rolle. Erforderlich.|
|notificationToUserOnElevation|Boolesch|**true** , wenn eine Benachrichtigung an den Endbenutzer gesendet wird, wenn die Rolle aktiviert wird. **false** , wenn keine Benachrichtigung gesendet wird, wenn die Rolle aktiviert wird. Erforderlich.|
|ticketingInfoOnElevation|Boolesch|**true** , wenn die Ticketing-Informationen erforderlich sind, wenn die Rolle zu aktivieren. **false** , wenn die Ticket Informationen beim Aktivieren der Rolle nicht erforderlich sind. Erforderlich.|
|approvalOnElevation|Boolesch|**true** , wenn die Genehmigung erforderlich ist, wenn die Rolle zu aktivieren. **false** , wenn die Genehmigung nicht erforderlich ist, wenn die Rolle zu aktivieren. Erforderlich.|
|approverIds|String collection|Liste der Genehmigungs-IDs, falls für die Aktivierung Genehmigung erforderlich ist.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.

Beachten Sie, dass der Mandant bei PIM registriert werden muss. Andernfalls wird der vom HTTP 403 Forbidden-Statuscode zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "put_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
Content-type: application/json

{
    "id": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "elevationDuration": "PT8H",
    "notificationToUserOnElevation": false,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": false,
    "maxElavationDuration": "PT0S",
    "minElevationDuration": "PT0S",
    "lastGlobalAdmin": false,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": false,
    "approverIds": ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort.

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesettings-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
