# <a name="use-the-people-api-in-microsoft-graph-to-get-information-about-the-people-most-relevant-to-you"></a>Verwenden der People API in Microsoft Graph zum Abrufen von Informationen über relevante Personen
Microsoft Graph-Anwendungen können die People API zum Abrufen von Personen verwenden, die für einen Benutzer am relevantesten sind. Relevanz wird durch die Kommunikations- und Zusammenarbeitsmuster und Geschäftsbeziehungen des Benutzers bestimmt. Personen können lokale Kontakte, Kontakte aus sozialen Netzwerken, aus dem Verzeichnis Ihrer Organisation und Personen aus kürzlichen Unterhaltungen (z. B. E-Mail und Skype) sein. Neben Generierung dieser Einblicke bietet die People API auch Unterstützung für Fuzzyübereinstimmungen bei Suchvorgängen sowie die Möglichkeit, eine Liste der für einen Benutzer relevanten Benutzer in der Organisation des angemeldeten Benutzers abzurufen. Die People API ist insbesondere beim Auswählen von Personen hilfreich, z. B. beim Verfassen einer E-Mail oder beim Erstellen einer Besprechung. Sie können die People API beispielsweise beim Verfassen von E-Mails verwenden.
 
## <a name="authorization"></a>Authorization
Zum Aufrufen der People API in Microsoft Graph benötigt Ihre App die entsprechenden Berechtigungen: 

