# <a name="get-person"></a><span data-ttu-id="3b9d3-101">Get person</span><span class="sxs-lookup"><span data-stu-id="3b9d3-101">Get person</span></span>

<span data-ttu-id="3b9d3-102">Dient zum Abrufen der Eigenschaften und der Beziehungen des [person](../resources/person.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-102">Retrieve the properties and relationships of [plannerAssignedToTaskBoardTaskFormat](../resources/person.md) object.</span></span>

<span data-ttu-id="3b9d3-p101">Sie können diese Informationen über die People API abrufen. Beispiele finden Sie in dem Abschnitt [Beispiele](#examples) und im Artikel [Abrufen von relevanten Informationen über Personen](../../../concepts/people_example.md).</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](../../../concepts/people_example.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b9d3-105">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="3b9d3-105">Prerequisites</span></span>
<span data-ttu-id="3b9d3-106">Die folgenden **Berechtigungen** sind erforderlich, um Teile dieses APIs auszuführen: *People.Read*; *People.Read.All*</span><span class="sxs-lookup"><span data-stu-id="3b9d3-106">The following **permissions** are required to execute portions of this API: *People.Read*; *People.Read.All*</span></span>
 
## <a name="http-request"></a><span data-ttu-id="3b9d3-107">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3b9d3-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/people/?$search='{property_value}'
GET /me/people/?$filter={person_property} eq '{property_value}'
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b9d3-108">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3b9d3-108">Optional query parameters</span></span>
|<span data-ttu-id="3b9d3-109">Name</span><span class="sxs-lookup"><span data-stu-id="3b9d3-109">Name</span></span>|<span data-ttu-id="3b9d3-110">Wert</span><span class="sxs-lookup"><span data-stu-id="3b9d3-110">Value</span></span>|<span data-ttu-id="3b9d3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b9d3-111">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="3b9d3-112">$filter</span><span class="sxs-lookup"><span data-stu-id="3b9d3-112">$filter</span></span>|<span data-ttu-id="3b9d3-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b9d3-113">string</span></span>|<span data-ttu-id="3b9d3-114">Dient zum Einschränken der Antwort auf diejenigen Personen, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-114">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="3b9d3-115">$orderby</span><span class="sxs-lookup"><span data-stu-id="3b9d3-115">$orderby</span></span>|<span data-ttu-id="3b9d3-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b9d3-116">string</span></span>|<span data-ttu-id="3b9d3-p102">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert. Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p102">By default, the people in the response are sorted by their relevance to your query. You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="3b9d3-119">$search</span><span class="sxs-lookup"><span data-stu-id="3b9d3-119">$search</span></span>|<span data-ttu-id="3b9d3-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b9d3-120">string</span></span>|<span data-ttu-id="3b9d3-p103">Dient für die Suche nach Personen anhand des Namens oder des Alias. Unterstützt Fuzzyübereinstimmung.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p103">Search for people by name or alias. Supports fuzzy matching.</span></span>|
|<span data-ttu-id="3b9d3-123">$select</span><span class="sxs-lookup"><span data-stu-id="3b9d3-123">$select</span></span>|<span data-ttu-id="3b9d3-124">string</span><span class="sxs-lookup"><span data-stu-id="3b9d3-124">string</span></span>|<span data-ttu-id="3b9d3-p104">Durch Trennzeichen getrennte Liste der Eigenschaften, die in die Antwort eingeschlossen werden sollen. Wählen Sie für optimale Leistung nur eine Teilmenge der benötigten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="3b9d3-127">$skip</span><span class="sxs-lookup"><span data-stu-id="3b9d3-127">$skip</span></span>|<span data-ttu-id="3b9d3-128">int</span><span class="sxs-lookup"><span data-stu-id="3b9d3-128">int</span></span>|<span data-ttu-id="3b9d3-p105">Die ersten n Ergebnisse werden übersprungen. Hilfreich für Paging. Wird bei Verwendung von *$search* nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="3b9d3-131">$top</span><span class="sxs-lookup"><span data-stu-id="3b9d3-131">$top</span></span>|<span data-ttu-id="3b9d3-132">int</span><span class="sxs-lookup"><span data-stu-id="3b9d3-132">int</span></span>|<span data-ttu-id="3b9d3-133">Anzahl der Ergebnisse, die zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-133">Number of results to be returned.</span></span>|

## <a name="parameters"></a><span data-ttu-id="3b9d3-134">Parameter</span><span class="sxs-lookup"><span data-stu-id="3b9d3-134">Parameters</span></span>
| <span data-ttu-id="3b9d3-135">Parameter</span><span class="sxs-lookup"><span data-stu-id="3b9d3-135">Parameter</span></span> |<span data-ttu-id="3b9d3-136">Typ</span><span class="sxs-lookup"><span data-stu-id="3b9d3-136">Type</span></span>       |<span data-ttu-id="3b9d3-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b9d3-137">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="3b9d3-138">property_value</span><span class="sxs-lookup"><span data-stu-id="3b9d3-138">property_value</span></span>|<span data-ttu-id="3b9d3-139">String</span><span class="sxs-lookup"><span data-stu-id="3b9d3-139">String</span></span>     |<span data-ttu-id="3b9d3-p106">Der Wert der erweiterten Eigenschaft, nach der gefiltert wird. Erforderlich, wo im Abschnitt **HTTP-Anforderung** aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p106">The value of the extended property to match. Required where listed in the HTTP request section above.</span></span>|
|<span data-ttu-id="3b9d3-142">person_property</span><span class="sxs-lookup"><span data-stu-id="3b9d3-142">person_property</span></span>|<span data-ttu-id="3b9d3-143">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3b9d3-143">String</span></span>    |<span data-ttu-id="3b9d3-p107">Die Eigenschaft der Person, die übereinstimmen muss. Erforderlich, wo im Abschnitt **HTTP-Anforderung** aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p107">The value of the extended property to match. Required where listed in the HTTP request section above.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="3b9d3-146">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3b9d3-146">Request headers</span></span>
| <span data-ttu-id="3b9d3-147">Name</span><span class="sxs-lookup"><span data-stu-id="3b9d3-147">Name</span></span>      |<span data-ttu-id="3b9d3-148">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3b9d3-148">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3b9d3-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b9d3-149">Authorization</span></span>  | <span data-ttu-id="3b9d3-p108">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3b9d3-152">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3b9d3-152">Request body</span></span>
<span data-ttu-id="3b9d3-153">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-153">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3b9d3-154">Antwort</span><span class="sxs-lookup"><span data-stu-id="3b9d3-154">Response</span></span>
<span data-ttu-id="3b9d3-p109">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [person](../resources/person.md)-Objekt im Antworttext zurückgegeben. Die Antwort kann eine person-Instanz oder eine Sammlung von person-Instanzen enthalten.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p109">If successful, this method returns a `200 OK` response code and a [person](../resources/person.md) object in the response body. The response can contain one person instance or a collection of person instances.</span></span> 
## <a name="examples"></a><span data-ttu-id="3b9d3-157">Beispiele</span><span class="sxs-lookup"><span data-stu-id="3b9d3-157">Examples</span></span>
### <a name="perform-a-search"></a><span data-ttu-id="3b9d3-158">Durchführen einer Suche</span><span class="sxs-lookup"><span data-stu-id="3b9d3-158">Perform a search</span></span> 
<span data-ttu-id="3b9d3-159">Die folgende Anforderung führt eine Suche nach einer Person mit dem Namen „Irene McGowan“ durch.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-159">The following request does a search for a person named Irene McGowan.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowan"
```

<span data-ttu-id="3b9d3-160">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-160">The following example shows an Autodiscover error response.</span></span> 

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
### <a name="select-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="3b9d3-161">Auswählen der Felder, die in einer gefilterten Antwort zurückgegeben werden</span><span class="sxs-lookup"><span data-stu-id="3b9d3-161">Select the fields to return in a filtered response</span></span> 
<span data-ttu-id="3b9d3-162">Sie können die *$select*- und *$filter*-Parameter gemeinsam verwenden, um eine benutzerdefinierte Liste der für den Benutzer relevanten Personen zu erstellen und nur die Felder abzurufen, die Ihre Anwendung benötigt.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-162">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span> 

<span data-ttu-id="3b9d3-p110">Im folgenden Beispiel wird **displayName** und **scoredEmailAddresses** von Personen angerufen, deren Anzeigenamen dem angegebenen Namen entspricht. In diesem Beispiel werden nur die Personen zurückgegeben, deren Anzeigename „Lorrie Frye“ lautet.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-p110">The following example gets the **displayName** and **scoredEmailAddresses** of people whose display name equals the specified name. In this example, only people whose display name equals "Lorrie Frye" are returned.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_person"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people/?$select=displayName,scoredEmailAddresses&$filter=displayName eq 'Lorrie Frye'
```

<span data-ttu-id="3b9d3-165">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="3b9d3-165">The following example shows an Autodiscover error response.</span></span> 

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
