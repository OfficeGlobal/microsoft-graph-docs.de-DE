# <a name="list-people"></a><span data-ttu-id="bc25f-101">List people</span><span class="sxs-lookup"><span data-stu-id="bc25f-101">List people</span></span>

<span data-ttu-id="bc25f-102">Dient zum Abrufen einer Sammlung von [person](../resources/person.md)-Objekten, die nach ihrer Relevanz für den [Benutzer](../resources/user.md) sortiert sind, die von den Mustern bei Kommunikation, Zusammenarbeit und den Geschäftsbeziehungen des Benutzers abhängt.</span><span class="sxs-lookup"><span data-stu-id="bc25f-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="bc25f-p101">Sie können diese Informationen über die People API abrufen. Beispiele finden Sie in dem Abschnitt [Beispiele](#examples) sowie im Artikel zum Thema [Abrufen relevanter Informationen über Personen](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="bc25f-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bc25f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bc25f-105">Permissions</span></span>
<span data-ttu-id="bc25f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="bc25f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="bc25f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc25f-108">Permission type</span></span>      | <span data-ttu-id="bc25f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc25f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc25f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc25f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc25f-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc25f-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="bc25f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc25f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc25f-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="bc25f-113">People.Read</span></span>    |
|<span data-ttu-id="bc25f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc25f-114">Application</span></span> | <span data-ttu-id="bc25f-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc25f-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc25f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc25f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bc25f-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bc25f-117">Optional query parameters</span></span>
|<span data-ttu-id="bc25f-118">Name</span><span class="sxs-lookup"><span data-stu-id="bc25f-118">Name</span></span>|<span data-ttu-id="bc25f-119">Wert</span><span class="sxs-lookup"><span data-stu-id="bc25f-119">Value</span></span>|<span data-ttu-id="bc25f-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc25f-120">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="bc25f-121">$filter</span><span class="sxs-lookup"><span data-stu-id="bc25f-121">$filter</span></span>|<span data-ttu-id="bc25f-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc25f-122">string</span></span>|<span data-ttu-id="bc25f-123">Dient zum Einschränken der Antwort auf diejenigen Personen, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="bc25f-123">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="bc25f-124">$orderby</span><span class="sxs-lookup"><span data-stu-id="bc25f-124">$orderby</span></span>|<span data-ttu-id="bc25f-125">string</span><span class="sxs-lookup"><span data-stu-id="bc25f-125">string</span></span>|<span data-ttu-id="bc25f-p103">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert. Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.</span><span class="sxs-lookup"><span data-stu-id="bc25f-p103">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response by using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="bc25f-128">$search</span><span class="sxs-lookup"><span data-stu-id="bc25f-128">$search</span></span>|<span data-ttu-id="bc25f-129">string</span><span class="sxs-lookup"><span data-stu-id="bc25f-129">string</span></span>|<span data-ttu-id="bc25f-p104">Dient für die Suche nach Personen anhand des Namens oder des Alias. Unterstützt Fuzzyübereinstimmung.</span><span class="sxs-lookup"><span data-stu-id="bc25f-p104">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="bc25f-132">$select</span><span class="sxs-lookup"><span data-stu-id="bc25f-132">$select</span></span>|<span data-ttu-id="bc25f-133">string</span><span class="sxs-lookup"><span data-stu-id="bc25f-133">string</span></span>|<span data-ttu-id="bc25f-p105">Durch Trennzeichen getrennte Liste der Eigenschaften, die in die Antwort eingeschlossen werden sollen. Wählen Sie für optimale Leistung nur eine Teilmenge der benötigten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="bc25f-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="bc25f-136">$skip</span><span class="sxs-lookup"><span data-stu-id="bc25f-136">$skip</span></span>|<span data-ttu-id="bc25f-137">int</span><span class="sxs-lookup"><span data-stu-id="bc25f-137">int</span></span>|<span data-ttu-id="bc25f-p106">Die ersten n Ergebnisse werden übersprungen. Hilfreich für Paging. Wird bei Verwendung von *$search* nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc25f-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="bc25f-140">$top</span><span class="sxs-lookup"><span data-stu-id="bc25f-140">$top</span></span>|<span data-ttu-id="bc25f-141">int</span><span class="sxs-lookup"><span data-stu-id="bc25f-141">int</span></span>|<span data-ttu-id="bc25f-142">Anzahl der Ergebnisse, die zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="bc25f-142">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="bc25f-143">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc25f-143">Request headers</span></span>
| <span data-ttu-id="bc25f-144">Name</span><span class="sxs-lookup"><span data-stu-id="bc25f-144">Name</span></span>      |<span data-ttu-id="bc25f-145">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc25f-145">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="bc25f-146">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc25f-146">Authorization</span></span>  | <span data-ttu-id="bc25f-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc25f-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bc25f-149">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bc25f-149">Accept</span></span> | <span data-ttu-id="bc25f-150">application/json</span><span class="sxs-lookup"><span data-stu-id="bc25f-150">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bc25f-151">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc25f-151">Request body</span></span>
<span data-ttu-id="bc25f-152">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bc25f-152">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bc25f-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc25f-153">Response</span></span>
<span data-ttu-id="bc25f-p108">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [person](../resources/person.md)-Objekten im Antworttext zurückgegeben. Die Antwort kann ein person-Objekt oder eine Sammlung von person-Objekten enthalten.</span><span class="sxs-lookup"><span data-stu-id="bc25f-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span> 
## <a name="examples"></a><span data-ttu-id="bc25f-156">Beispiele</span><span class="sxs-lookup"><span data-stu-id="bc25f-156">Examples</span></span>

