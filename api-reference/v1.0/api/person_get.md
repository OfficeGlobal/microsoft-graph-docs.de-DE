# <a name="get-person"></a><span data-ttu-id="cb15e-101">Get person</span><span class="sxs-lookup"><span data-stu-id="cb15e-101">Get person</span></span>

<span data-ttu-id="cb15e-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des [person](../resources/person.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="cb15e-102">Retrieve the properties and relationships of a [person](../resources/person.md) object.</span></span>

<span data-ttu-id="cb15e-p101">Sie können diese Informationen über die People API abrufen. Beispiele finden Sie in dem Abschnitt [Beispiele](#examples) sowie im Artikel zum Thema [Abrufen relevanter Informationen über Personen](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="cb15e-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cb15e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cb15e-105">Permissions</span></span>
<span data-ttu-id="cb15e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="cb15e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>
 

|<span data-ttu-id="cb15e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cb15e-108">Permission type</span></span>      | <span data-ttu-id="cb15e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cb15e-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="cb15e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cb15e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb15e-111">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb15e-111">People.Read, People.Read.All</span></span>    | 
|<span data-ttu-id="cb15e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cb15e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb15e-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="cb15e-113">People.Read</span></span>    | 
|<span data-ttu-id="cb15e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cb15e-114">Application</span></span> | <span data-ttu-id="cb15e-115">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="cb15e-115">People.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="cb15e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cb15e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cb15e-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cb15e-117">Optional query parameters</span></span>
|<span data-ttu-id="cb15e-118">Name</span><span class="sxs-lookup"><span data-stu-id="cb15e-118">Name</span></span>|<span data-ttu-id="cb15e-119">Wert</span><span class="sxs-lookup"><span data-stu-id="cb15e-119">Value</span></span>|<span data-ttu-id="cb15e-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb15e-120">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="cb15e-121">$filter</span><span class="sxs-lookup"><span data-stu-id="cb15e-121">$filter</span></span>|<span data-ttu-id="cb15e-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb15e-122">string</span></span>|<span data-ttu-id="cb15e-123">Dient zum Einschränken der Antwort auf diejenigen Personen, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="cb15e-123">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="cb15e-124">$orderby</span><span class="sxs-lookup"><span data-stu-id="cb15e-124">$orderby</span></span>|<span data-ttu-id="cb15e-125">string</span><span class="sxs-lookup"><span data-stu-id="cb15e-125">string</span></span>|<span data-ttu-id="cb15e-p103">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert. Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.</span><span class="sxs-lookup"><span data-stu-id="cb15e-p103">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="cb15e-128">$search</span><span class="sxs-lookup"><span data-stu-id="cb15e-128">$search</span></span>|<span data-ttu-id="cb15e-129">string</span><span class="sxs-lookup"><span data-stu-id="cb15e-129">string</span></span>|<span data-ttu-id="cb15e-p104">Dient für die Suche nach Personen anhand des Namens oder des Alias. Unterstützt Fuzzyübereinstimmung.</span><span class="sxs-lookup"><span data-stu-id="cb15e-p104">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="cb15e-132">$select</span><span class="sxs-lookup"><span data-stu-id="cb15e-132">$select</span></span>|<span data-ttu-id="cb15e-133">string</span><span class="sxs-lookup"><span data-stu-id="cb15e-133">string</span></span>|<span data-ttu-id="cb15e-p105">Durch Trennzeichen getrennte Liste der Eigenschaften, die in die Antwort eingeschlossen werden sollen. Wählen Sie für optimale Leistung nur eine Teilmenge der benötigten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="cb15e-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="cb15e-136">$skip</span><span class="sxs-lookup"><span data-stu-id="cb15e-136">$skip</span></span>|<span data-ttu-id="cb15e-137">int</span><span class="sxs-lookup"><span data-stu-id="cb15e-137">int</span></span>|<span data-ttu-id="cb15e-p106">Die ersten n Ergebnisse werden übersprungen. Hilfreich für Paging. Wird bei Verwendung von *$search* nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cb15e-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="cb15e-140">$top</span><span class="sxs-lookup"><span data-stu-id="cb15e-140">$top</span></span>|<span data-ttu-id="cb15e-141">int</span><span class="sxs-lookup"><span data-stu-id="cb15e-141">int</span></span>|<span data-ttu-id="cb15e-142">Anzahl der Ergebnisse, die zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="cb15e-142">Number of results to be returned.</span></span>|

## <a name="parameters"></a><span data-ttu-id="cb15e-143">Parameter</span><span class="sxs-lookup"><span data-stu-id="cb15e-143">Parameters</span></span>
| <span data-ttu-id="cb15e-144">Parameter</span><span class="sxs-lookup"><span data-stu-id="cb15e-144">Parameter</span></span> |<span data-ttu-id="cb15e-145">Typ</span><span class="sxs-lookup"><span data-stu-id="cb15e-145">Type</span></span>       |<span data-ttu-id="cb15e-146">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb15e-146">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="cb15e-147">property_value</span><span class="sxs-lookup"><span data-stu-id="cb15e-147">property_value</span></span>|<span data-ttu-id="cb15e-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb15e-148">String</span></span>     |<span data-ttu-id="cb15e-p107">Der Wert der erweiterten Eigenschaft, nach der gefiltert wird. Erforderlich, wo im Abschnitt **HTTP-Anforderung** aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="cb15e-p107">The value of the extended property to match. Required where listed in the **HTTP request** section.</span></span>|
|<span data-ttu-id="cb15e-151">person_property</span><span class="sxs-lookup"><span data-stu-id="cb15e-151">person_property</span></span>|<span data-ttu-id="cb15e-152">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cb15e-152">String</span></span>    |<span data-ttu-id="cb15e-p108">Die Eigenschaft der Person, die übereinstimmen muss. Erforderlich, wo im Abschnitt **HTTP-Anforderung** aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="cb15e-p108">The person property to match. Required where listed in the **HTTP request** section.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="cb15e-155">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cb15e-155">Request headers</span></span>
| <span data-ttu-id="cb15e-156">Name</span><span class="sxs-lookup"><span data-stu-id="cb15e-156">Name</span></span>      |<span data-ttu-id="cb15e-157">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cb15e-157">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cb15e-158">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb15e-158">Authorization</span></span>  | <span data-ttu-id="cb15e-p109">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cb15e-p109">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb15e-161">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cb15e-161">Request body</span></span>
<span data-ttu-id="cb15e-162">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cb15e-162">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="cb15e-163">Antwort</span><span class="sxs-lookup"><span data-stu-id="cb15e-163">Response</span></span>
<span data-ttu-id="cb15e-p110">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [person](../resources/person.md)-Objekt im Antworttext zurückgegeben. Die Antwort kann eine person-Instanz oder eine Sammlung von person-Instanzen enthalten.</span><span class="sxs-lookup"><span data-stu-id="cb15e-p110">If successful, this method returns a `200 OK` response code and a [person](../resources/person.md) object in the response body. The response can contain one person instance or a collection of person instances.</span></span> 
## <a name="examples"></a><span data-ttu-id="cb15e-166">Beispiele</span><span class="sxs-lookup"><span data-stu-id="cb15e-166">Examples</span></span>
### <a name="perform-a-search"></a><span data-ttu-id="cb15e-167">Durchführen einer Suche</span><span class="sxs-lookup"><span data-stu-id="cb15e-167">Perform a search</span></span> 
<span data-ttu-id="cb15e-168">Die folgende Anforderung führt eine Suche nach einer Person mit dem Namen „Irene McGowan“ durch.</span><span class="sxs-lookup"><span data-stu-id="cb15e-168">The following request does a search for a person named Irene McGowan.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

<span data-ttu-id="cb15e-169">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="cb15e-169">The following example shows the response.</span></span> 

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
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
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
### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="cb15e-170">Auswählen der Felder, die in einer gefilterten Antwort zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="cb15e-170">Select the fields to return in a filtered response</span></span> 
<span data-ttu-id="cb15e-171">Sie können die *$select*- und *$filter*-Parameter gemeinsam verwenden, um eine benutzerdefinierte Liste der für den Benutzer relevanten Personen zu erstellen und nur die Felder abzurufen, die Ihre Anwendung benötigt.</span><span class="sxs-lookup"><span data-stu-id="cb15e-171">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span> 

<span data-ttu-id="cb15e-p111">Im folgenden Beispiel wird **displayName** und **scoredEmailAddresses** von Personen angerufen, deren Anzeigenamen dem angegebenen Namen entspricht. In diesem Beispiel werden nur die Personen zurückgegeben, deren Anzeigename „Lorrie Frye“ lautet.</span><span class="sxs-lookup"><span data-stu-id="cb15e-p111">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="cb15e-174">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="cb15e-174">The following example shows the response.</span></span> 

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get person",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
