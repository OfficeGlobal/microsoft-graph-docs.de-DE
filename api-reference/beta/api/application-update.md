---
title: Aktualisieren der Anwendung
description: Aktualisieren Sie die Eigenschaften des Application-Objekts.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9965a46e340063940e1a9af18a89ada7e492bf26
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572213"
---
# <a name="update-application"></a>Aktualisieren der Anwendung

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie die Eigenschaften des Application-Objekts.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Application.ReadWrite.OwnedBy Application.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowPublicClient|Boolean| Gibt an, ob die Anwendung als öffentliche Client fungieren kann. Beispielsweise eine installierte Anwendung, die auf einem mobilen Gerät ausgeführt. Der Standardwert lautet *false*. |
|API|[API](../resources/api.md)| Gibt die Einstellungen für eine API-Anwendung. |
|appRoles|[AppRole](../resources/approle.md) -Auflistung|Die Auflistung der Anwendungsrollen, die eine Anwendung deklarieren kann. Diese Funktionen können Benutzer, Gruppen oder Dienstprinzipale zugewiesen werden. Lässt keine NULL-Werte zu.|
|applicationAliases|Zeichenfolgenauflistung| Die URIs, die die Anwendung zu bestimmen. Weitere Informationen finden Sie unter [Application Objects und Service Principal-Objekte](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). Der *any*-Operator ist für Filterausdrücke für mehrwertige Eigenschaften erforderlich. Lässt keine NULL-Werte zu. |
|createdDateTime|DateTimeOffset| Das Datum und die Zeit, die die Anwendung registriert wurde. |
|deletedDateTime|DateTimeOffset| Das Datum und die Zeit, die die Anwendung gelöscht wurde. |
|displayName|String|Der Anzeigename für die Anwendung. |
|id|String|Der eindeutige Bezeichner für die Anwendung. Geerbt von [directoryObject](../resources/directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt. |
|Info|[informationalUrl](../resources/informationalurl.md)| Grundlegende Profilinformationen der Anwendung. | Gibt die Einstellungen für installierte Clients wie desktop oder mobilen Geräten. |
|keyCredentials|[KeyCredential](../resources/keycredential.md) -Auflistung|Die Auflistung der wichtigsten Anmeldeinformationen der Anwendung nicht zugeordnete NULL-Werte zulässt. |
|logo|Stream|Das Hauptfenster Logo für die Anwendung. Lässt keine NULL-Werte zu. |
|orgRestrictions|Zeichenfolgenauflistung| Die Organisationseinheit TenantIds, die die Anwendung beschränkt ist.  Wenn die Auflistung leer ist, ist die Anwendung mit mehreren Mandanten (nicht eingeschränkt). Wenn die Auflistung TenantIds enthält, ist die Anwendung auf die Organisationseinheit TenantIds in der Auflistung beschränkt. Angeben von anderen Mandanten, aber nicht die TenantId, in dem die Anwendung registriert ist, impliziert, dass die TenantId der Anwendung indirekt enthalten ist. |
|passwordCredentials|[PasswordCredential](../resources/passwordcredential.md) -Auflistung|Die Auflistung von Anmeldeinformationen, die mit der Anwendung verbunden sind. Lässt keine NULL-Werte zu.|
|preAuthorizedApplications|[PreAuthorizedApplication](../resources/preauthorizedapplication.md) -Auflistung| Listen-Anwendungen und angeforderten Berechtigungen für implizite Zustimmung. Erfordert ein Administrator Zustimmung an die Anwendung bereitgestellt haben. PreAuthorizedApplications erfordern keinen den Benutzer, die angeforderten Berechtigungen zuzustimmen. In PreAuthorizedApplications aufgelisteten Berechtigungen erfordern keine Zustimmung des Benutzers. Keine weiteren angeforderten Berechtigungen nicht in PreAuthorizedApplications aufgeführten erfordern jedoch Zustimmung des Benutzers. |
|requiredResourceAccess|[RequiredResourceAccess](../resources/requiredresourceaccess.md) -Auflistung|Gibt die Ressourcen, die diese Anwendung benötigt Zugriff auf und den Satz von OAuth berechtigungsbereiche und Anwendungsrollen, die unter jeder dieser Ressourcen benötigt werden. Diese vor Konfiguration erforderlichen Ressourcenzugriff Laufwerke der Zustimmung wünschen. Lässt keine NULL-Werte zu.|
|tags|Zeichenfolgenauflistung| Benutzerdefinierte Zeichenfolgen, die zum Kategorisieren und Identifizieren der Anwendung verwendet werden können. |
|web|[webApplication](../resources/web.md)| Gibt die Einstellungen für eine Webanwendung. |

## <a name="response"></a>Antwort

Wenn erfolgreich ist, diese Methode gibt einen `204 No Content` Antwortcode und kein Suchzeichenfolge im Antworttext zurückgegeben wird.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json
Content-length: 72

{
  "allowPublicClient": false,
  "displayName": "New display name"
}
```
##### <a name="response"></a>Antwort
Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
