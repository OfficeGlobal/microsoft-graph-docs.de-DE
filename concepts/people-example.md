---
title: Verwenden der People API in Microsoft Graph zum Abrufen von Informationen über relevante Personen
description: Microsoft Graph-Anwendungen können die People API zum Abrufen von Personen verwenden, die für einen Benutzer am relevantesten sind. Relevanz wird durch die Kommunikations- und Zusammenarbeitsmuster und Geschäftsbeziehungen des Benutzers bestimmt. Personen können lokale Kontakte, Kontakte aus sozialen Netzwerken, aus dem Verzeichnis Ihrer Organisation und Personen aus kürzlichen Unterhaltungen (z. B. E-Mail und Skype) sein. Neben Generierung dieser Einblicke bietet die People API auch Unterstützung für Fuzzyübereinstimmungen bei Suchvorgängen sowie die Möglichkeit, eine Liste der für einen Benutzer relevanten Benutzer in der Organisation des angemeldeten Benutzers abzurufen.
ms.date: 12/04/2018
author: simonhult
ms.openlocfilehash: e5cfc5abb7bac06f0355ebc2a2b70460050aa7e8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306853"
---
# <a name="use-the-people-api-in-microsoft-graph-to-get-information-about-the-people-most-relevant-to-you"></a><span data-ttu-id="ef25c-106">Verwenden der People API in Microsoft Graph zum Abrufen von Informationen über relevante Personen</span><span class="sxs-lookup"><span data-stu-id="ef25c-106">Use the People API in Microsoft Graph to get information about the people most relevant to you</span></span>

<span data-ttu-id="ef25c-p102">Microsoft Graph-Anwendungen können die People API zum Abrufen von Personen verwenden, die für einen Benutzer am relevantesten sind. Relevanz wird durch die Kommunikations- und Zusammenarbeitsmuster und Geschäftsbeziehungen des Benutzers bestimmt. Personen können lokale Kontakte, Kontakte aus sozialen Netzwerken, aus dem Verzeichnis Ihrer Organisation und Personen aus kürzlichen Unterhaltungen (z. B. E-Mail und Skype) sein. Neben Generierung dieser Einblicke bietet die People API auch Unterstützung für Fuzzyübereinstimmungen bei Suchvorgängen sowie die Möglichkeit, eine Liste der für einen Benutzer relevanten Benutzer in der Organisation des angemeldeten Benutzers abzurufen. Die People API ist insbesondere beim Auswählen von Personen hilfreich, z. B. beim Verfassen einer E-Mail oder beim Erstellen einer Besprechung. Sie können die People API beispielsweise beim Verfassen von E-Mails verwenden.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p102">Microsoft Graph applications can use the People API to retrieve the people who are most relevant to a user. Relevance is determined by the user’s communication and collaboration patterns and business relationships. People can be local contacts, contacts from social networking or from an organization’s directory, and people from recent communications (such as email and Skype). Along with generating this insight, the People API also provides fuzzy matching search support and the ability to retrieve the list of users relevant to another user in the signed-in user's organization. The People API is particularly useful for people picking scenarios, such as composing an email or creating a meeting. For example, you can use the People API in email compose scenarios.</span></span>

## <a name="authorization"></a><span data-ttu-id="ef25c-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef25c-113">Authorization</span></span>

<span data-ttu-id="ef25c-114">Zum Aufrufen der People API in Microsoft Graph benötigt Ihre App die entsprechenden Berechtigungen:</span><span class="sxs-lookup"><span data-stu-id="ef25c-114">To call the People API in Microsoft Graph, your app will need the appropriate permissions:</span></span>

* <span data-ttu-id="ef25c-p103">People.Read – Verwenden Sie diese Berechtigung für allgemeine People API-Aufrufe, beispielsweise `https://graph.microsoft.com/v1.0/me/people/`. People.Read erfordert die Zustimmung des Endbenutzers.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p103">People.Read - Use to make general People API calls; for example, `https://graph.microsoft.com/v1.0/me/people/`. People.Read requires end user consent.</span></span>
* <span data-ttu-id="ef25c-117">People.Read.All – Erforderlich, um die für einen bestimmten Benutzer relevanten Personen in den Aufrufen der Organisation des angemeldeten Benutzers (`https://graph.microsoft.com/v1.0/users('{id}')/people`) abzurufen.</span><span class="sxs-lookup"><span data-stu-id="ef25c-117">People.Read.All - Required to retrieve the people most relevant to a specified user in the signed-in user’s organization (`https://graph.microsoft.com/v1.0/users('{id}')/people`) calls.</span></span> <span data-ttu-id="ef25c-118">People.Read.All erfordert die Zustimmung des Administrators.</span><span class="sxs-lookup"><span data-stu-id="ef25c-118">People.Read.All requires admin consent.</span></span>

