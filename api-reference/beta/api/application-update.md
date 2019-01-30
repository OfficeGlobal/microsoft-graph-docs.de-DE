---
title: Update application
description: Aktualisieren Sie die Eigenschaften des Application-Objekts.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 335281a0ac37ae3b966f731112223f019a67437d
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642828"
---
# <a name="update-application"></a>Update application

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren Sie die Eigenschaften des Application-Objekts.
## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) |  Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a>Anforderungsheader
| Name       | Typ | Beschreibung|
|:-----------|:------|:----------|
| Autorisierung  | string  | Bearer {token}. Erforderlich.  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|allowPublicClient|Boolean| Gibt an, ob die Anwendung als öffentliche Client fungieren kann. Beispielsweise eine installierte Anwendung, die auf einem mobilen Gerät ausgeführt. Der Standardwert lautet *false*. |
|api|[api](../resources/api.md)| Legt die Einstellungen für eine API-Anwendung fest. |
|appRoles|[appRole](../resources/approle.md)-Sammlung|Die Sammlung der Anwendungsrollen, die eine Anwendung möglicherweise deklariert. Diese Rollen können Benutzern, Gruppen oder Dienstprinzipalen zugewiesen werden. Lässt keine Nullwerte zu.|
|applicationAliases|String-Sammlung| Die URIs, die die Anwendung identifizieren. Weitere Informationen finden Sie unter [Anwendungsobjekte und Dienstprinzipalobjekte](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/). Der *any*-Operator ist für Filterausdrücke für mehrwertige Eigenschaften erforderlich. Lässt keine Nullwerte zu. |
|createdDateTime|DateTimeOffset| Datum und Uhrzeit der Anwendungsregistrierung. |
|deletedDateTime|DateTimeOffset| Datum und Uhrzeit der Anwendungslöschung. |
|displayName|String|Der Anzeigename der Anwendung. |
|id|String|Eindeutiger Bezeichner für die Anwendung. Geerbt von [directoryObject](../resources/directoryobject.md). Key. Lässt keine Nullwerte zu. Schreibgeschützt. |
|info|[informationalUrl](../resources/informationalurl.md)| Grundlegende Profilinformationen der Anwendung. | Legt die Einstellungen für installierte Clients wie Desktop- oder mobile Geräte fest. |
|keyCredentials|[keyCredential](../resources/keycredential.md)-Sammlung|Die Sammlung der wichtigsten Anmeldeinformationen, die mit der Anwendung verknüpft sind. Lässt keine Nullwerte zu. |
|logo|Stream|Das Hauptlogo für die Anwendung. Lässt keine Nullwerte zu. |
|orgRestrictions|String-Sammlung| Die Organisationseinheit TenantIds, die die Anwendung beschränkt ist.  Wenn die Auflistung leer ist, ist die Anwendung mit mehreren Mandanten (nicht eingeschränkt). Wenn die Auflistung TenantIds enthält, ist die Anwendung auf die Organisationseinheit TenantIds in der Auflistung beschränkt. Angeben von anderen Mandanten, aber nicht die TenantId, in dem die Anwendung registriert ist, impliziert, dass die TenantId der Anwendung indirekt enthalten ist. |
|passwordCredentials|[passwordCredential](../resources/passwordcredential.md)-Sammlung|Die Sammlung der Kennwortanmeldeinformationen, die mit der Anwendung verknüpft sind. Lässt keine Nullwerte zu.|
|preAuthorizedApplications|[PreAuthorizedApplication](../resources/preauthorizedapplication.md) -Auflistung| Listen-Anwendungen und angeforderten Berechtigungen für implizite Zustimmung. Erfordert ein Administrator Zustimmung an die Anwendung bereitgestellt haben. PreAuthorizedApplications erfordern keinen den Benutzer, die angeforderten Berechtigungen zuzustimmen. In PreAuthorizedApplications aufgelisteten Berechtigungen erfordern keine Zustimmung des Benutzers. Keine weiteren angeforderten Berechtigungen nicht in PreAuthorizedApplications aufgeführten erfordern jedoch Zustimmung des Benutzers. |
|requiredResourceAccess|[requiredResourceAccess](../resources/requiredresourceaccess.md)-Sammlung|Gibt Ressourcen an, auf die diese Anwendung zugreifen muss, sowie den Satz von OAuth-Berechtigungsbereichen und Anwendungsrollen, die unter den jeweiligen Ressourcen benötigt werden. Durch diese Vorkonfiguration des erforderlichen Ressourcenzugriffs wird die Zustimmungsoberfläche bestimmt. Lässt keine Nullwerte zu.|
|tags|String-Sammlung| Benutzerdefinierte Zeichenfolgen, die zum Kategorisieren und Identifizieren der Anwendung verwendet werden können. |
|web|[web](../resources/web.md)| Legt die Einstellungen für eine Webanwendung fest. |

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
