---
title: schemaExtension erstellen
description: Erstellen Sie eine neue schemaExtension-Definition, um einen unterstützenden Ressourcentyp zu erweitern.
localization_priority: Normal
ms.openlocfilehash: 4d351565d697e1e9c399dcabd0d03a701cac2e81
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826390"
---
# <a name="create-schemaextension"></a>schemaExtension erstellen

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Erstellen Sie eine neue [schemaExtension](../resources/schemaextension.md)-Definition, um einen [unterstützenden Ressourcentyp](/graph/extensibility-overview#supported-resources) zu erweitern.

Mit Schemaerweiterungen können Sie stark typisierte benutzerdefinierte Daten zu einer Ressource hinzufügen. Die App, die eine Schemaerweiterung erstellt, ist die Besitzer-App. Abhängig vom [Status](/graph/extensibility-overview#schema-extensions-lifecycle) der Erweiterung kann die Besitzer-App, und nur die Besitzer-App, die Erweiterung aktualisieren oder löschen. 

Erfahren Sie anhand von Beispielen, wie Sie [eine Schemaerweiterung definieren, die einen Schulungskurs beschreibt](/graph/extensibility-schema-groups#2-register-a-schema-extension-definition-that-describes-a-training-course), die Schemaerweiterungsdefinition zum [Erstellen einer neuen Gruppe mit Schulungskursdaten](/graph/extensibility-schema-groups#3-create-a-new-group-with-extended-data) verwenden und [Schulungskursdaten zu einer vorhandenen Gruppe hinzufügen](/graph/extensibility-schema-groups#4-add-update-or-remove-custom-data-in-an-existing-group).

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
POST /schemaExtensions
```

## <a name="request-headers"></a>Anforderungsheader
| Name       | Beschreibung|
|:---------------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Anforderungstext
Geben Sie im Anforderungstext eine JSON-Darstellung eines [schemaExtension](../resources/schemaextension.md)-Objekts an.

In der folgenden Tabelle werden die Eigenschaften gezeigt, die beim Erstellen einer Erweiterungs Schema verfügbar sind.

| Parameter | Typ | Beschreibung|
|:---------------|:--------|:----------|
|description|String|Beschreibung für die Schemaerweiterung.|
|id|String|Der eindeutige Bezeichner für die Schemaerweiterungsdefinition. <br>Sie können einen Wert mit einer von zwei Methoden zuweisen: <ul><li>Verketten Sie den Namen einer Ihrer überprüften Domänen mit einem Namen für die Schemaerweiterung, um eine eindeutige Zeichenfolge in diesem Format zu bilden: \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}. Beispiel: `contoso_mySchema`. HINWEIS: Nur überprüfte Domänen unter den folgenden Domänen auf oberster Eben werden unterstützt: `.com`,`.net`, `.gov`, `.edu` oder `.org`. </li><li>Geben Sie einen Schemanamen an, und verwenden Sie diesen Schemanamen in Microsoft Graph zum Vervollständigen der **id**-Zuweisung in diesem Format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Zum Beispiel: `extkvbmkofy_mySchema`.</li></ul>Diese Eigenschaft kann nach dem Erstellen nicht mehr geändert werden. |
|owner|Zeichenfolge|(Optional) Die `appId` der Anwendung, die der Besitzer der Schemaerweiterung ist. Diese Eigenschaft kann bei der Erstellung bereitgestellt werden, um den Besitzer anzugeben.  Wird Sie nicht bereitgestellt, wird die `appId` der aufrufenden Anwendung als Besitzer festgelegt. Wenn Sie z. B. eine neue Definition für eine Schemaerweiterung mit dem Graph-Tester erstellen, **müssen** Sie die Besitzereigenschaft angeben. Wurde diese Eigenschaft einmal festgelegt, ist sie schreibgeschützt und kann nicht geändert werden.|
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md)-Sammlung|Die Sammlung von Eigenschaftennamen und Typen, die die Schemaerweiterungsdefinition bilden.|
|targetTypes|String-Sammlung|Ein Satz von Microsoft Graph-Ressourcentypen (die Erweiterungen unterstützen), auf die diese Schemaerweiterungsdefinition angewendet werden kann.|

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [schemaExtension](../resources/schemaextension.md)-Objekt im Antworttext zurückgegeben.

## <a name="example"></a>Beispiel

##### <a name="request-1"></a>Anforderung 1

Im ersten Beispiel wird veranschaulicht, wie aus einem überprüften Domänennamen, `graphlearn`, und einem Schemanamen, `courses`, eine eindeutige Zeichenfolge für die **id**-Eigenschaft der Schemaerweiterungsdefinition gebildet wird. Die eindeutige Zeichenfolge basiert auf diesem Format: \{_&#65279;domainName_\}\_\{_&#65279;schemaName_\}.

Geben Sie im Anforderungstext eine JSON-Darstellung des [schemaExtension](../resources/schemaextension.md)-Objekts an.
<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_1"
}-->
```http
POST https://graph.microsoft.com/beta/schemaExtensions
Content-type: application/json

{
    "id":"graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="response-1"></a>Antwort 1

Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="request-2"></a>Anforderung 2

Im zweiten Beispiel wird lediglich ein Schemaname, `courses`, in der **id**-Eigenschaft in der Anforderung angegeben, zusammen mit der JSON-Darstellung der restlichen Eigenschaften im [schemaExtension](../resources/schemaextension.md)-Objekt. Microsoft Graph weist einen eindeutigen Zeichenfolgenwert zu und gibt ihn in der Antwort zurück.

<!-- {
  "blockType": "request",
  "name": "create_schemaextension_from_schemaextensions_2"
}-->
```http
POST https://graph.microsoft.com/beta/schemaExtensions
Content-type: application/json

{
    "id":"courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

##### <a name="response-2"></a>Antwort 2

Die Antwort enthält eine eindeutige Zeichenfolge in der **id**-Eigenschaft, die auf dem in der Anforderung angegebenen Schemanamen zusammen mit dem Rest der neu erstellten Schemadefinition basiert. Der Wert der **id**-Eigenschaft der Antwort basiert auf diesem Format: ext\{_&#65279;8-random-alphanumeric-chars_\}\_\{_&#65279;schema-name_\}. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 420

{
    "id": "extk9eruy7c_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "String"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```


## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](/graph/extensibility-overview)
- [Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create schemaExtension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