## <a name="browse-people"></a><span data-ttu-id="ef25c-119">Durchsuchen von Personen</span><span class="sxs-lookup"><span data-stu-id="ef25c-119">Browse people</span></span>

<span data-ttu-id="ef25c-p105">Bei den Anforderungen in diesem Abschnitt werden die für den angemeldeten Benutzer oder einen bestimmten Benutzer, der bei der Organisation des Benutzers angemeldet ist, relevantesten Personen abgerufen (`/me`). Für diese Anforderungen ist die Berechtigung „People.Read“ oder „People.Read.All“ erforderlich. Standardmäßig gibt jede Antwort 10 Datensätze zurück, Sie können diese Einstellung jedoch mithilfe des *$top*-Abfrageparameters ändern.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p105">The requests in this section get the people most relevant to the signed-in user (`/me`), or to a specific user in the signed-in user’s organization. These requests require the People.Read or People.Read.All permission respectively. By default, each response returns 10 records, but you can change this by using the *$top* query parameter.</span></span>

### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="ef25c-123">Abrufen einer Sammlung relevanter Personen</span><span class="sxs-lookup"><span data-stu-id="ef25c-123">Get a collection of relevant people</span></span>

<span data-ttu-id="ef25c-124">Mit der folgenden Anforderung werden die für den angemeldeten Benutzer relevantesten Personen (`/me`) auf Grundlage von Kommunikations- und Zusammenarbeitsmustern sowie Geschäftsbeziehungen abgerufen.</span><span class="sxs-lookup"><span data-stu-id="ef25c-124">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="ef25c-p106">Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mithilfe des *$top*-Abfrageparameters ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p106">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>

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
      "userPrincipalName": "LorrieF@contoso.onmicrosoft.com",
      "imAddress": "sip:LorrieF@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "LorrieF@contoso.onmicrosoft.com",
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
      "userPrincipalName": "MaynardD@contoso.onmicrosoft.com",
      "imAddress": "sip:MaynardD@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "MaynardD@contoso.onmicrosoft.com",
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
      "userPrincipalName": "DarrelH@contoso.onmicrosoft.com",
      "imAddress": "sip:DarrelH@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "DarrelH@contoso.onmicrosoft.com",
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

### <a name="request-a-subsequent-page-of-people"></a><span data-ttu-id="ef25c-129">Anfordern einer nachfolgenden Seite mit Personen</span><span class="sxs-lookup"><span data-stu-id="ef25c-129">Request a subsequent page of people</span></span>

<span data-ttu-id="ef25c-p107">Wenn die erste Antwort nicht die vollständige Liste der relevanten Personen enthält, können Sie mit *$top* und *$skip* eine zweite Anforderung für das Abrufen weiterer Seiten mit Informationen einreichen. Wenn die vorherige Anforderung zusätzliche Informationen enthält, ruft die darauf folgende Anforderung die nächste Seite der Personen vom Server ab.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p107">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$top=3&$skip=10
```

<span data-ttu-id="ef25c-p108">Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mithilfe des *$top*-Abfrageparameters ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p108">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>

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
      "userPrincipalName": "FelixC@contoso.onmicrosoft.com",
      "imAddress": "sip:FelixC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "FelixC@contoso.onmicrosoft.com",
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
      "userPrincipalName": "LenoraR@contoso.onmicrosoft.com",
      "imAddress": "sip:LenoraR@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "LenoraR@contoso.onmicrosoft.com",
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
      "userPrincipalName": "ManuelC@contoso.onmicrosoft.com",
      "imAddress": "sip:ManuelC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "ManuelC@contoso.onmicrosoft.com",
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

### <a name="sort-the-response"></a><span data-ttu-id="ef25c-136">Sortieren der Antwort</span><span class="sxs-lookup"><span data-stu-id="ef25c-136">Sort the response</span></span>

<span data-ttu-id="ef25c-p109">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert. Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern. Diese Abfrage wählt die für Sie relevanten Personen aus, sortiert sie nach **displayName**, und gibt dann die ersten 10 Personen der sortierten Liste zurück.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p109">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter. This query selects the people most relevant to you, sorts them by their **displayName**, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$orderby=displayName
```

