---
title: List directoryAudits
description: Stellt die Liste der von Azure Active Directory generierten Überwachungsprotokolle bereit. Enthält Überwachungsprotokolle, die von verschiedenen Diensten innerhalb von Azure Active Directory generiert werden, z. B. Benutzer-, App-, Geräte- und Gruppenverwaltung, Privileged Identity Management, Zugriffsüberprüfungen, Nutzungsbedingungen, Identity Protection, Kennwortverwaltung (SSPR- und Administratorkennwortzurücksetzungen), Self-Service-Gruppenverwaltung usw.
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f9330cd8ca1bd2b17755ffd1e09fee7743355b2
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576682"
---
# <a name="list-directoryaudits"></a>List directoryAudits

Stellt die Liste der von Azure Active Directory generierten Überwachungsprotokolle bereit. Enthält Überwachungsprotokolle, die von verschiedenen Diensten innerhalb von Azure Active Directory generiert werden, z. B. Benutzer-, App-, Geräte- und Gruppenverwaltung, Privileged Identity Management, Zugriffsüberprüfungen, Nutzungsbedingungen, Identity Protection, Kennwortverwaltung (SSPR- und Administratorkennwortzurücksetzungen), Self-Service-Gruppenverwaltung usw.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | AuditLog.Read.All |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt   |
|Anwendung | AuditLog.Read.All | 

Darüber hinaus müssen Apps bei Azure AD [ordnungsgemäß registriert](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) sein.

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die folgende OData-Abfrageparameter zur Anpassung der Antwort. Wenn Sie wissen möchten, wie diese Parameter verwendet werden, finden Sie weitere Informationen unter [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters).

|Name     |Beschreibung                            |Beispiel|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](/graph/query-parameters#filter-parameter)|Dient zum Filtern von Ergebnissen (Zeilen). |/`auditLogs/directoryAudits?&$filter=createdDateTime le 2018-01-24`
|[$top](/graph/query-parameters#top-parameter)|Dient zum Festlegen der Seitengröße von Ergebnissen.|`/auditLogs/directoryAudits?$top=1`|
|[$skiptoken](/graph/query-parameters#skiptoken-parameter)|Dient zum Abrufen der nächsten Seite von Ergebnissen aus Resultsets, die mehrere Seiten umfassen.|`auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a>Liste der Attribute, die durch den Parameter "$filter" unterstützt werden
|Attributname |Unterstützte Operatoren|
|:----------------|:------|
|activityDisplayName| eq, startswith|
|activityDateTime| eq, ge, le|
|loggedByService|eq|
|initiatedBy/user/id|eq|
|initiatedBy/user/displayName| eq|
|initiatedBy/user/userPrincipalName| eq, startswith|
|initiatedBy/app/appId| eq|
|initiatedBy/app/appDisplayName| eq|
|targetResources/any(t: t/id)| eq|
|targetResources/any(t:t/displayName)| eq, startswith|
## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response"></a>Antwort
Bei Erfolg gibt diese Methode den Antwortcode `200 OK` und eine Sammlung von [directoryAudit](../resources/directoryaudit.md)-Objekten im Antworttext zurück.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_directoryaudits"
}-->
```http
GET https://graph.microsoft.com/beta/auditLogs/directoryAudits
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryAudit",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 271
```
```json
{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/directoryAudits
  "value": [{
        "id": "id",
        "category": "UserManagement",
        "correlationId": "da159bfb-54fa-4092-8a38-6e1fa7870e30",
        "result": "success",
        "resultReason": "Successfully added member to group",
        "activityDisplayName": "Add member to group",
        "activityDateTime": "2018-01-09T21:20:02.7215374Z",
        "loggedByService": "Core Directory",
        "initiatedBy": {
            "user": {
                "id": "7283X9ae-1a37-4937-9aex-e35d964db09b",
                "displayName": "Jamie Doe",
                "userPrincipalName": "jdoe@wingtiptoysonline.com",
                "ipAddress": "127.0.0.1"
            },
            "app": null
        },
        "targetResources": [{
            "@odata.type": "microsoft.graph.TargetResourceGroup",
            "id": "ef7x527d-6x92-42x4-8x6d-cfxfdfx57f95",
            "displayName": "Lynda.com",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync"
            }],
            "groupType": "unifiedGroups"
        }, {
            "@odata.type": "microsoft.graph.targetResourceUser",
            "id": "1f0ex8f5-3x61-4x6b-9x50-d4xx572f2bb7",
            "displayName": null,
            "modifiedProperties": [],
            "userPrincipalName": "jdoe@contoso.com"
        }],
        "additionalDetails": [{
            "key": "Additional Detail Name",
            "value": "Additional Detail Value"
        }]
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryAudits",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
