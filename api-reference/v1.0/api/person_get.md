# <a name="get-person"></a><span data-ttu-id="1e6ae-101">Get person</span><span class="sxs-lookup"><span data-stu-id="1e6ae-101">Get person</span></span>

<span data-ttu-id="1e6ae-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des [person](../resources/person.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-102">Retrieve the properties and relationships of a [person](../resources/person.md) object.</span></span>

<span data-ttu-id="1e6ae-p101">Sie können diese Informationen über die People API abrufen. Beispiele finden Sie in dem Abschnitt [Beispiele](#examples) sowie im Artikel zum Thema [Abrufen relevanter Informationen über Personen](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="1e6ae-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1e6ae-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1e6ae-105">Permissions</span></span>
<span data-ttu-id="1e6ae-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1e6ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="1e6ae-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e6ae-108">Permission type</span></span>      | <span data-ttu-id="1e6ae-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e6ae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e6ae-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e6ae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1e6ae-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e6ae-111">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="1e6ae-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e6ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e6ae-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="1e6ae-113">People.Read</span></span>    |
|<span data-ttu-id="1e6ae-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e6ae-114">Application</span></span> | <span data-ttu-id="1e6ae-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e6ae-115">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e6ae-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e6ae-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/{id}
GET /users/{id | userPrincipalName}/people/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e6ae-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1e6ae-117">Optional query parameters</span></span>
<span data-ttu-id="1e6ae-118">Diese Methode unterstützt die folgende [OData-Abfrageparameter](../../../concepts/people_example.md) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-118">This method supports the [OData Query Parameters](../../../concepts/people_example.md) to help customize the response.</span></span>

|<span data-ttu-id="1e6ae-119">Name</span><span class="sxs-lookup"><span data-stu-id="1e6ae-119">Name</span></span>|<span data-ttu-id="1e6ae-120">Wert</span><span class="sxs-lookup"><span data-stu-id="1e6ae-120">Value</span></span>|<span data-ttu-id="1e6ae-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e6ae-121">Description</span></span>| 
|:---------------|:--------|:-------| 
|<span data-ttu-id="1e6ae-122">$filter</span><span class="sxs-lookup"><span data-stu-id="1e6ae-122">$filter</span></span>|<span data-ttu-id="1e6ae-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e6ae-123">string</span></span>|<span data-ttu-id="1e6ae-124">Dient zum Einschränken der Antwort auf diejenigen Personen, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-124">Limits the response to only those people whose record contains the specified criteria.</span></span>| 
|<span data-ttu-id="1e6ae-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="1e6ae-125">$orderby</span></span>|<span data-ttu-id="1e6ae-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e6ae-126">string</span></span>|<span data-ttu-id="1e6ae-127">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-127">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the $orderby parameter.</span></span> <span data-ttu-id="1e6ae-128">Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-128">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>| 
|<span data-ttu-id="1e6ae-129">$search</span><span class="sxs-lookup"><span data-stu-id="1e6ae-129">$search</span></span>|<span data-ttu-id="1e6ae-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="1e6ae-130">string</span></span>|<span data-ttu-id="1e6ae-131">Dient für die Suche nach Personen anhand des Namens oder des Alias.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-131">Search for people by name or alias. Supports fuzzy matching.</span></span> <span data-ttu-id="1e6ae-132">Unterstützt Fuzzyübereinstimmung.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-132">Supports Fuzzy matching</span></span>| 
|<span data-ttu-id="1e6ae-133">$select</span><span class="sxs-lookup"><span data-stu-id="1e6ae-133">$select</span></span>|<span data-ttu-id="1e6ae-134">string</span><span class="sxs-lookup"><span data-stu-id="1e6ae-134">string</span></span>|<span data-ttu-id="1e6ae-p105">Durch Trennzeichen getrennte Liste der Eigenschaften, die in die Antwort eingeschlossen werden sollen. Wählen Sie für optimale Leistung nur eine Teilmenge der benötigten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>| 
|<span data-ttu-id="1e6ae-137">$skip</span><span class="sxs-lookup"><span data-stu-id="1e6ae-137">$skip</span></span>|<span data-ttu-id="1e6ae-138">int</span><span class="sxs-lookup"><span data-stu-id="1e6ae-138">int</span></span>|<span data-ttu-id="1e6ae-p106">Die ersten n Ergebnisse werden übersprungen. Hilfreich für Paging. Wird bei Verwendung von *$search* nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>| 
|<span data-ttu-id="1e6ae-141">$top</span><span class="sxs-lookup"><span data-stu-id="1e6ae-141">$top</span></span>|<span data-ttu-id="1e6ae-142">int</span><span class="sxs-lookup"><span data-stu-id="1e6ae-142">int</span></span>|<span data-ttu-id="1e6ae-143">Anzahl der Ergebnisse, die zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-143">Number of results to be returned.</span></span>| 

## <a name="request-headers"></a><span data-ttu-id="1e6ae-144">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e6ae-144">Request headers</span></span>
| <span data-ttu-id="1e6ae-145">Name</span><span class="sxs-lookup"><span data-stu-id="1e6ae-145">Name</span></span>      |<span data-ttu-id="1e6ae-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e6ae-146">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1e6ae-147">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e6ae-147">Authorization</span></span>  | <span data-ttu-id="1e6ae-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e6ae-150">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e6ae-150">Request body</span></span>
<span data-ttu-id="1e6ae-151">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-151">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e6ae-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e6ae-152">Response</span></span>
<span data-ttu-id="1e6ae-153">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [person](../resources/person.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-153">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/person.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1e6ae-154">Beispiele</span><span class="sxs-lookup"><span data-stu-id="1e6ae-154">Examples</span></span>
#### <a name="request-1"></a><span data-ttu-id="1e6ae-155">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="1e6ae-155">Request 1</span></span>
<span data-ttu-id="1e6ae-156">Nachfolgend sehen Sie ein Beispiel der Anforderung, die die Person mit dieser ID in der Organisation des Benutzers abruft.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-156">The following is an example of the request that gets the person who has this ID in the user's organization.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person_by_id"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people/e3d0513b-449e-4198-ba6f-bd97ae7cae85
```

#### <a name="response-1"></a><span data-ttu-id="1e6ae-157">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="1e6ae-157">Response 1</span></span>
<span data-ttu-id="1e6ae-158">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-158">Here is an example of the response.</span></span>

><span data-ttu-id="1e6ae-159">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1e6ae-160">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-160">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_by_id",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 629

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
```

#### <a name="request-2"></a><span data-ttu-id="1e6ae-161">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="1e6ae-161">Request 2</span></span>
<span data-ttu-id="1e6ae-162">Nachfolgend sehen Sie ein Beispiel der Anforderung, die die Person mit dieser ID in der Organisation des Benutzers abruft und die Antwort auf die ausgewählten Eigenschaften beschränkt.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-162">The following is an example of the request that gets the person who has this ID in the user's organization and restricts the response to the selected properties.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_by_id_with_select"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/people/e3d0513b-449e-4198-ba6f-bd97ae7cae85?$select=displayName
```
#### <a name="response-2"></a><span data-ttu-id="1e6ae-163">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="1e6ae-163">Response 2</span></span>
<span data-ttu-id="1e6ae-164">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-164">Here is an example of the response.</span></span>

><span data-ttu-id="1e6ae-165">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-165">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="1e6ae-166">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="1e6ae-166">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_by_id_with_select",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 305

{
  "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
  "displayName": "Isaiah Langer"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get person",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