<span data-ttu-id="ef25c-p110">Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. Im folgenden Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p110">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. The following example uses *$top* to limit the response to three records.</span></span>

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
      "userPrincipalName": "AdrianaR@contoso.onmicrosoft.com",
      "imAddress": "sip:AdrianaR@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "AdrianaR@contoso.onmicrosoft.com",
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
      "userPrincipalName": "AlyceC@contoso.onmicrosoft.com",
      "imAddress": "sip:AlyceC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "AlyceC@contoso.onmicrosoft.com",
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
      "userPrincipalName": "AlyssaC@contoso.onmicrosoft.com",
      "imAddress": "sip:AlyssaC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "AlyssaC@contoso.onmicrosoft.com",
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

### <a name="change-the-number-of-people-and-fields-returned"></a><span data-ttu-id="ef25c-144">Ändern der Anzahl von Personen und der zurückgegebenen Felder</span><span class="sxs-lookup"><span data-stu-id="ef25c-144">Change the number of people and fields returned</span></span>

<span data-ttu-id="ef25c-145">Sie können die Anzahl der Personen ändern, die in der Antwort zurückgegeben wird, indem Sie den *$top*-Parameter festlegen.</span><span class="sxs-lookup"><span data-stu-id="ef25c-145">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="ef25c-p111">Im folgende Beispiel werden die für `/me` 1.000 relevantesten Personen angefordert. Die Anforderung begrenzt außerdem die Menge der Daten, die vom Server gesendet werden, indem nur der **displayName** der Person angefordert wird.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p111">The following example requests the 1,000 people most relevant to `/me`. The request also limits the amount of data sent back from the server by requesting only the **displayName** of the person.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$top=1000&$Select=displayName
```

<span data-ttu-id="ef25c-148">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="ef25c-148">The following example shows the response.</span></span>

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
    }
  ]
}
```

### <a name="select-the-fields-to-return"></a><span data-ttu-id="ef25c-149">Auswählen der zurückgegebenen Felder</span><span class="sxs-lookup"><span data-stu-id="ef25c-149">Select the fields to return</span></span>

<span data-ttu-id="ef25c-p112">Sie können die Menge der vom Server zurückgegebenen Daten einschränken, indem Sie den *$select*-Parameter zum Auswählen der Felder verwenden. Das `@odata.id`-Feld wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p112">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields. The `@odata.id` field is always returned.</span></span>

<span data-ttu-id="ef25c-152">Im folgenden Beispiel wird die Antwort auf **displayName** und **scoredEmailAddresses** der 10 relevantesten Personen begrenzt.</span><span class="sxs-lookup"><span data-stu-id="ef25c-152">The following example limits the response to the **displayName** and **scoredEmailAddresses** of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses
```

<span data-ttu-id="ef25c-p113">Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p113">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

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
          "address": "LorrieF@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ]
    },
    {
      "id": "5767393D-42BA-4E5C-BEE4-52BB25639CF4",
      "displayName": "Maynard Denman",
      "scoredEmailAddresses": [
        {
          "address": "MaynardD@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ]
    },
    {
      "id": "914B5191-11FA-4C0B-A354-0FA8C8EFD585",
      "displayName": "Darrel Halsey",
      "scoredEmailAddresses": [
        {
          "address": "DarrelH@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ]
    }
  ]
}
```

### <a name="use-a-filter-to-limit-the-response"></a><span data-ttu-id="ef25c-157">Verwenden eines Filters zum Einschränken der Antwort</span><span class="sxs-lookup"><span data-stu-id="ef25c-157">Use a filter to limit the response</span></span>