* People.Read – Verwenden Sie diese Berechtigung für allgemeine People API-Aufrufe, beispielsweise https://graph.microsoft.com/v1.0/me/people/. People.Read erfordert die Zustimmung des Endbenutzers.
* People.Read.All – Erforderlich, um die für einen bestimmten Benutzer relevanten Personen in den Aufrufen der Organisation des angemeldeten Benutzer abzurufen (https://graph.microsoft.com/v1.0/users(('{id}')/people). People.Read.All erfordert die Zustimmung des Administrators.
## <a name="browse-people"></a>Durchsuchen von Personen
Bei den Anforderungen in diesem Abschnitt werden die für den angemeldeten Benutzer oder einen bestimmten Benutzer, der bei der Organisation des Benutzers angemeldet ist, relevantesten Personen abgerufen (`/me`). Für diese Anforderungen ist die Berechtigung „People.Read“ oder „People.Read.All“ erforderlich. Standardmäßig gibt jede Antwort 10 Datensätze zurück, Sie können diese Einstellung jedoch mithilfe des *$top*-Abfrageparameters ändern. 
### <a name="get-a-collection-of-relevant-people"></a>Abrufen einer Sammlung relevanter Personen 
Mit der folgenden Anforderung werden die für den angemeldeten Benutzer relevantesten Personen (`/me`) auf Grundlage von Kommunikations- und Zusammenarbeitsmustern sowie Geschäftsbeziehungen abgerufen. 

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mithilfe des *$top*-Abfrageparameters ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.

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
                    "relevanceScore": 8
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
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
                    "relevanceScore": 8
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
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
                    "relevanceScore": 8
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```
### <a name="request-a-subsequent-page-of-people"></a>Anfordern einer nachfolgenden Seite mit Personen
Wenn die erste Antwort nicht die vollständige Liste der relevanten Personen enthält, können Sie mit *$top* und *$skip* eine zweite Anforderung für das Abrufen weiterer Seiten mit Informationen einreichen. Wenn die vorherige Anforderung zusätzliche Informationen enthält, ruft die darauf folgende Anforderung die nächste Seite der Personen vom Server ab.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$top=3&$skip=10
```

Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mithilfe des *$top*-Abfrageparameters ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "1F28616D-BDFE-4080-8F06-03366A851688",
            "displayName": "Felix Coppola",
            "givenName": "Felix",
            "surname": "Coppola",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "CVP Legal",
            "companyName": null,
            "yomiCompany": "",
            "department": "Legal",
            "officeLocation": "19/2109",
            "profession": "",
            "userPrincipalName": "Felixc@contoso.onmicrosoft.com",
            "imAddress": "sip:Felixc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Felixc@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 309 555 0104"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "8A3FC021-6DBB-44AC-8884-B7B500CC260A",
            "displayName": "Lenora Rowland",
            "givenName": "Lenora",
            "surname": "Rowland",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Marketing Assistant",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "18/1106",
            "profession": "",
            "userPrincipalName": "Lenorar@contoso.onmicrosoft.com",
            "imAddress": "sip:Lenorar@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Lenorar@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 954 555 0118"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "032C9919-4DF9-4715-8C46-4D0FAE7B3EB2",
            "displayName": "Manuel Collette",
            "givenName": "Manuel",
            "surname": "Collette",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Accountant II",
            "companyName": null,
            "yomiCompany": "",
            "department": "Finance",
            "officeLocation": "98/2202",
            "profession": "",
            "userPrincipalName": "Manuelc@contoso.onmicrosoft.com",
            "imAddress": "sip:Manuelc@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Manuelc@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+20 255501070"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```
### <a name="sort-the-response"></a>Sortieren der Antwort 
Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert. Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern. Diese Abfrage wählt die für Sie relevanten Personen aus, sortiert sie nach **displayName**, und gibt dann die ersten 10 Personen der sortierten Liste zurück.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$orderby=displayName
```

Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. Im folgenden Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "818E29A1-E6BB-4EDA-AB20-8230B4B1E290",
            "displayName": "Adriana Ramos",
            "givenName": "Adriana",
            "surname": "Ramos",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Product Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "18/2111",
            "profession": "",
            "userPrincipalName": "Adrianar@contoso.onmicrosoft.com",
            "imAddress": "sip:Adrianar@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Adrianar@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 425 555 0109"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "62633BAA-1CB9-4FA2-9B8F-55AB1840B69D",
            "displayName": "Alyce Cooley",
            "givenName": "Alyce",
            "surname": "Cooley",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Marketing Assistant",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "131/1104",
            "profession": "",
            "userPrincipalName": "Alycec@contoso.onmicrosoft.com",
            "imAddress": "sip:Alycec@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Alycec@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 858 555 0110"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "6BB54D2C-EF20-48DA-ADD9-AE757DD30C4E",
            "displayName": "Alyssa Clarke",
            "givenName": "Alyssa",
            "surname": "Clarke",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Corporate Security Officer",
            "companyName": null,
            "yomiCompany": "",
            "department": "Operations",
            "officeLocation": "24/1106",
            "profession": "",
            "userPrincipalName": "Alyssac@contoso.onmicrosoft.com",
            "imAddress": "sip:Alyssac@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "Alyssac@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 262 555 0106"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```
### <a name="change-the-number-of-people-and-fields-returned"></a>Ändern der Anzahl von Personen und der zurückgegebenen Felder 
Sie können die Anzahl der Personen ändern, die in der Antwort zurückgegeben wird, indem Sie den *$top*-Parameter festlegen. 

Im folgende Beispiel werden die für `/me` 1.000 relevantesten Personen angefordert. Die Anforderung begrenzt außerdem die Menge der Daten, die vom Server gesendet werden, indem nur der **displayName** der Person angefordert wird.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$top=1000&$Select=displayName
```

Das folgende Beispiel zeigt die Antwort. 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye"
        },
        {
            "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
            "displayName": "Maynard Denman"
        },
        {
            "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
            "displayName": "Darrel Halsey"
        },
        {
            "id": "E3C5B235-DE15-4566-B7B1-7A8E32426540",
            "displayName": "Roscoe Seidel"
        },
        {
            "id": "6BB54D2C-EF20-48DA-ADD9-AE757DD30C4E",
            "displayName": "Alyssa Clarke"
        },
        {
            "id": "818E29A1-E6BB-4EDA-AB20-8230B4B1E290",
            "displayName": "Adriana Ramos"
        },
        {
            "id": "62633BAA-1CB9-4FA2-9B8F-55AB1840B69D",
            "displayName": "Alyce Cooley"
        },
        {
            "id": "6BB9CC1F-418D-4DDF-AB0C-6A1C4ABCDBF4",
            "displayName": "Wayne Leeper"
        },
        {
            "id": "E7D40AC5-0078-4575-B1F3-F738124C4BC9",
            "displayName": "Jan Travis"
        },
        {
            "id": "6F99D1CC-4FCC-49E4-9160-E8AB01BF3E83",
            "displayName": "Charlotte Delacruz"
        },
        {
            "id": "1F28616D-BDFE-4080-8F06-03366A851688",
            "displayName": "Felix Coppola"
        },
        {
            "id": "8A3FC021-6DBB-44AC-8884-B7B500CC260A",
            "displayName": "Lenora Rowland"
        },
        {
            "id": "032C9919-4DF9-4715-8C46-4D0FAE7B3EB2",
            "displayName": "Manuel Collette"
        },
      ... etc
}
```
### <a name="select-the-fields-to-return"></a>Auswählen der zurückgegebenen Felder
Sie können die Menge der vom Server zurückgegebenen Daten einschränken, indem Sie den *$select*-Parameter zum Auswählen der Felder verwenden. Das `@odata.id`-Feld wird immer zurückgegeben.

Im folgenden Beispiel wird die Antwort auf **displayName** und **scoredEmailAddresses** der 10 relevantesten Personen begrenzt.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses
```

Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        },
        {
            "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
            "displayName": "Maynard Denman",
            "scoredEmailAddresses": [
                {
                    "address": "Maynardd@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        },
        {
            "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
            "displayName": "Darrel Halsey",
            "scoredEmailAddresses": [
                {
                    "address": "Darrelh@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        }
    ]
}
```
### <a name="use-a-filter-to-limit-the-response"></a>Verwenden eines Filters zum Einschränken der Antwort 
Sie können den *$filter*-Parameter zum Einschränken der Antwort auf diejenigen Personen einschränken, deren Datensätze die angegebenen Kriterien enthalten. 

Bei der folgenden Abfrage wird die Antwort auf die **person**-Instanzen mit der **personType**-Eigenschaft eingeschränkt, für die **person** als **class** und **organizationUser** als **subclass** festgelegt ist.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$filter=personType/class eq 'Person' and personType/subclass eq 'OrganizationUser'
```

Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.

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
                    "relevanceScore": 8
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
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
                    "relevanceScore": 8
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
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
                    "relevanceScore": 8
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```
### <a name="select-the-fields-to-return-in-a-filtered-response"></a>Auswählen der Felder, die in einer gefilterten Antwort zurückgegeben werden 
Sie können die *$select*- und *$filter*-Parameter gemeinsam verwenden, um eine benutzerdefinierte Liste der für den Benutzer relevanten Personen zu erstellen und nur die Felder abzurufen, die Ihre Anwendung benötigt. 

Im folgenden Beispiel wird **displayName** und **scoredEmailAddresses** von Personen angerufen, deren Anzeigenamen dem angegebenen Namen entspricht. In diesem Beispiel werden nur die Personen zurückgegeben, deren Anzeigename „Lorrie Frye“ lautet. 

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

Das folgende Beispiel zeigt die Antwort. 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "8CE6E1DE-CB84-4BF5-971D-D3ECF452E2B5",
            "displayName": "Lorrie Frye",
            "scoredEmailAddresses": [
                {
                    "address": "Lorrief@contoso.onmicrosoft.com",
                    "relevanceScore": 8
                }
            ]
        }
    ]
}
```

### <a name="browse-another-users-relevant-people"></a>Durchsuchen von für andere Benutzer relevanten Personen
Die folgende Anforderung ruft die für eine andere Person in der Organisation des angemeldeten Benutzers relevanten Personen ab. Für diese Anforderung ist die Berechtigung People.Read.All erforderlich. Alle in den vorherigen Abschnitten beschriebenen Abfrageparameter gelten ebenfalls.

In diesem Beispiel werden für Roscoe Seidel relevante Personen angezeigt.

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. Im folgenden Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.

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
                    "relevanceScore": 20
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
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
                    "relevanceScore": 10
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
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
                    "relevanceScore": 10
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```

