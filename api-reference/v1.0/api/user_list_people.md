# <a name="list-people"></a><span data-ttu-id="87efe-101">Personen auflisten</span><span class="sxs-lookup"><span data-stu-id="87efe-101">List people</span></span>

<span data-ttu-id="87efe-102">Dient zum Abrufen einer Sammlung von [person](../resources/person.md)-Objekten, die nach ihrer Relevanz für den [Benutzer](../resources/user.md) sortiert sind, die von den Mustern bei Kommunikation, Zusammenarbeit und den Geschäftsbeziehungen des Benutzers abhängt.</span><span class="sxs-lookup"><span data-stu-id="87efe-102">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="87efe-p101">Sie können diese Informationen über die People API abrufen. Beispiele finden Sie in dem Abschnitt [Beispiele](#examples) sowie im Artikel zum Thema [Abrufen relevanter Informationen über Personen](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="87efe-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="87efe-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="87efe-105">Permissions</span></span>

<span data-ttu-id="87efe-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="87efe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87efe-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="87efe-108">Permission type</span></span>      | <span data-ttu-id="87efe-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="87efe-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87efe-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="87efe-110">Delegated (work or school account)</span></span> | <span data-ttu-id="87efe-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="87efe-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="87efe-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="87efe-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87efe-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="87efe-113">People.Read</span></span>    |
|<span data-ttu-id="87efe-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="87efe-114">Application</span></span> | <span data-ttu-id="87efe-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="87efe-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="87efe-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="87efe-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87efe-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="87efe-117">Optional query parameters</span></span>

<span data-ttu-id="87efe-118">Diese Methode unterstützt die [OData-Abfrageparameter](../../../concepts/query_parameters.md), um bei der Anpassung der Antwort zu helfen. Beispiele dazu finden Sie im Artikel [Abrufen relevanter Informationen über Personen](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="87efe-118">This method supports the [OData query parameters](../../../concepts/query_parameters.md) to help customize the response, as shown in the examples in the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

|<span data-ttu-id="87efe-119">Name</span><span class="sxs-lookup"><span data-stu-id="87efe-119">Name</span></span>|<span data-ttu-id="87efe-120">Wert</span><span class="sxs-lookup"><span data-stu-id="87efe-120">Value</span></span>|<span data-ttu-id="87efe-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87efe-121">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="87efe-122">$filter</span><span class="sxs-lookup"><span data-stu-id="87efe-122">$filter</span></span>|<span data-ttu-id="87efe-123">string</span><span class="sxs-lookup"><span data-stu-id="87efe-123">string</span></span>|<span data-ttu-id="87efe-124">Dient zum Einschränken der Antwort auf diejenigen Personen, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="87efe-124">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="87efe-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="87efe-125">$orderby</span></span>|<span data-ttu-id="87efe-126">string</span><span class="sxs-lookup"><span data-stu-id="87efe-126">string</span></span>|<span data-ttu-id="87efe-127">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert.</span><span class="sxs-lookup"><span data-stu-id="87efe-127">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="87efe-128">Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.</span><span class="sxs-lookup"><span data-stu-id="87efe-128">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="87efe-129">$search</span><span class="sxs-lookup"><span data-stu-id="87efe-129">$search</span></span>|<span data-ttu-id="87efe-130">string</span><span class="sxs-lookup"><span data-stu-id="87efe-130">string</span></span>|<span data-ttu-id="87efe-131">Dient für die Suche nach Personen anhand des Namens oder des Alias.</span><span class="sxs-lookup"><span data-stu-id="87efe-131">Search for people by name or alias.</span></span> <span data-ttu-id="87efe-132">Unterstützt Fuzzyübereinstimmung.</span><span class="sxs-lookup"><span data-stu-id="87efe-132">Supports Fuzzy matching.</span></span> <span data-ttu-id="87efe-133">Der Parameter funktioniert nur für die Suche der relevanten Personen des angemeldeten Benutzers, nicht zum Suchen von Personen, die für andere Benutzer relevant sind.</span><span class="sxs-lookup"><span data-stu-id="87efe-133">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="87efe-134">Unterstützt außerdem die `topic` Schlüsselwort-Personensuche basierend auf Themen, die aus E-Mail-Konversationen mit dieser Person extrahiert wurden.</span><span class="sxs-lookup"><span data-stu-id="87efe-134">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="87efe-135">Siehe Abschnitt *Eine Fuzzy-Suche ausführen* unter [Abrufen von relevanten Informationen über Personen](../../../concepts/people_example.md#perform-a-fuzzy-search) für Informationen und Beispiele.</span><span class="sxs-lookup"><span data-stu-id="87efe-135">See the *Perform a fuzzy search* section at [Get relevant information about people](../../../concepts/people_example.md#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="87efe-136">$select</span><span class="sxs-lookup"><span data-stu-id="87efe-136">$select</span></span>|<span data-ttu-id="87efe-137">string</span><span class="sxs-lookup"><span data-stu-id="87efe-137">string</span></span>|<span data-ttu-id="87efe-p105">Durch Trennzeichen getrennte Liste der Eigenschaften, die in die Antwort eingeschlossen werden sollen. Wählen Sie für optimale Leistung nur eine Teilmenge der benötigten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="87efe-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="87efe-140">$skip</span><span class="sxs-lookup"><span data-stu-id="87efe-140">$skip</span></span>|<span data-ttu-id="87efe-141">int</span><span class="sxs-lookup"><span data-stu-id="87efe-141">int</span></span>|<span data-ttu-id="87efe-p106">Die ersten n Ergebnisse werden übersprungen. Hilfreich für Paging. Wird bei Verwendung von *$search* nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="87efe-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="87efe-144">$top</span><span class="sxs-lookup"><span data-stu-id="87efe-144">$top</span></span>|<span data-ttu-id="87efe-145">int</span><span class="sxs-lookup"><span data-stu-id="87efe-145">int</span></span>|<span data-ttu-id="87efe-146">Anzahl der Ergebnisse, die zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="87efe-146">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="87efe-147">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="87efe-147">Request headers</span></span>

| <span data-ttu-id="87efe-148">Name</span><span class="sxs-lookup"><span data-stu-id="87efe-148">Name</span></span>      |<span data-ttu-id="87efe-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="87efe-149">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="87efe-150">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="87efe-150">Authorization</span></span>  | <span data-ttu-id="87efe-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="87efe-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="87efe-153">Akzeptieren</span><span class="sxs-lookup"><span data-stu-id="87efe-153">Accept</span></span> | <span data-ttu-id="87efe-154">Anwendung/json</span><span class="sxs-lookup"><span data-stu-id="87efe-154">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="87efe-155">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="87efe-155">Request body</span></span>

<span data-ttu-id="87efe-156">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="87efe-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87efe-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="87efe-157">Response</span></span>

<span data-ttu-id="87efe-p108">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [person](../resources/person.md)-Objekten im Antworttext zurückgegeben. Die Antwort kann ein person-Objekt oder eine Sammlung von person-Objekten enthalten.</span><span class="sxs-lookup"><span data-stu-id="87efe-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="87efe-160">Beispiele</span><span class="sxs-lookup"><span data-stu-id="87efe-160">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="87efe-161">Anforderung</span><span class="sxs-lookup"><span data-stu-id="87efe-161">Request</span></span>

<span data-ttu-id="87efe-162">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="87efe-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="87efe-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="87efe-163">Response</span></span>

<span data-ttu-id="87efe-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="87efe-164">The following is an example of the response.</span></span>

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

<span data-ttu-id="87efe-165">Weitere Beispiele finden Sie im Artikel [Abrufen relevanter Informationen über Personen](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="87efe-165">For more examples, see the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
