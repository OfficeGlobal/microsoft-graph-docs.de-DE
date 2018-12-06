---
title: 'Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen '
description: 'Sie werden durch ein Beispiel geführt, um die Verwendung von *Schemaerweiterungen* zu veranschaulichen. '
ms.openlocfilehash: 098853ffaa5292313c71259e97fb8f1a8063fec4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092225"
---
# <a name="add-custom-data-to-groups-using-schema-extensions"></a>Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen 

Sie werden durch ein Beispiel geführt, um die Verwendung von *Schemaerweiterungen* zu veranschaulichen. 

Angenommen, Sie sind ein Entwickler in einem Unternehmen für Lernverwaltungssoftware mit dem Namen „Graph Learn“, das Schulungskurse und Materialien für Unternehmen erstellt.  Office 365-Gruppen mit ihren vielfältigen Oberflächen für die Zusammenarbeit bieten eine hervorragende Möglichkeit zur Bereitstellung von Kursinhalten und zum Aufzeichnen von Übungen unter Teilnehmern, sowohl für Onlinekurse als auch für Kurse mit Kursleitern.  Es bietet sich an, die Office 365-Gruppen, die für Schulungskurse verwendet werden, leicht erkennbar zu gestalten, sodass andere Entwickler Ihre Gruppen auffinden und vielfältige Oberflächen zusätzlich zu Ihren Lernkursen erstellen können.

In diesem Szenario erlernen Sie Folgendes:

1. Anzeigen verfügbarer Schemaerweiterungsdefinitionen, die Sie verwenden können
2. Registrieren einer Schemaerweiterungsdefinition, die auf Gruppen für Schulungskurse abzielt
3. Erstellen einer neuen Gruppe mit erweiterten Daten basierend auf der Schemaerweiterungsdefinition, die Sie soeben registriert haben
4. Hinzufügen, Aktualisieren oder Entfernen von benutzerdefinierten Daten in einer vorhandenen Gruppe basierend auf einer Schemaerweiterungsdefinition
5. Einlesen einer Gruppe und der Erweiterungsdaten

>**Hinweis:** In diesem Artikel erfahren Sie, wie Sie Schemaerweiterungswerte in einer **group**-Ressource erstellen und lesen können (Schritte 3 bis 5).  Diese Methoden werden auch von Ressourcen des Typs **administrativeUnit**, **device**, **event**, **message**, **organization**, **post** und **user** unterstützt.  Sie können also auf jede dieser Ressourcen ähnliche Vorgänge wie die unten beschriebenen Beispielanforderungen anwenden. Beachten Sie, dass  **administrativeUnit** nur im Beta-Endpunkt verfügbar ist.

## <a name="1-view-available-schema-extensions"></a>1. Anzeigen verfügbarer Schemaerweiterungen
Als Entwickler möchten Sie wahrscheinlich zuerst prüfen, ob es bereits andere Schemaerweiterungsdefinitionen gibt, die Sie für Ihre App wiederverwenden könnten.  Das können Sie durch Abfragen der Ressource **schemaExtension** tun.  
Im Beispiel unten fragen Sie eine spezifische Schemaerweiterung anhand ihres **id**-Werts ab.

Beachten Sie: Die in der Antwort zurückgegebene Erweiterung hat den **status**-Wert **Available**. Das bedeutet, dass jede App, die zum Zugriff auf die in der Eigenschaft **targetTypes** definierten Ressourcen berechtigt ist, die Erweiterung verwenden und mit additiven Änderungen aktualisieren kann. Im Allgemeinen gibt dieser Vorgang alle Schemaerweiterungen zurück, die dem angegebenen Filter entsprechen, unabhängig von ihrem **status**-Wert. Bevor Sie eine Erweiterung verwenden, sollten Sie also immer ihren Status überprüfen.