## <a name="search-people"></a>Durchsuchen von Personen
Mit den Anforderungen in diesem Abschnitt können Sie nach Personen suchen, die für den angemeldeten Benutzer (`/me`) und andere Benutzer in der Organisation des angemeldeten Benutzers relevant sind. Für diese Anforderungen ist die People.Read-Berechtigung erforderlich. Eine Ausnahme stellt die Suche nach für andere Benutzer relevanten Personen, für die die People.Read.All-Berechtigung erforderlich ist. Standardmäßig gibt jede Antwort 10 Datensätze zurück, Sie können diese Einstellung jedoch mithilfe des *$top*-Parameters ändern. 
### <a name="use-search-to-select-people"></a>Verwenden der Suche zum Auswählen von Personen 
Verwenden Sie den *$search*-Parameter zum Auswählen von Personen, die bestimmte Kriterien erfüllen. 

Mit der folgenden Abfrage werden die für `/me` relevanten Personen zurückgegeben, deren **displayName** oder „emailAddress“ mit dem Buchstaben „j“ beginnt.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search=j
```

Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
            "id": "E3C5B235-DE15-4566-B7B1-7A8E32426540",
            "displayName": "Jan Travis",
            "givenName": "Jan",
            "surname": "Travis",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "VP Sales",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "19/3123",
            "profession": "",
            "userPrincipalName": "jant@contoso.onmicrosoft.com",
            "imAddress": "sip:jant@contoso.onmicrosoft.com",
            "scoredEmailAddresses": [
                {
                    "address": "jant@contoso.onmicrosoft.com",
                    "relevanceScore": -12.297347783416837
                }
            ],
            "phones": [
                {
                    "type": "Business",
                    "number": "+1 732 555 0102"
                }
            ],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        },
        {
            "id": "C43BF05E-5B6B-4DCF-B2FC-0837B09E0FA9",
            "displayName": "Jacob Cazares (TAILSPIN)",
            "givenName": null,
            "surname": null,
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "userPrincipalName": "",
            "imAddress": null,
            "scoredEmailAddresses": [
                {
                    "address": "jacobc@tailspintoys.com",
                    "relevanceScore": -12.298154282019846
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "PersonalContact"
            }
        },
        {
            "id": "6BB9CC1F-418D-4DDF-AB0C-6A1C4ABCDBF4",
            "displayName": "Jewell Montgomery",
            "givenName": "Jewell",
            "surname": "Montgomery",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "userPrincipalName": "jewellm@contoso.onmicrosoft.com",
            "imAddress": null,
            "scoredEmailAddresses": [
                {
                    "address": "jewellm@contoso.onmicrosoft.com",
                    "relevanceScore": -12.531408487977451
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```
### <a name="perform-a-fuzzy-search"></a>Durchführen einer Fuzzysuche 

