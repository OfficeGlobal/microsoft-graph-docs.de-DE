---
title: Liste directoryAudits
description: Enthält eine Liste der Überwachungsprotokolle von Azure Active Directory generiert. Durch verschiedene Dienste innerhalb von Azure Active Directory wie Benutzer, App, Gerät und Verwaltung von Gruppen, privilegierten Identity Management, Access Bewertungen, rechtlichen Hinweise, Schutz, Kennwortverwaltung (SSPR und Admin das Zurücksetzen von Kennwörtern generiert Überwachungsprotokolle enthält ), Self-service Gruppe Management usw....
localization_priority: Priority
ms.openlocfilehash: 08b9cd5ded6771883a6d0f1129cf44a808515f8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829337"
---
# <a name="list-directoryaudits"></a>Liste directoryAudits

Enthält eine Liste der Überwachungsprotokolle von Azure Active Directory generiert. Durch verschiedene Dienste innerhalb von Azure Active Directory wie Benutzer, App, Gerät und Verwaltung von Gruppen, privilegierten Identity Management, Access Bewertungen, rechtlichen Hinweise, Schutz, Kennwortverwaltung (SSPR und Admin das Zurücksetzen von Kennwörtern generiert Überwachungsprotokolle enthält ), Self-service Gruppe Management usw....

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | AuditLog.Read.All |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt   |
|Anwendung | AuditLog.Read.All | 

Darüber hinaus müssen apps Azure AD [ordnungsgemäß registriert](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) sein.

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/directoryAudits
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die folgende OData-Abfrageparameter zur Anpassung der Antwort. Überprüfen Sie die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) dafür, wie diese Parameter zu verwenden.

|Name     |Beschreibung                            |Beispiel|
|:--------------------|----------------|------------------------------------------------------------------------|
|[$filter](/graph/query-parameters#filter-parameter)|Dient zum Filtern von Ergebnissen (Zeilen). |/`auditLogs/directoryAudits?&$filter=createdDateTime le 2018-01-24`
|[$top](/graph/query-parameters#top-parameter)|Dient zum Festlegen der Seitengröße von Ergebnissen.|`/auditLogs/directoryAudits?$top=1`|
|[$skiptoken](/graph/query-parameters#skiptoken-parameter)|Ruft ab, das die nächste Seite mit Ergebnissen aus Ergebnis, die festgelegt über mehrere Seiten erstrecken.|`auditLogs/directoryAudits?$skiptoken=01fa0e77c60c2d3d63226c8e3294c860__1`|

### <a name="list-of-attributes-supported-by-filter-parameter"></a>Liste der Attribute von $filter Parameter unterstützt werden
|Name des Attributs |Unterstützte Operatoren|
|:----------------|:------|
|activityDisplayName| EQ startswith|
|activityDateTime| EQ, ge, le|
|loggedByService|eq|
|InitiatedBy/Mitgliedsname|eq|
|InitiatedBy/Benutzer/displayName| eq|
|InitiatedBy/Benutzer/userPrincipalName| EQ startswith|
|InitiatedBy/app/appId| eq|
|InitiatedBy/app/appDisplayName| eq|
|TargetResources/any(t: t/id)| eq|
|targetResources/any(t:t/displayName)| EQ startswith|
## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {code}|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response"></a>Antwort
Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [DirectoryAudit](../resources/directoryaudit.md) .
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
            "@odata.type": "#microsoft.graph.TargetResourceGroup",
            "id": "ef7x527d-6x92-42x4-8x6d-cfxfdfx57f95",
            "displayName": "Lynda.com",
            "modifiedProperties": [{
                "displayName": "Action Client Name",
                "oldValue": null,
                "newValue": "DirectorySync"
            }],
            "groupType": "unifiedGroups"
        }, {
            "@odata.type": "#microsoft.graph.targetResourceUser",
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