### <a name="get-a-collection-of-relevant-people"></a><span data-ttu-id="bc25f-157">Abrufen einer Sammlung relevanter Personen</span><span class="sxs-lookup"><span data-stu-id="bc25f-157">Get a collection of relevant people</span></span> 

<span data-ttu-id="bc25f-158">Mit der folgenden Anforderung werden die für den angemeldeten Benutzer relevantesten Personen (`/me`) auf Grundlage von Kommunikations- und Zusammenarbeitsmustern sowie Geschäftsbeziehungen abgerufen.</span><span class="sxs-lookup"><span data-stu-id="bc25f-158">The following request gets the people most relevant to the signed-in user (`/me`), based on communication and collaboration patterns and business relationships.</span></span> 
<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/
```

<span data-ttu-id="bc25f-p109">Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mithilfe des *$top*-Abfrageparameters ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="bc25f-p109">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>
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
### <a name="search-other-users-relevant-people"></a><span data-ttu-id="bc25f-163">Durchsuchen von für andere Benutzer relevanten Personen</span><span class="sxs-lookup"><span data-stu-id="bc25f-163">Search other user’s relevant people</span></span>

<span data-ttu-id="bc25f-p110">Die folgende Anforderung ruft die für eine andere Person in der Organisation des angemeldeten Benutzers relevanten Personen ab. Für diese Anforderung ist die Berechtigung People.Read.All erforderlich. In diesem Beispiel werden für Roscoe Seidel relevante Personen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="bc25f-p110">The following request gets the people most relevant to another person in the signed-in user's organization. This request requires the People.Read.All permission. In this example, Roscoe Seidel's relevant people are displayed.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/users('roscoes@contoso.com')/people/
```

<span data-ttu-id="bc25f-p111">Das folgende Beispiel zeigt die Antwort. Standardmäßig gibt jeder Antwort 10 Datensätze zurück. Sie können diese Einstellung mit dem *$top*-Parameter ändern. In diesem Beispiel wird *$top* verwendet, um die Anzahl der Antworten auf drei Datensätze einzuschränken.</span><span class="sxs-lookup"><span data-stu-id="bc25f-p111">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* parameter. This example uses *$top* to limit the response to three records.</span></span>

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
