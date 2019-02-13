---
title: Erstellen von governanceRoleAssignmentRequest
description: Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll. Die folgende Tabelle enthält die Vorgänge.
localization_priority: Normal
ms.openlocfilehash: 104ab1a0d4909bc2181df70bc4fc895fc4558260
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967221"
---
# <a name="create-governanceroleassignmentrequest"></a>Erstellen von governanceRoleAssignmentRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Erstellen Sie eine Rolle Zuordnung Anforderung zur Darstellung der Operation in einer rollenzuweisung angezeigt werden soll. Die folgende Tabelle enthält die Vorgänge.

| Vorgang                                   | Typ        |
|:--------------------------------------------|:------------|
| Zuweisen einer rollenzuweisung                    | AdminAdd    |
| Aktivieren einer qualifizierten rollenzuweisung        | UserAdd     |
| Deaktivieren einer aktivierten rollenzuweisung     | UserRemove  |
| Entfernen einer rollenzuweisung                    | AdminRemove |
| Aktualisieren einer rollenzuweisung                    | AdminUpdate |
| So erweitern Sie meine rollenzuweisung anfordern        | UserExtend  |
| Erweitern Sie eine rollenzuweisung                    | AdminExtend |
| Anforderung an meine abgelaufene rollenzuweisung erneuern | UserRenew   |
| Erneuern einer abgelaufenen rollenzuweisung            | AdminRenew  |

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp                        | Berechtigungen                               |
|:---------------------------------------|:------------------------------------------|
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | PrivilegedAccess.ReadWrite.AzureResources |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt                            |
| Anwendung                            | PrivilegedAccess.ReadWrite.AzureResources |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /privilegedAccess/azureResources/roleAssignmentRequests
```

## <a name="request-headers"></a>Anforderungsheader

| Name          | Beschreibung      |
|:--------------|:-----------------|
| Authorization | Bearer {code}    |
| Content-type  | application/json |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts.

| Eigenschaft         | Typ                                                     | Beschreibung |
|:-----------------|:---------------------------------------------------------|:--|
| resourceId       | String                                                   | Die ID der Ressource. Erforderlich. |
| roleDefinitionId | Zeichenfolge                                                   | Die ID der Rollendefinition. Erforderlich. |
| subjectId        | Zeichenfolge                                                   | Die ID des Betreffs. Erforderlich. |
| assignmentState  | Zeichenfolge                                                   | Der Status der Zuordnung. Der Wert kann sein `Eligible` und `Active`. Erforderlich. |
| type             | Zeichenfolge                                                   | Der Anforderungstyp. Der Wert kann sein `AdminAdd`, `UserAdd`, `AdminUpdate`, `AdminRemove`, `UserRemove`, `UserExtend`, `UserRenew`, `AdminRenew`und `AdminExtend`. Erforderlich. |
| Grund           | Zeichenfolge                                                   | Der Grund muss bereitgestellt werden, für die Rolle Zuordnung Anforderung zur Überwachung und Zweck überprüfen. |
| Zeitplan         | [governanceSchedule](../resources/governanceschedule.md) | Den Zeitplan der Rolle Zuordnung Anforderung. Für Anforderungstyp `UserAdd`, `AdminAdd`, `AdminUpdate`, und `AdminExtend`, es ist erforderlich. |

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `201 Created` Antwortcode und eines [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) -Objekts in der Antworttext.

### <a name="error-codes"></a>Fehlercodes

Diese API gibt die standard-HTTP-Fehlercodes zurück. Darüber hinaus gibt auch die Fehlercodes in der folgenden Tabelle aufgeführten zurück.

| Fehlercode     | Fehlermeldung                               | Details       |
|:---------------|:--------------------------------------------|:--------------|
| 400 BadRequest | RoleNotFound                                | Die `roleDefinitionId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann. |
| 400 BadRequest | ResourceIsLocked                            | Die Ressource, die im Textkörper Anforderung bereitgestellt ist, im Zustand des `Locked` und Role Assignment Anforderungen kann nicht erstellt werden. |
| 400 BadRequest | SubjectNotFound                             | Die `subjectId` vorausgesetzt, in der Anforderung Nachrichtentext nicht gefunden werden kann. |
| 400 BadRequest | PendingRoleAssignmentRequest                | Gibt es vorhanden bereits eine ausstehende [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) im System. |
| 400 BadRequest | RoleAssignmentExists                        | Der zu erstellenden bereits angefordert [GovernanceRoleAssignment](../resources/governanceroleassignment.md) im System vorhanden ist. |
| 400 BadRequest | RoleAssignmentDoesNotExist                  | Die [GovernanceRoleAssignment](../resources/governanceroleassignment.md) aktualisiert/erweitert werden angefordert ist im System nicht vorhanden. |
| 400 BadRequest | RoleAssignmentRequestPolicyValidationFailed | Die [GovernanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) entspricht nicht den Richtlinien für interne und kann nicht erstellt werden. |

## <a name="examples"></a>Beispiele

Die folgenden Beispiele zeigen, wie diese API verwendet.

### <a name="example-1-administrator-assigns-user-to-a-role"></a>In Beispiel 1: Administrator weist Benutzer zu einer Rolle

