---
title: schemaExtensions auflisten
description: 'Abrufen einer Liste von SchemaExtension-Objekten erstellt mithilfe von apps, die Sie in den aktuellen Mandanten besitzen (das werden kann '
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: a320cc0261c40ee8b87dcc658c6ca146d77190e6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529159"
---
# <a name="list-schemaextensions"></a>schemaExtensions auflisten

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Dient zum Abrufen einer Liste von [schemaExtension](../resources/schemaextension.md)-Objekten, die von beliebigen Apps erstellt wurden, die Sie im aktuellen Mandanten besitzen (kann **InDevelopment**, **Available** oder **Deprecated** sein), sowie aller anderen Schemaerweiterungen im Besitz von anderen Apps, die als **Available** gekennzeichnet sind. 

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.Read.All, Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Directory.Read.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /schemaExtensions
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.

## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Content-Type   | application/json |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [schemaExtension](../resources/schemaextension.md)-Objekten im Antworttext zurückgegeben.
## <a name="example"></a>Beispiel
##### <a name="request"></a>Anforderung
Im folgenden Beispiel wird gezeigt, wie Sie unter allen zugänglichen Erweiterungen nach einer bestimmten Erweiterung suchen, indem Sie nach ihrer eindeutigen **ID** filtern. 
<!-- {
  "blockType": "request",
  "name": "get_schemaextensions"
}-->
```http
GET https://graph.microsoft.com/beta/schemaExtensions?$filter=id%20eq%20'graphlearn_test'
```
##### <a name="response"></a>Antwort
Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 274

{
  "value": [
    {
      "id":"graphlearn_test",
      "description": "Yet another test schema",
      "targetTypes": [
          "User", "Group"
      ],
      "status": "InDevelopment",
      "owner": "24d3b144-21ae-4080-943f-7067b395b913",
      "properties": [
          {
              "name": "testName",
              "type": "String"
          }
      ]
    }
  ]
}
```

## <a name="see-also"></a>Siehe auch

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List schemaExtensions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