<span data-ttu-id="ef25c-158">Sie können den *$filter*-Parameter zum Einschränken der Antwort auf diejenigen Personen einschränken, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="ef25c-158">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="ef25c-159">Bei der folgenden Abfrage wird die Antwort auf die **person**-Instanzen mit der **personType**-Eigenschaft eingeschränkt, für die **person** als **class** und **organizationUser** als **subclass** festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="ef25c-159">The following query limits the response to **person** instances with the **personType** property being assigned **person** as **class** and **organizationUser** as **subclass**.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$filter=personType/class eq 'Person' and personType/subclass eq 'OrganizationUser'
```

<span data-ttu-id="ef25c-p114">Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p114">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

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
      "userPrincipalName": "LorrieF@contoso.onmicrosoft.com",
      "imAddress": "sip:LorrieF@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "LorrieF@contoso.onmicrosoft.com",
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
      "userPrincipalName": "MaynardD@contoso.onmicrosoft.com",
      "imAddress": "sip:MaynardD@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "MaynardD@contoso.onmicrosoft.com",
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
      "userPrincipalName": "DarrelH@contoso.onmicrosoft.com",
      "imAddress": "sip:DarrelH@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "DarrelH@contoso.onmicrosoft.com",
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

### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="ef25c-164">Auswählen der Felder, die in einer gefilterten Antwort zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="ef25c-164">Select the fields to return in a filtered response</span></span>

<span data-ttu-id="ef25c-165">Sie können die *$select*- und *$filter*-Parameter gemeinsam verwenden, um eine benutzerdefinierte Liste der für den Benutzer relevanten Personen zu erstellen und nur die Felder abzurufen, die Ihre Anwendung benötigt.</span><span class="sxs-lookup"><span data-stu-id="ef25c-165">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="ef25c-p115">Im folgenden Beispiel wird **displayName** und **scoredEmailAddresses** von Personen angerufen, deren Anzeigenamen dem angegebenen Namen entspricht. In diesem Beispiel werden nur die Personen zurückgegeben, deren Anzeigename „Lorrie Frye“ lautet.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p115">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="ef25c-168">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="ef25c-168">The following example shows the response.</span></span>

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
          "address": "LorrieF@contoso.onmicrosoft.com",
          "relevanceScore": 8
        }
      ]
    }
  ]
}
```

### <a name="browse-another-users-relevant-people"></a><span data-ttu-id="ef25c-169">Durchsuchen von für andere Benutzer relevanten Personen</span><span class="sxs-lookup"><span data-stu-id="ef25c-169">Browse another user’s relevant people</span></span>

<span data-ttu-id="ef25c-170">Die folgende Anforderung ruft die für eine andere Person in der Organisation des angemeldeten Benutzers relevanten Personen ab.</span><span class="sxs-lookup"><span data-stu-id="ef25c-170">The following request gets the people most relevant to another person in the signed-in user's organization.</span></span> <span data-ttu-id="ef25c-171">Für diese Anforderung ist die Berechtigung People.Read.All erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ef25c-171">This request requires the People.Read.All permission.</span></span> <span data-ttu-id="ef25c-172">Alle in den vorherigen Abschnitten beschriebenen Abfrageparameter gelten ebenfalls.</span><span class="sxs-lookup"><span data-stu-id="ef25c-172">All the query parameters described in the above sections apply as well.</span></span>

<span data-ttu-id="ef25c-173">In diesem Beispiel werden für Roscoe Seidel relevante Personen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ef25c-173">In this example, Roscoe Seidel's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="ef25c-p117">Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. Im folgenden Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p117">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. The example below uses *$top* to limit the response to three records.</span></span>

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
      "userPrincipalName": "CliftonC@contoso.onmicrosoft.com",
      "imAddress": "sip:CliftonC@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "CliftonC@contoso.onmicrosoft.com",
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
      "userPrincipalName": "ShereeM@contoso.onmicrosoft.com",
      "imAddress": "sip:ShereeM@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "ShereeM@contoso.onmicrosoft.com",
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
      "userPrincipalName": "VincentM@contoso.onmicrosoft.com",
      "imAddress": "sip:VincentM@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "VincentM@contoso.onmicrosoft.com",
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

## <a name="search-people"></a><span data-ttu-id="ef25c-178">Durchsuchen von Personen</span><span class="sxs-lookup"><span data-stu-id="ef25c-178">Search people</span></span>