In diesem Beispiel weist ein Administrator Benutzer nawu@fimdev.net Rolle Abrechnung.

 >**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.

| Eigenschaft         | Typ                                                     | Erforderlich                 | Wert |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| resourceId       | String                                                   | Ja                      | \<resourceId\> |
| roleDefinitionId | Zeichenfolge                                                   | Ja                      | \<roleDefinitionId\> |
| subjectId        | Zeichenfolge                                                   | Ja                      | \<subjectId\> |
| assignmentState  | Zeichenfolge                                                   | Ja                      | Berechtigte / Active |
| type             | Zeichenfolge                                                   | Ja                      | AdminAdd |
| Grund           | Zeichenfolge                                                   | hängt von der Rolle Einstellungen |   |
| Zeitplan         | [governanceSchedule](../resources/governanceschedule.md) | Ja                      |   |

#### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Eligible",
  "type": "AdminAdd",
  "reason": "Assign an eligible role",
  "schedule": {
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "type": "Once"
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "1232e4ea-741a-4be5-8044-5edabdd61672",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "ea48ad5e-e3b0-4d10-af54-39a45bbfe68d",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminAdd",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "Evaluate Only",
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "AdminRequestRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:37:43.356Z",
    "endDateTime": "2018-11-08T23:37:43.356Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-2-user-activates-eligible-role"></a>Beispiel 2: Benutzer aktiviert zu auswählbaren Rolle

In diesem Beispiel wird der Benutzer nawu@fimdev.net zu auswählbaren Abrechnung Rolle aktiviert.

| Eigenschaft         | Typ                                                     | Erforderlich                 | Wert |
|:-----------------|:---------------------------------------------------------|:-------------------------|:--|
| resourceId       | String                                                   | Ja                      | \<resourceId\> |
| roleDefinitionId | Zeichenfolge                                                   | Ja                      | \<roleDefinitionId\> |
| subjectId        | Zeichenfolge                                                   | Ja                      | \<subjectId\> |
| assignmentState  | Zeichenfolge                                                   | Ja                      | Aktiv |
| type             | Zeichenfolge                                                   | Ja                      | UserAdd |
| Grund           | Zeichenfolge                                                   | hängt von der Rolle Einstellungen |   |
| Zeitplan         | [governanceSchedule](../resources/governanceschedule.md) | Ja                      |   |

#### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserAdd",
  "reason": "Activate the owner role",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "duration": "PT9H"
  },
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394"
}
```

#### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "3ad49a7c-918e-4d86-9f84-fab28f8658c0",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "8b4d1d51-08e9-4254-b0a6-b16177aae376",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "linkedEligibleRoleAssignmentId": "e327f4be-42a0-47a2-8579-0a39b025b394",
  "type": "UserAdd",
  "assignmentState": "Active",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "Activate the owner role",
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "EligibilityRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      },
      {
        "key": "JustificationRule",
        "value": "Grant"
      },
      {
        "key": "ActivationDayRule",
        "value": "Grant"
      },
      {
        "key": "ApprovalRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:28:43.537Z",
    "endDateTime": "0001-01-01T00:00:00Z",
    "duration": "PT9H"
  }
}
```

### <a name="example-3-user-deactivates-an-assigned-role"></a>Beispiel 3: Benutzer deaktiviert zugewiesene Rolle

In diesem Beispiel deaktiviert die nawu@fimdev.net Benutzer die aktive Abrechnung Reader-Rolle.

| Eigenschaft         | Typ                                                     | Erforderlich | Wert |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| resourceId       | String                                                   | Ja      | \<resourceId\> |
| roleDefinitionId | Zeichenfolge                                                   | Ja      | \<roleDefinitionId\> |
| subjectId        | Zeichenfolge                                                   | Ja      | \<subjectId\> |
| assignmentState  | Zeichenfolge                                                   | Ja      | Aktiv |
| type             | Zeichenfolge                                                   | Ja      | UserRemove |
| Grund           | Zeichenfolge                                                   | Nein       |   |
| Zeitplan         | [governanceSchedule](../resources/governanceschedule.md) | Nein       |   |

#### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "assignmentState": "Active",
  "type": "UserRemove",
  "reason": "Deactivate the role",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec"
}
```

#### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "abfcdb57-8e5d-42a0-ae67-7598b96fddb1",
  "resourceId": "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735",
  "roleDefinitionId": "bc75b4e6-7403-4243-bf2f-d1f6990be122",
  "subjectId": "918e54be-12c4-4f4c-a6d3-2ee0e3661c51",
  "linkedEligibleRoleAssignmentId": "cb8a533e-02d5-42ad-8499-916b1e4822ec",
  "type": "UserRemove",
  "assignmentState": "Active",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "Evaluate only",
  "schedule": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  }
}
```

### <a name="example-4-administrator-removes-user-from-a-role"></a>Beispiel 4: Administrator entfernt Benutzer aus einer Rolle

In diesem Beispiel entfernt ein Administrator die nawu@fimdev.net Benutzer aus der Abrechnung Reader-Rolle.

 >**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.