##### <a name="request"></a>Anforderung
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id eq 'graphlearn_test'
```
##### <a name="response"></a>Antwort
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420
{
    "value": [
        {
            "id":"graphlearn_test",
            "description": "Yet another test schema",
            "targetTypes": [
                "User", "Group"
            ],
            "status": "Available",
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
## <a name="2-register-a-schema-extension-definition-that-describes-a-training-course"></a>2. Registrieren einer Schemaerweiterungsdefinition, die einen Schulungskurs beschreibt
Wenn Sie keine Schemaerweiterung finden, die ihren Anforderungen *bereits entspricht*, können Sie eine neue Erweiterungsdefinition für Schulungskurse in der **group**-Ressource erstellen und registrieren.  

Beim Erstellen einer Schemaerweiterungsdefinition sollten Sie eine Zeichenfolge für die **id**-Eigenschaft angeben. Sie können auf zwei Arten vorgehen: Das folgende Beispiel zeigt die bevorzugte Methode, die einen Vanity-Domänennamen (`graphlearn.com`) verwendet, der mit Ihrem Mandanten überprüft wurde. Verketten Sie den überprüften Domänennamen (`graphlearn`) mit einem Namen für die Schemaerweiterung (`courses`), und weisen Sie **id** mit der resultierenden Zeichenfolge, `graphlearn_courses`, zu.  

Geben Sie dann eine Beschreibung (zwecks Erkennbarkeit), die Zieltypen (d. h. die Ressourcen, auf die die Erweiterung angewendet werden kann) und die benutzerdefinierten Eigenschaften an, die das Schema bilden sollen.  In diesem Beispiel geben Sie die benutzerdefinierten Eigenschaften `courseId`, `courseName` und `courseType` sowie deren Typen an.

Sehen Sie sich ein [Beispiel für die andere Möglichkeit zum Zuweisen von **id** in der Anforderung](/graph/api/schemaextension-post-schemaextensions?view=graph-rest-1.0#request-2) an, für die nur ein Schemaname angegeben werden muss.

Beachten Sie: Bei der Ersterstellung einer Schemaerweiterung hat diese den Status **InDevelopment**. Sie können die Erweiterung während der weiteren Entwicklung in diesem Status belassen. Dann kann die Erweiterung nur von der App mit additiven Änderungen aktualisiert oder gelöscht werden, von der sie erstellt wurde. Sobald die Erweiterung für andere Apps verfügbar sein soll, können Sie den Wert **status** auf **Available** setzen.

##### <a name="request"></a>Anforderung
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
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
##### <a name="response"></a>Antwort
```http
HTTP/1.1 201 Created
Content-Type: application/json
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

## <a name="3-create-a-new-group-with-extended-data"></a>3. Erstellen einer neuen Gruppe mit erweiterten Daten 
Erstellen Sie eine _neue_ Gruppe, und erweitern Sie sie unter Verwendung der soeben registrierten Schemaerweiterungsdefinition `graphlearn_courses` mit zusätzlichen Daten.  Dies ist ein standardmäßiger ```POST``` für die **group**-Ressource, wobei die zusätzliche Erweiterung `graphlearn_courses` mit komplexem Typ im Anforderungstext definiert ist.  Die Antwort spiegelt keine Datenerweiterungen wider. Für die Erweiterung muss explizit ```$select``` anhand des Namens unter Verwendung eines ```GET```-Vorgangs durchgeführt werden.

##### <a name="request"></a>Anforderung
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
{
    "displayName": "New Managers March 2017",
    "description": "New Managers training course for March 2017",
    "groupTypes": ["Unified"],
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "graphlearn_courses": {
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }
}
```
##### <a name="response"></a>Antwort
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "dfc8016f-db97-4c47-a582-49cb8f849355",
    "createdDateTime": "2017-02-09T00:17:05Z",
    "description": "New Managers training course for March 2017",
    "displayName": "New Managers March 2017",
    "groupTypes": [
        "Unified"
    ],
    "mail": "newMan201703@graphlearn.com",
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```

