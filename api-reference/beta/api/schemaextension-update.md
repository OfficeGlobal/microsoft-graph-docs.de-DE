---
title: schemaExtension aktualisieren
description: Dient zum Aktualisieren der Eigenschaften in der Definition der angegebenen schemaExtension.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: f457609af15716ef2ada3945132afd285fd2394c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515538"
---
# <a name="update-schemaextension"></a>schemaExtension aktualisieren

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Dient zum Aktualisieren der Eigenschaften in der Definition der angegebenen [schemaExtension](../resources/schemaextension.md).

Die Aktualisierung gilt für alle Ressourcen, die in der Eigenschaft **targetTypes** der Erweiterung enthalten sind. Diese Ressourcen gehören zu den [unterstützenden Ressourcentypen](/graph/extensibility-overview#supported-resources).

Nur die App, mit der eine Schemaerweiterung erstellt wurde (Besitzer-App), kann additive Aktualisierungen an der Erweiterung vornehmen, wenn die Erweiterung den Status **InDevelopment** oder **Available** aufweist. Dies bedeutet, dass die App keine benutzerdefinierten Eigenschaften oder Zielressourcentypen aus der Definition entfernen kann. Die App kann jedoch die Beschreibung der Erweiterung ändern.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).


|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | Directory.AccessAsUser.All    |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a>Optionale Anforderungsheader

| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Content-Type   | application/json |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.

| Eigenschaft   | Typ |Beschreibung|
|:---------------|:--------|:----------|
|description|String|Beschreibung für die Schemaerweiterung.|
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md)-Sammlung|Die Sammlung von Eigenschaftennamen und Typen, die die Schemaerweiterungsdefinition bilden. Nur additive Änderungen sind zulässig. |
|status|String|Der Lebenszyklusstatus der Schemaerweiterung. Der Anfangszustand erstellt worden ist **InDevelopment**. Möglichen Zuständen Übergänge liegen **InDevelopment** bis **verfügbar** und **veraltet** **verfügbar** .|
|targetTypes|String collection|Satz von Microsoft Graph-Typen (die Erweiterungen unterstützen können), auf die die Schemaerweiterung angewendet werden kann.  Nur additive Änderungen sind zulässig.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request"></a>Anforderung

<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```

##### <a name="response"></a>Antwort

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schemaextension-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