| Eigenschaft         | Typ                                                     | Erforderlich | Wert |
|:-----------------|:---------------------------------------------------------|:---------|:--|
| resourceId       | String                                                   | Ja      | \<resourceId\> |
| roleDefinitionId | String                                                   | Ja      | \<roleDefinitionId\> |
| subjectId        | String                                                   | Ja      | \<subjectId\> |
| assignmentState  | String                                                   | Ja      | Berechtigte / Active |
| type             | Zeichenfolge                                                   | Ja      | AdminRemove |
| Grund           | Zeichenfolge                                                   | Nein       |   |
| Zeitplan         | [governanceSchedule](../resources/governanceschedule.md) | Nein       |   |

#### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminRemove"
}
```

#### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "c934fcb9-cf53-42ac-a8b4-6246f6726299",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "65bb4622-61f5-4f25-9d75-d0e20cf92019",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminRemove",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "Closed",
    "subStatus": "Revoked",
    "statusDetails": []
  },
  "schedule": null
}
```

### <a name="example-5-administrator-updates-role-assignment"></a>Beispiel 5: Administrator aktualisiert rollenzuweisung

In diesem Beispiel aktualisieren Administratoren die rollenzuweisung für den Benutzer nawu@fimdev.net Besitzer.

 >**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.

| Eigenschaft         | Typ                                                     | Erforderlich                | Wert |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| resourceId       | String                                                   | Ja                     | \<resourceId\> |
| roleDefinitionId | String                                                   | Ja                     | \<roleDefinitionId\> |
| subjectId        | String                                                   | Ja                     | \<subjectId\> |
| assignmentState  | String                                                   | Ja                     | Berechtigte / Active |
| type             | Zeichenfolge                                                   | Ja                     | AdminUpdate |
| Grund           | Zeichenfolge                                                   | hängt von roleSettings |   |
| Zeitplan         | [governanceSchedule](../resources/governanceschedule.md) | Ja                     |   |

#### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "assignmentState": "Eligible",
  "type": "AdminUpdate",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31.000Z"
  }
}
```

#### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "4f6d4802-b3ac-4f5a-86d7-a6a4edd7d383",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "70521f3e-3b95-4e51-b4d2-a2f485b02103",
  "subjectId": "1566d11d-d2b6-444a-a8de-28698682c445",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminUpdate",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": null,
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "AdminRequestRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-03-08T05:42:45.317Z",
    "endDateTime": "2018-06-05T05:42:31Z",
    "duration": "PT0S"
  }
}
```

### <a name="example-6-administrator-extends-expiring-role-assignment"></a>Beispiel 6: Administrator erweitert ablaufende rollenzuweisung

In diesem Beispiel wird erweitert die ablaufende rollenzuweisung für Benutzer ANUJCUSER API Management Service Mitwirkenden.

 >**Hinweis:** Neben der Berechtigung, dieses Beispiel erfordert, dass die anfordernde Person mindestens eine `Active` Administrator rollenzuweisung (`owner` oder `user access administrator`) für die Ressource.

| Eigenschaft         | Typ                                                     | Erforderlich                | Wert |
|:-----------------|:---------------------------------------------------------|:------------------------|:--|
| resourceId       | String                                                   | Ja                     | \<resourceId\> |
| roleDefinitionId | String                                                   | Ja                     | \<roleDefinitionId\> |
| subjectId        | String                                                   | Ja                     | \<subjectId\> |
| assignmentState  | Zeichenfolge                                                   | Ja                     | Berechtigte / Active |
| type             | Zeichenfolge                                                   | Ja                     | AdminExtend |
| Grund           | Zeichenfolge                                                   | hängt von roleSettings |   |
| Zeitplan         | [governanceSchedule](../resources/governanceschedule.md) | Ja                     |   |

#### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "governanceroleassignmentrequest_post"
}-->

```http
POST https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleAssignmentRequests
Content-type: application/json

{
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "assignmentState": "Eligible",
  "type": "AdminExtend",
  "reason": "extend role assignment",
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z"
  }
}
```

#### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequest"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#governanceRoleAssignmentRequests/$entity",
  "id": "486f0c05-47c8-4498-9c06-086a78c83004",
  "resourceId": "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  "roleDefinitionId": "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  "subjectId": "74765671-9ca4-40d7-9e36-2f4a570608a6",
  "linkedEligibleRoleAssignmentId": "",
  "type": "AdminExtend",
  "assignmentState": "Eligible",
  "requestedDateTime": "0001-01-01T00:00:00Z",
  "reason": "extend role assignment",
  "status": {
    "status": "InProgress",
    "subStatus": "Granted",
    "statusDetails": [
      {
        "key": "AdminRequestRule",
        "value": "Grant"
      },
      {
        "key": "ExpirationRule",
        "value": "Grant"
      },
      {
        "key": "MfaRule",
        "value": "Grant"
      }
    ]
  },
  "schedule": {
    "type": "Once",
    "startDateTime": "2018-05-12T23:53:55.327Z",
    "endDateTime": "2018-08-10T23:53:55.327Z",
    "duration": "PT0S"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Post roleAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/governanceroleassignmentrequest-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