Suchvorgänge implementieren einen Algorithmus für Fuzzyübereinstimmungen. Dabei werden Ergebnisse basierend auf einer exakten Übereinstimmung und auch zu Rückschlüssen zu der Absicht der Suche zurückgegeben. Verwenden wir als Beispiel einen Benutzer mit dem Anzeigenamen „Tyler Lee“ und der E-Mail-Adresse „tylerle@example.com“, der sich in der **people**-Sammlung des angemeldeten Benutzers befindet. Alle der folgenden Suchvorgänge geben den Benutzer „Tyler“ als eines der Ereignisse zurück.

```http
GET https://graph.microsoft.com/v1.0/me/people?$search=tyler                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search=tylerle              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search=tiler                //fuzzy match with Tyler's name 
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"          //matches Tyler's name. Note the quotes to enclose the space.
```

Sie können auch Suchvorgänge nach Personen durchführen, die für den angemeldeten Benutzer relevant sind und Interesse an der Kommunikation über bestimmte Themen mit diesem Benutzer gezeigt haben, wie z. B. zum Thema „Pizza“ wie im folgenden Beispiel:

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:pizza"                
```

Themen in diesem Sinne sind einfach Wörter, die in der E-Mail-Kommunikation von den Benutzern am häufigsten verwendet wurden. Microsoft extrahiert diese Wörter und erstellt einen Index für diese Daten, um die Fuzzysuche zu erleichtern. 

Beachten Sie, dass der Suchbegriff in Anführungszeichen eingeschlossen ist und die Themen in diesen Daten ohne Kontext extrahiert werden. Beispiel – Die Suche nach dem englischen Begriff „Windows“ in der folgenden Abfrage:

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="topic:windows" 
```
ist eine Fuzzysuche im Themendatenindex, und die Ergebnisse können Instanzen umfassen, die das Windows-Betriebssystem, eine Öffnung in einer Gebäudewand oder andere Definitionen bezeichnen.

Sie können auch Personen- und Themensuchen in derselben Anforderung kombinieren, indem Sie die beiden Typen von Suchausdrücken kombinieren.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="tyl topic:pizza"                
```

Bei dieser Anforderung werden im Wesentlichen zwei Suchvorgänge ausgeführt: eine unscharfe Suche in den Eigenschaften**displayName** und **emailAddress** der relevanten Personen des angemeldeten Benutzers und eine Themensuche nach „Pizza“ in den relevanten Personen des Benutzers. Die Ergebnisse werden dann bewertet, sortiert und zurückgegeben. Beachten Sie, dass die Suche nicht restriktiv ist. Sie erhalten möglicherweise Ergebnisse, die Personen enthalten, die mit „tyl“ übereinstimmen oder die an „Pizza“ interessiert sind oder beides.

