# <a name="list-people"></a><span data-ttu-id="87ed1-101">Personen auflisten</span><span class="sxs-lookup"><span data-stu-id="87ed1-101">List people</span></span>

<span data-ttu-id="87ed1-102">Dient zum Abrufen einer Sammlung von [person](../resources/person.md)-Objekten, die nach ihrer Relevanz für den [Benutzer](../resources/user.md) sortiert sind, die von den Mustern bei Kommunikation, Zusammenarbeit und den Geschäftsbeziehungen des Benutzers abhängt.</span><span class="sxs-lookup"><span data-stu-id="87ed1-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns and business relationships.</span></span>

<span data-ttu-id="87ed1-p101">Sie können diese Informationen über die People API abrufen. Beispiele finden Sie in dem Abschnitt [Beispiele](#examples) sowie im Artikel zum Thema [Abrufen relevanter Informationen über Personen](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="87ed1-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="87ed1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87ed1-105">Permissions</span></span>
<span data-ttu-id="87ed1-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87ed1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87ed1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87ed1-108">Permission type</span></span>      | <span data-ttu-id="87ed1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87ed1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87ed1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87ed1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="87ed1-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="87ed1-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="87ed1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87ed1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87ed1-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="87ed1-113">People.Read</span></span>    |
|<span data-ttu-id="87ed1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87ed1-114">Application</span></span> | <span data-ttu-id="87ed1-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="87ed1-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87ed1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87ed1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87ed1-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="87ed1-117">Optional query parameters</span></span>
<span data-ttu-id="87ed1-118">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/people_example.md) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87ed1-118">This method supports the [OData Query Parameters](../../../concepts/people_example.md) to help customize the response.</span></span>

|<span data-ttu-id="87ed1-119">Name</span><span class="sxs-lookup"><span data-stu-id="87ed1-119">Name</span></span>|<span data-ttu-id="87ed1-120">Wert</span><span class="sxs-lookup"><span data-stu-id="87ed1-120">Value</span></span>|<span data-ttu-id="87ed1-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87ed1-121">Description</span></span>| 
|:---------------|:--------|:-------| 
|<span data-ttu-id="87ed1-122">$filter</span><span class="sxs-lookup"><span data-stu-id="87ed1-122">$filter</span></span>|<span data-ttu-id="87ed1-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87ed1-123">string</span></span>|<span data-ttu-id="87ed1-124">Dient zum Einschränken der Antwort auf diejenigen Personen, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="87ed1-124">Limits the response to only those people whose record contains the specified criteria.</span></span>| 
|<span data-ttu-id="87ed1-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="87ed1-125">$orderby</span></span>|<span data-ttu-id="87ed1-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87ed1-126">string</span></span>|<span data-ttu-id="87ed1-127">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert.</span><span class="sxs-lookup"><span data-stu-id="87ed1-127">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the $orderby parameter.</span></span> <span data-ttu-id="87ed1-128">Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.</span><span class="sxs-lookup"><span data-stu-id="87ed1-128">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>| 
|<span data-ttu-id="87ed1-129">$search</span><span class="sxs-lookup"><span data-stu-id="87ed1-129">$search</span></span>|<span data-ttu-id="87ed1-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="87ed1-130">string</span></span>|<span data-ttu-id="87ed1-131">Dient für die Suche nach Personen anhand des Namens oder des Alias.</span><span class="sxs-lookup"><span data-stu-id="87ed1-131">Search for people by name or alias. Supports fuzzy matching.</span></span> <span data-ttu-id="87ed1-132">Unterstützt Fuzzyübereinstimmung.</span><span class="sxs-lookup"><span data-stu-id="87ed1-132">Supports Fuzzy matching</span></span>| 
|<span data-ttu-id="87ed1-133">$select</span><span class="sxs-lookup"><span data-stu-id="87ed1-133">$select</span></span>|<span data-ttu-id="87ed1-134">string</span><span class="sxs-lookup"><span data-stu-id="87ed1-134">string</span></span>|<span data-ttu-id="87ed1-p105">Durch Trennzeichen getrennte Liste der Eigenschaften, die in die Antwort eingeschlossen werden sollen. Wählen Sie für optimale Leistung nur eine Teilmenge der benötigten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="87ed1-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>| 
|<span data-ttu-id="87ed1-137">$skip</span><span class="sxs-lookup"><span data-stu-id="87ed1-137">$skip</span></span>|<span data-ttu-id="87ed1-138">int</span><span class="sxs-lookup"><span data-stu-id="87ed1-138">int</span></span>|<span data-ttu-id="87ed1-p106">Die ersten n Ergebnisse werden übersprungen. Hilfreich für Paging. Wird bei Verwendung von *$search* nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87ed1-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>| 
|<span data-ttu-id="87ed1-141">$top</span><span class="sxs-lookup"><span data-stu-id="87ed1-141">$top</span></span>|<span data-ttu-id="87ed1-142">int</span><span class="sxs-lookup"><span data-stu-id="87ed1-142">int</span></span>|<span data-ttu-id="87ed1-143">Anzahl der Ergebnisse, die zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="87ed1-143">Number of results to be returned.</span></span>| 

## <a name="request-headers"></a><span data-ttu-id="87ed1-144">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87ed1-144">Request headers</span></span>
| <span data-ttu-id="87ed1-145">Name</span><span class="sxs-lookup"><span data-stu-id="87ed1-145">Name</span></span>      |<span data-ttu-id="87ed1-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87ed1-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="87ed1-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="87ed1-147">Authorization</span></span>  | <span data-ttu-id="87ed1-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87ed1-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87ed1-150">Annehmen</span><span class="sxs-lookup"><span data-stu-id="87ed1-150">Accept</span></span> | <span data-ttu-id="87ed1-151">application/json</span><span class="sxs-lookup"><span data-stu-id="87ed1-151">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="87ed1-152">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87ed1-152">Request body</span></span>
<span data-ttu-id="87ed1-153">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="87ed1-153">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87ed1-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="87ed1-154">Response</span></span>
<span data-ttu-id="87ed1-p108">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [person](../resources/person.md)-Objekten im Antworttext zurückgegeben. Die Antwort kann ein person-Objekt oder eine Sammlung von person-Objekten enthalten.</span><span class="sxs-lookup"><span data-stu-id="87ed1-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="87ed1-157">Beispiele</span><span class="sxs-lookup"><span data-stu-id="87ed1-157">Examples</span></span>
#### <a name="request"></a><span data-ttu-id="87ed1-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87ed1-158">Request</span></span>
<span data-ttu-id="87ed1-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87ed1-159">The following is an example of making the request in ASP.NET that uses the TokenHelper file:</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="87ed1-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="87ed1-160">Response</span></span>
<span data-ttu-id="87ed1-161">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87ed1-161">Here is an example of the response.</span></span>

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
Content-length: 1370

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
                    "address": "Marketing@contoso.com",
                    "relevanceScore": 30.0
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "personType": {
                "class": "Group",
                "subclass": "UnifiedGroup"
            }
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "jobTitle": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "userPrincipalName": "IsaiahL@contoso.com",
            "imAddress": "sip:isaiahl@contoso.com",
            "scoredEmailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "relevanceScore": 20.0
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
            "personType": {
                "class": "Person",
                "subclass": "OrganizationUser"
            }
        }
    ]
}
```

<span data-ttu-id="87ed1-162">Weitere Beispiele finden Sie im Artikel [Abrufen relevanter Informationen über Personen](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="87ed1-162">For more examples, see the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
