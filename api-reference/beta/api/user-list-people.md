---
title: Personen auflisten
description: Abrufen einer Liste von Person-Objekten sortiert nach ihrer Relevanz für den Benutzer, die durch des Benutzers Kommunikation und Zusammenarbeit Muster und geschäftliche Beziehungen bestimmt wird.
author: simonhult
ms.openlocfilehash: 64d24111f295fd076024a889d050c8c48c104295
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347656"
---
# <a name="list-people"></a>Personen auflisten

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Abrufen einer Liste von [Person](../resources/person.md) -Objekten sortiert nach ihrer Relevanz für den [Benutzer](../resources/user.md), die durch des Benutzers Kommunikation und Zusammenarbeit Muster und geschäftliche Beziehungen bestimmt wird.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | People.Read    |
|Delegiert (persönliches Microsoft-Konto) | People.Read    |
|Anwendung | Nicht unterstützt |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a>Optionale Abfrageparameter

Diese Methode unterstützt die folgenden Parameter der OData-Abfrage, mit denen die Antwort anpassen.

|Name|Wert|Beschreibung|
|:---------------|:--------|:-------|
|$filter|string|Dient zum Einschränken der Antwort auf diejenigen Personen, deren Datensätze die angegebenen Kriterien enthalten.|
|$orderby|string|Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert. Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.|
|$search|string|Dient für die Suche nach Personen anhand des Namens oder des Alias. Unterstützt Fuzzyübereinstimmung. Parameter funktioniert nur für die Suche des angemeldeten Benutzers zuständigen Personen, nicht zum Suchen von Personen, die für andere Benutzer relevant. Unterstützt außerdem die `topic` Schlüsselwort Personensuche basierend auf Themen aus E-mail-Konversationen mit dieser Person extrahiert. Siehe Abschnitt *Perform eine fuzzy-Suche* unter [Abrufen von relevante Informationen über Personen](/graph/people-example#perform-a-fuzzy-search) Informationen und Beispiele.|
|$select|string|Durch Trennzeichen getrennte Liste der Eigenschaften, die in die Antwort eingeschlossen werden sollen. Wählen Sie für optimale Leistung nur eine Teilmenge der benötigten Eigenschaften.|
|$skip|int|Die ersten n Ergebnisse werden übersprungen. Hilfreich für Paging. Wird bei Verwendung von *$search* nicht unterstützt.|
|$top|int|Anzahl der Ergebnisse, die zurückgegeben werden.|

## <a name="request-headers"></a>Anforderungsheader

| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Accept | application/json |

## <a name="request-body"></a>Anforderungstext

Geben Sie für diese Methode keinen Anforderungstext an.

## <a name="response"></a>Antwort

Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [Person](../resources/person.md) .

## <a name="examples"></a>Beispiele

### <a name="browse"></a>Durchsuchen

Die Anforderungen in diesem Abschnitt die Personen Abrufen der angemeldeten Benutzer am relevantesten (`/me`), basierend auf Kommunikation, Zusammenarbeit und Business Beziehungen.

Standardmäßig gibt jede Antwort 10 Datensätze zurück, aber Sie können dies mit dem Parameter *$top* ändern. Diese Anfragen erfordern die People.Read-Berechtigung an.

#### <a name="request"></a>Anforderung

Es folgt ein Beispiel für die Standard-Anforderung.
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.
>**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "name": "get_person_collection_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1326

{
    "value": [
        {
            "id": "33b43a5b-87d6-41ec-91f8-a2610048105f",
            "displayName": "Marketing",
            "givenName": null,
            "surname": null,
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "mailboxType": "GroupMailbox",
            "personType": "ModernGroup",
            "userPrincipalName": "",
            "emailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "rank": 30
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "mailboxType": "Mailbox",
            "personType": "Person",
            "userPrincipalName": "IsaiahL@contoso.com",
            "emailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "rank": 20
                }
            ],
            "phones": [
                {
                    "type": "business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        }
    ]
}
```

#### <a name="requesting-a-subsequent-page-of-people"></a>Anfordern einer nachfolgenden Seite von Personen

Wenn die erste Antwort nicht die vollständige Liste der relevanten Personen enthält, können Sie mit *$top* und *$skip* eine zweite Anforderung für das Abrufen weiterer Seiten mit Informationen einreichen. Wenn die vorherige Anforderung zusätzliche Informationen enthält, ruft die darauf folgende Anforderung die nächste Seite der Personen vom Server ab.

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a>Sortieren der Antwort

Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert. Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern. Diese Abfrage wählt die für Sie relevantesten Personen aus, sortiert sie nach ihrem Anzeigenamen und gibt dann die ersten 10 Personen auf der sortierten Liste zurück.

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a>Ändern der Anzahl der zurückgegebenen Personen und der zurückgegebenen Felder

Sie können die Anzahl der Personen ändern, die in der Antwort zurückgegeben wird, indem Sie den *$top*-Parameter festlegen.

Das folgende Beispiel fordert den 1.000 Mitarbeiter am relevantesten `/me`. Die Anforderung schränkt auch die Menge der Daten, die vom Server gesendet werden, indem nur den Anzeigenamen der Person anfordern.

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a>Auswahl der zurückzugebenden Felder

Sie können die Menge der Daten vom Server mithilfe des *$select* -Parameters ein oder mehrere Felder auswählen zurückgegebenen einschränken. Das Feld *@odata.id* wird immer zurückgegeben.

Im folgende Beispiel wird die Antwort auf die *DisplayName* und *EmailAddress* die 10 wichtigsten Benutzer beschränkt.

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a>Verwendung eines Filters zur Begrenzung der Antwort

Sie können den *$filter*-Parameter zum Einschränken der Antwort auf diejenigen Personen einschränken, deren Datensätze die angegebenen Kriterien enthalten.

Die folgende Abfrage beschränkt die Antwort an Personen mit der Quelle "Verzeichnis".

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a>Auswählen der Felder, die in eine gefilterte Antwort zurückgegeben

Sie können die *$select*- und *$filter*-Parameter gemeinsam verwenden, um eine benutzerdefinierte Liste der für den Benutzer relevanten Personen zu erstellen und nur die Felder abzurufen, die Ihre Anwendung benötigt.

Das folgende Beispiel ruft die *DisplayName* und *EmailAddress* von Personen, deren Anzeigename den angegebenen Namen entspricht. In diesem Beispiel werden nur Personen zurückgegeben, deren Anzeigename "Nestor Kellum" ist.

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a>Durchsuchen von Personen

Die Anforderungen in diesem Abschnitt auch die Personen Abrufen der angemeldeten Benutzer am relevantesten (`/me`). Suchanforderungen erfordern die People.Read-Berechtigung an.

#### <a name="using-search-to-select-people"></a>Wählen Sie Personen mithilfe der Suche

Verwenden Sie den *$search*-Parameter zum Auswählen von Personen, die bestimmte Kriterien erfüllen.

Die folgenden Suchabfrage zurückgibt Personen für die Überprüfung relevante `/me` , deren Vorname oder Nachname beginnt mit dem Buchstaben "j".

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a>Mit der Suche ein relevantes Thema angeben

Die folgende Anforderung gibt Personen für die Überprüfung relevante `/me` , deren Namen enthält "Ma" und besitzen eine Zuordnung mit "Feature planen".

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a>Fuzzy-Suche durchführen

Die folgende Anforderung wird eine Suche nach einer Person, die mit dem Namen "Hermaini Saal." Da eine Person, die mit dem Namen "Herminia Hülle" für den angemeldeten Benutzer relevant ist, wird die Informationen für "Herminia Hülle" zurückgegeben.

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a>Verwandte Personen

Die folgende Anforderung Ruft die Personen in der Organisation des Benutzers relevantesten an eine andere Person. Diese Anforderung erfordert die User.ReadBasic.All für People.Read.All-Berechtigung an. In diesem Beispiel werden die Nestor Kellums entsprechenden Personen angezeigt.

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
