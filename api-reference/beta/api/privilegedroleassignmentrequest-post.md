---
title: Erstellen von privilegedRoleAssignmentRequest
description: Erstellen Sie ein Privilegedroleassignmentrequest-Objekt.
localization_priority: Normal
ms.openlocfilehash: 3f1b88415e5671e38ad557cc28200569a42a9630
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847769"
---
# <a name="create-privilegedroleassignmentrequest"></a>Erstellen von privilegedRoleAssignmentRequest

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Erstellen Sie ein [Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) -Objekt.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignmentRequests
```

## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [Privilegedroleassignmentrequest](../resources/privilegedroleassignmentrequest.md) -Objekts. 

| Eigenschaft     | Typ    |  Beschreibung|
|:---------------|:--------|:----------|
|roleId|String|Die ID der Rolle. Erforderlich.|
|type|String|Stellt die den Typ des Vorgangs für die rollenzuweisung. Der Wert kann sein `AdminAdd`: Administratoren hinzufügen von Benutzern zu Rollen; `UserAdd`: Hinzufügen von Benutzern rollenzuweisungen. Erforderlich.|
|assignmentState|String|Der Status der Zuordnung. Der Wert kann sein `Eligible` für die Zuweisung von zu auswählbaren `Active` – Wenn sie direkt zugeordnet ist `Active` von Administratoren, oder an einer Zuordnung zu auswählbaren durch den Benutzer aktiviert. Mögliche Werte: ``NotStarted``, `Completed`, `RequestedApproval`, `Scheduled`, `Approved`, `ApprovalDenied`, `ApprovalAborted`, `Cancelling`, `Cancelled`, `Revoked`, `RequestExpired`. Erforderlich.|
|Grund|String|Der Grund muss bereitgestellt werden, für die Rolle Zuordnung Anforderung zur Überwachung und Zweck überprüfen.|
|Zeitplan|[governanceSchedule](../resources/governanceschedule.md)|Den Zeitplan der Rolle Zuordnung Anforderung.|

## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [PrivilegedRoleAssignmentRequest](../resources/privilegedroleassignmentrequest.md) -Objekts in der Antworttext.

### <a name="error-codes"></a>Fehlercodes
Diese API gibt den betreffenden Standard-HTTP-Fehlercodes. Darüber hinaus kann die Fehlercodes in der folgenden Tabelle aufgeführten zurückgegeben werden.

|Fehlercode     | Fehlermeldung              | 
|:--------------------| :---------------------|
| 400 BadRequest | RoleAssignmentRequest-Eigenschaft wurde NULL |
| 400 BadRequest | Kann nicht RoleAssignmentRequest Objekt deserialisiert werden. |
| 400 BadRequest | RoleId ist erforderlich. |
| 400 BadRequest | Startdatum muss angegeben werden und sollte jetzt größer sein. |
| 400 BadRequest | Ein Zeitplan für diesen Benutzer, Rollen und Zeitplan ist bereits vorhanden. |
| 400 BadRequest | Für diesen Benutzer, Rollen und Genehmigung ist eine ausstehende Genehmigung bereits vorhanden. |
| 400 BadRequest | Requestor Grund ist nicht vorhanden. |
| 400 BadRequest | Requestor Grund sollten weniger als 500 Zeichen lang sein. |
| 400 BadRequest | Elevation-Dauer muss zwischen 0,5 und {von Einstellung} sein. |
| 400 BadRequest | Es ist eine Überlappung zwischen geplanten Aktivierungs- und die Anforderung. |
| 400 BadRequest | Die Rolle ist bereits aktiviert. |
| 400 BadRequest | GenericElevateUserToRoleAssignments: Tickting Informationen ist erforderlich und nicht in der Aktivierungsprozess angegeben. |
| 400 BadRequest | Es ist eine Überlappung zwischen geplanten Aktivierungs- und die Anforderung. |
| 403 nicht autorisiert | Elevation erfordert Multi-Factor Authentication. |
| 403 nicht autorisiert | Im Namen Elevation ist nicht zulässig. |

## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "post_privilegedroleassignmentrequest"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignmentRequests
Content-type: application/json

{
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "schedule": {
        "startDateTime": "2018-02-08T02:35:17.903Z"
    },
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignmentRequest"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedRoleAssignmentRequests/$entity",
    "schedule": {
        "type": "activation",
        "startDateTime": "2018-02-08T02:35:17.903Z",
        "endDateTime": null,
        "duration" : null
    },
    "id": "e13ef8a0-c1cb-4d03-aaae-9cd1c8ede2d1",
    "evaluateOnly": false,
    "type": "UserAdd",
    "assignmentState": "Active",
    "requestedDateTime": "2018-02-08T02:35:42.9137335Z",
    "status": "NotStarted",
    "duration": "2",
    "reason": "Activate the role for business purpose",
    "ticketNumber": "234",
    "ticketSystem": "system",
    "userId": "Self"，
    "roleId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Post privilegedRoleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
