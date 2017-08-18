# <a name="list-people"></a><span data-ttu-id="3983d-101">List people</span><span class="sxs-lookup"><span data-stu-id="3983d-101">List people</span></span>

<span data-ttu-id="3983d-102">Dient zum Abrufen einer Sammlung von [person](../resources/person.md)-Objekten, die nach ihrer Relevanz für den [Benutzer](../resources/user.md) sortiert sind, die von den Mustern bei Kommunikation, Zusammenarbeit und den Geschäftsbeziehungen des Benutzers abhängt.</span><span class="sxs-lookup"><span data-stu-id="3983d-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="3983d-p101">Sie können diese Informationen über die People API abrufen. Beispiele finden Sie in dem Abschnitt [Beispiele](#examples) und im Artikel [Abrufen von relevanten Informationen über Personen](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="3983d-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3983d-105">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3983d-105">Prerequisites</span></span>
<span data-ttu-id="3983d-106">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen: *People.Read* *People.Read.All*</span><span class="sxs-lookup"><span data-stu-id="3983d-106">The following **scopes** are required to execute this API: *People.Read* *People.Read.All*</span></span>
 
## <a name="http-request"></a><span data-ttu-id="3983d-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3983d-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3983d-108">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3983d-108">Optional query parameters</span></span>
|<span data-ttu-id="3983d-109">Name</span><span class="sxs-lookup"><span data-stu-id="3983d-109">Name</span></span>|<span data-ttu-id="3983d-110">Wert</span><span class="sxs-lookup"><span data-stu-id="3983d-110">Value</span></span>|<span data-ttu-id="3983d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3983d-111">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="3983d-112">$filter</span><span class="sxs-lookup"><span data-stu-id="3983d-112">$filter</span></span>|<span data-ttu-id="3983d-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3983d-113">string</span></span>|<span data-ttu-id="3983d-114">Dient zum Einschränken der Antwort auf diejenigen Personen, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="3983d-114">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="3983d-115">$orderby</span><span class="sxs-lookup"><span data-stu-id="3983d-115">$orderby</span></span>|<span data-ttu-id="3983d-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3983d-116">string</span></span>|<span data-ttu-id="3983d-p102">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert. Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.</span><span class="sxs-lookup"><span data-stu-id="3983d-p102">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="3983d-119">$search</span><span class="sxs-lookup"><span data-stu-id="3983d-119">$search</span></span>|<span data-ttu-id="3983d-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3983d-120">string</span></span>|<span data-ttu-id="3983d-p103">Dient für die Suche nach Personen anhand des Namens oder des Alias. Unterstützt Fuzzyübereinstimmung.</span><span class="sxs-lookup"><span data-stu-id="3983d-p103">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="3983d-123">$select</span><span class="sxs-lookup"><span data-stu-id="3983d-123">$select</span></span>|<span data-ttu-id="3983d-124">string</span><span class="sxs-lookup"><span data-stu-id="3983d-124">string</span></span>|<span data-ttu-id="3983d-p104">Durch Trennzeichen getrennte Liste der Eigenschaften, die in die Antwort eingeschlossen werden sollen. Wählen Sie für optimale Leistung nur eine Teilmenge der benötigten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="3983d-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="3983d-127">$skip</span><span class="sxs-lookup"><span data-stu-id="3983d-127">$skip</span></span>|<span data-ttu-id="3983d-128">int</span><span class="sxs-lookup"><span data-stu-id="3983d-128">int</span></span>|<span data-ttu-id="3983d-p105">Die ersten n Ergebnisse werden übersprungen. Hilfreich für Paging. Wird bei Verwendung von *$search* nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3983d-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="3983d-131">$top</span><span class="sxs-lookup"><span data-stu-id="3983d-131">$top</span></span>|<span data-ttu-id="3983d-132">int</span><span class="sxs-lookup"><span data-stu-id="3983d-132">int</span></span>|<span data-ttu-id="3983d-133">Anzahl der Ergebnisse, die zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="3983d-133">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3983d-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3983d-134">Request headers</span></span>
| <span data-ttu-id="3983d-135">Name</span><span class="sxs-lookup"><span data-stu-id="3983d-135">Name</span></span>      |<span data-ttu-id="3983d-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3983d-136">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3983d-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="3983d-137">Authorization</span></span>  | <span data-ttu-id="3983d-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3983d-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3983d-140">Annehmen</span><span class="sxs-lookup"><span data-stu-id="3983d-140">Accept</span></span> | <span data-ttu-id="3983d-141">application/json</span><span class="sxs-lookup"><span data-stu-id="3983d-141">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3983d-142">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3983d-142">Request body</span></span>
<span data-ttu-id="3983d-143">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3983d-143">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3983d-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="3983d-144">Response</span></span>
<span data-ttu-id="3983d-p107">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [person](../resources/person.md)-Objekten im Antworttext zurückgegeben. Die Antwort kann ein person-Objekt oder eine Sammlung von person-Objekten enthalten.</span><span class="sxs-lookup"><span data-stu-id="3983d-p107">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span> 
## <a name="examples"></a><span data-ttu-id="3983d-147">Beispiele</span><span class="sxs-lookup"><span data-stu-id="3983d-147">Examples</span></span>

### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="3983d-148">Abrufen einer Sammlung relevanter Personen</span><span class="sxs-lookup"><span data-stu-id="3983d-148">Get a collection of relevant people</span></span> 

<span data-ttu-id="3983d-149">Mit der folgenden Anforderung werden die für den angemeldeten Benutzer relevantesten Personen (`/me`) auf Grundlage von Kommunikations- und Zusammenarbeitsmustern sowie Geschäftsbeziehungen abgerufen.</span><span class="sxs-lookup"><span data-stu-id="3983d-149">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="3983d-p108">Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mithilfe des *$top*-Abfrageparameters ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="3983d-p108">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
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
### <a name="search-other-users-relevant-people"></a><span data-ttu-id="3983d-154">Durchsuchen von für andere Benutzer relevanten Personen</span><span class="sxs-lookup"><span data-stu-id="3983d-154">Search other user’s relevant people</span></span>

<span data-ttu-id="3983d-p109">Die folgende Anforderung ruft die für eine andere Person in der Organisation des angemeldeten Benutzers relevanten Personen ab. Für diese Anforderung ist die Berechtigung People.Read.All erforderlich. In diesem Beispiel werden für Roscoe Seidel relevante Personen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="3983d-p109">The following request gets the people most relevant to another person in the signed-in user's organization. This request requires the People.Read.All permission. In this example, Roscoe Seidel's relevant people are displayed.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="3983d-p110">Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="3983d-p110">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