## <a name="4-add-update-or-remove-custom-data-in-an-existing-group"></a>4. Hinzufügen, Aktualisieren oder Entfernen von benutzerdefinierten Daten in einer vorhandenen Gruppe
Sie können eine _vorhandene_ Gruppeninstanz mit der zusätzlichen Erweiterung `graphlearn_courses` mit komplexem Typ, die im Textkörper einer ```PATCH```-Anforderung definiert ist, erweitern und ihr benutzerdefinierte Daten hinzufügen.  

##### <a name="request"></a>Anforderung
```http
PATCH https://graph.microsoft.com/v1.0/groups/dfc8016f-db97-4c47-a582-49cb8f849355
Content-type: application/json
Content-length: 230
{
    "graphlearn_courses":{
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }   
}
```
##### <a name="response"></a>Antwort
```http
HTTP/1.1 204 No Content
```

Wenn Sie die Werte der Erweiterungsdaten aktualisieren möchten, platzieren Sie die gesamte Erweiterung des komplexen Typs im Textkörper einer ```PATCH```-Anforderung (ähnlich wie das Hinzufügen von benutzerdefinierten Daten zu einer vorhandenen Ressource).

Sie können benutzerdefinierte Daten, die einer Ressourceninstanz hinzugefügt wurden, auch entfernen, indem Sie die entsprechende Erweiterungseigenschaft auf NULL festlegen. 

Um eine Schemaerweiterung aus einer Ressourceninstanz zu entfernen, legen Sie die Erweiterung mit komplexem Typ in der betreffenden Instanz auf NULL fest.


## <a name="5-get-a-group-and-its-extension-data"></a>5. Abrufen einer Gruppe und ihrer Erweiterungsdaten
Eine praktische Möglichkeit zum Suchen nach einer Gruppe (oder Gruppen) ist die Verwendung von `$filter`, um bestimmte Erweiterungseigenschaftswerte abzugleichen, z. B. Erweiterungsname oder -ID. 

Um die benutzerdefinierten Daten in einer Gruppe abzurufen, verwenden Sie dann `$select` zum Einschließen der Erweiterung nach Name (in diesem Fall `graphlearn_courses`).

Im folgenden Beispiel wird nach der Gruppe mit der Erweiterung `graphlearn_courses` gesucht, deren `courseId`-Eigenschaft den Wert `123` hat, und es werden die Gruppeneigenschaften **displayName**, **id** und **description** sowie die benutzerdefinierten Daten in der Erweiterung `graphlearn_courses` abgerufen. (Denken Sie daran, in der tatsächlichen Abfrage URL-Codierung nach Bedarf anzuwenden.)

#### <a name="request"></a>Anforderung

```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


##### <a name="response"></a>Antwort
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
  "value": [
    {
      "displayName": "New Managers March 2017",
      "id": "14429ae5-3e74-41a2-9fa8-028fbb984637",
      "description": "New Managers training course for March 2017",
      "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
      }
    }
  ]
}
```

## <a name="see-also"></a>Weitere Artikel

- [Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen](extensibility-overview.md)
- [Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)](extensibility-open-users.md)
- [Office 365-Domänen](https://technet.microsoft.com/de-DE/library/office-365-domains.aspx)
- [Hinzufügen und Überprüfen einer Domäne für das NEUE Office 365](https://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [schemaExtension-Ressourcentyp](/graph/api/resources/schemaextension?view=graph-rest-1.0)
- [schemaExtensions aufführen](/graph/api/schemaextension-list?view=graph-rest-1.0)
- [schemaExtension erstellen](/graph/api/schemaextension-post-schemaextensions?view=graph-rest-1.0)
- [schemaExtension abrufen](/graph/api/schemaextension-get?view=graph-rest-1.0)
- [schemaExtension aktualisieren](/graph/api/schemaextension-update?view=graph-rest-1.0)
- [schemaExtension löschen](/graph/api/schemaextension-delete?view=graph-rest-1.0)