<span data-ttu-id="ef25c-p118">Mit den Anforderungen in diesem Abschnitt können Sie nach Personen suchen, die für den angemeldeten Benutzer (`/me`) und andere Benutzer in der Organisation des angemeldeten Benutzers relevant sind. Für diese Anforderungen ist die People.Read-Berechtigung erforderlich. Eine Ausnahme stellt die Suche nach für andere Benutzer relevanten Personen, für die die People.Read.All-Berechtigung erforderlich ist. Standardmäßig gibt jede Antwort 10 Datensätze zurück, Sie können diese Einstellung jedoch mithilfe des *$top*-Parameters ändern.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p118">The requests in this section allow you to search for people relevant to the signed-in user (`/me`) and other users in the signed-in user’s organization. These requests require the People.Read permission, with the exception of searching other users’ relevant people, which requires People.Read.All. By default, each response returns 10 records, but you can change this by using the *$top* parameter.</span></span>

### <a name="use-search-to-select-people"></a><span data-ttu-id="ef25c-182">Verwenden der Suche zum Auswählen von Personen</span><span class="sxs-lookup"><span data-stu-id="ef25c-182">Use search to select people</span></span>

<span data-ttu-id="ef25c-183">Verwenden Sie den *$search*-Parameter zum Auswählen von Personen, die bestimmte Kriterien erfüllen.</span><span class="sxs-lookup"><span data-stu-id="ef25c-183">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="ef25c-184">Mit der folgenden Abfrage werden die für `/me` relevanten Personen zurückgegeben, deren **displayName** oder „emailAddress“ mit dem Buchstaben „j“ beginnt.</span><span class="sxs-lookup"><span data-stu-id="ef25c-184">The following search query returns people relevant to `/me` whose **displayName** or \*emailAddress" has a word that begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search=j
```

<span data-ttu-id="ef25c-p119">Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="ef25c-p119">The following example shows the response. By default, each response returns 10 records. You can change this using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

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
      "userPrincipalName": "JanT@contoso.onmicrosoft.com",
      "imAddress": "sip:JanT@contoso.onmicrosoft.com",
      "scoredEmailAddresses": [
        {
          "address": "JanT@contoso.onmicrosoft.com",
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
          "address": "JacobC@tailspintoys.com",
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
      "userPrincipalName": "JewellM@contoso.onmicrosoft.com",
      "imAddress": null,
      "scoredEmailAddresses": [
        {
          "address": "JewellM@contoso.onmicrosoft.com",
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

### <a name="perform-a-fuzzy-search"></a><span data-ttu-id="ef25c-189">Durchführen einer Fuzzysuche</span><span class="sxs-lookup"><span data-stu-id="ef25c-189">Perform a fuzzy search</span></span>

<span data-ttu-id="ef25c-190">Suchvorgänge implementieren einen Algorithmus für Fuzzyübereinstimmungen.</span><span class="sxs-lookup"><span data-stu-id="ef25c-190">Searches implement a fuzzy matching algorithm.</span></span> <span data-ttu-id="ef25c-191">Dabei werden Ergebnisse basierend auf einer exakten Übereinstimmung und auch zu Rückschlüssen zu der Absicht der Suche zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef25c-191">They will return results based on an exact match and also on inferences about the intent of the search.</span></span> <span data-ttu-id="ef25c-192">Verwenden wir als Beispiel einen Benutzer mit dem Anzeigenamen „Tyler Lee“ und der E-Mail-Adresse „tylerle@example.com“, der sich in der **people**-Sammlung des angemeldeten Benutzers befindet.</span><span class="sxs-lookup"><span data-stu-id="ef25c-192">For example, imagine a user with a display name of "Tyler Lee" and an email address of tylerle@example.com who is in the **people** collection of the signed-in user.</span></span> <span data-ttu-id="ef25c-193">Alle der folgenden Suchvorgänge geben den Benutzer „Tyler“ als eines der Ereignisse zurück.</span><span class="sxs-lookup"><span data-stu-id="ef25c-193">All of the following searches will return this user Tyler as one of the results.</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler"                //matches both Tyler's name and email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle"              //matches Tyler's email
GET https://graph.microsoft.com/v1.0/me/people?$search="tylerle@example.com"  //matches Tyler's email. Note the quotes to enclose '@'.
GET https://graph.microsoft.com/v1.0/me/people?$search="tiler"                //fuzzy match with Tyler's name
GET https://graph.microsoft.com/v1.0/me/people?$search="tyler lee"            //matches Tyler's name. Note the quotes to enclose the space.
```
