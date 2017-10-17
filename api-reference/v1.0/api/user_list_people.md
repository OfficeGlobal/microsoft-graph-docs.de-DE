# <a name="list-people"></a>List people

Dient zum Abrufen einer Sammlung von [person](../resources/person.md)-Objekten, die nach ihrer Relevanz für den [Benutzer](../resources/user.md) sortiert sind, die von den Mustern bei Kommunikation, Zusammenarbeit und den Geschäftsbeziehungen des Benutzers abhängt.

Sie können diese Informationen über die People API abrufen. Beispiele finden Sie in dem Abschnitt [Beispiele](#examples) sowie im Artikel zum Thema [Abrufen relevanter Informationen über Personen](../../../concepts/people_example.md).

## <a name="permissions"></a>Berechtigungen
Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).
 

|Berechtigungstyp      | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto) | People.Read, People.Read.All    |
|Delegiert (persönliches Microsoft-Konto) | People.Read    |
|Anwendung | People.Read.All |

## <a name="http-request"></a>HTTP-Anforderung
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```
## <a name="optional-query-parameters"></a>Optionale Abfrageparameter
|Name|Wert|Beschreibung|
|:---------------|:--------|:-------|
|$filter|Zeichenfolge|Dient zum Einschränken der Antwort auf diejenigen Personen, deren Datensätze die angegebenen Kriterien enthalten.|
|$orderby|string|Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert. Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.|
|$search|string|Dient für die Suche nach Personen anhand des Namens oder des Alias. Unterstützt Fuzzyübereinstimmung.|
|$select|string|Durch Trennzeichen getrennte Liste der Eigenschaften, die in die Antwort eingeschlossen werden sollen. Wählen Sie für optimale Leistung nur eine Teilmenge der benötigten Eigenschaften.|
|$skip|int|Die ersten n Ergebnisse werden übersprungen. Hilfreich für Paging. Wird bei Verwendung von *$search* nicht unterstützt.|
|$top|int|Anzahl der Ergebnisse, die zurückgegeben werden.|

## <a name="request-headers"></a>Anforderungsheader
| Name      |Beschreibung|
|:----------|:----------|
| Authorization  | Bearer {token}. Erforderlich. |
| Annehmen | application/json |

## <a name="request-body"></a>Anforderungstext
Geben Sie für diese Methode keinen Anforderungstext an.
## <a name="response"></a>Antwort
Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [person](../resources/person.md)-Objekten im Antworttext zurückgegeben. Die Antwort kann ein person-Objekt oder eine Sammlung von person-Objekten enthalten. 
## <a name="examples"></a>Beispiele

### <a name="get-a-collection-of-relevant-people"></a>Abrufen einer Sammlung relevanter Personen 

Mit der folgenden Anforderung werden die für den angemeldeten Benutzer relevantesten Personen (`/me`) auf Grundlage von Kommunikations- und Zusammenarbeitsmustern sowie Geschäftsbeziehungen abgerufen. 
<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mithilfe des *$top*-Abfrageparameters ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.
<!-- {
  "blockType": "response",
  "name": "get_person_collection",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "givenName": "Lorrie",
            "surname": "Frye",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Paralegal",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "20/1109",
            "profession": "",
            "userPrincipalName": "Lorrief@contoso.onmicrosoft.com",
            "imAddress": "sip:Lorrief@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 980 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        },
        {
            "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
            "displayName": "Maynard Denman",
            "givenName": "Maynard",
            "surname": "Denman",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "Maynardd@contoso.onmicrosoft.com",
            "imAddress": "sip:Maynardd@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Maynardd@contoso.onmicrosoft.com",
                    "relevanceScore": 8.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        },
        {
            "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
            "displayName": "Darrel Halsey",
            "givenName": "Darrel",
            "surname": "Halsey",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Attorney",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "14/1102",
            "profession": "",
            "userPrincipalName": "Darrelh@contoso.onmicrosoft.com",
            "imAddress": "sip:Darrelh@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Darrelh@contoso.onmicrosoft.com",
                    "relevanceScore": 8.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 205 555 0103"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        }
    ]
}
```
### <a name="search-other-users-relevant-people"></a>Durchsuchen von für andere Benutzer relevanten Personen

Die folgende Anforderung ruft die für eine andere Person in der Organisation des angemeldeten Benutzers relevanten Personen ab. Für diese Anforderung ist die Berechtigung People.Read.All erforderlich. In diesem Beispiel werden für Roscoe Seidel relevante Personen angezeigt.

<!-- {
  "blockType": "request",
  "name": "get_other_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.

<!-- {
  "blockType": "response",
  "name": "get_other_person",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
     "value": [
        {
            "id": "56155636-703F-47F2-B657-C83F01F49BBC",
            "displayName": "Clifton Clemente",
            "givenName": "Clifton",
            "surname": "Clemente",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Director",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "19/2106",
            "profession": "",
            "userPrincipalName": "Cliftonc@contoso.onmicrosoft.com",
            "imAddress": "sip:Cliftonc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Cliftonc@contoso.onmicrosoft.com",
                    "relevanceScore": 20.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 309 555 0101"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        },
        {
            "id": "6BF27D5A-AB4F-4C43-BED0-7DAD9EB0C1C4",
            "displayName": "Sheree Mitchell",
            "givenName": "Sheree",
            "surname": "Mitchell",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Product Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/2107",
            "profession": "",
            "userPrincipalName": "Shereem@contoso.onmicrosoft.com",
            "imAddress": "sip:shereem@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Shereem@contoso.onmicrosoft.com",
                    "relevanceScore": 10.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 918 555 0107"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        },
        {
            "id": "B3E5302D-EAF0-4E8B-8C6C-A2AE64B4B163",
            "displayName": "Vincent Matney",
            "givenName": "Vincent",
            "surname": "Matney",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "CVP Engineering",
            "companyName": null,
            "yomiCompany": "",
            "department": "Engineering",
            "officeLocation": "23/2102",
            "profession": "",
            "userPrincipalName": "Vincentm@contoso.onmicrosoft.com",
            "imAddress": "sip:vincentm@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Vincentm@contoso.onmicrosoft.com",
                    "relevanceScore": 10.0
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 502 555 0102"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": [
                {
                    "class": "Person",
                    "subclass": "OrganizationUser"
                }
            ]
        }
    ]
}
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
