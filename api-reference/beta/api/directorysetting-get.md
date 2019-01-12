---
title: Eine Einstellung für die Directory abrufen
description: Rufen Sie die Eigenschaften eines bestimmten Verzeichnis Einstellung-Objekts ab.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 73953ccedeb7ecaeeba5cb68e6827956430ada82
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950823"
---
# <a name="get-a-directory-setting"></a>Eine Einstellung für die Directory abrufen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Rufen Sie die Eigenschaften eines bestimmten Verzeichnis Einstellung-Objekts ab.

> **Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird. Die /v1.0 Version dieser API wurde zum *Abrufen von GroupSettings*umbenannt.

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Directory.Read.All, Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->Abrufen einer bestimmten Mandanten geltende oder gruppeneinstellung
```http
GET /settings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich.|

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode eine `200 OK` Code und [Verzeichnisberechtigungen](../resources/directorysetting.md) Antwortobjekt im Antworttext.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Nachfolgend sehen Sie ein Beispiel der Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_directorysetting"
}-->
```http
GET https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 198

{
  "id": "id-value",
  "displayName": "displayName-value",
  "settingTemplateId": "settingTemplateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
