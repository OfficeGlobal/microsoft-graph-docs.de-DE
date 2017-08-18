# <a name="person-resource-type"></a><span data-ttu-id="31fb5-101">Personenressourcentyp</span><span class="sxs-lookup"><span data-stu-id="31fb5-101">person resource type</span></span>

<span data-ttu-id="31fb5-p101">Eine Ansammlung von Informationen über eine Person aus E-Mails, Kontakten und sozialen Netzwerken. Personen können lokale Kontakte, Kontakte aus sozialen Netzwerken, aus dem Verzeichnis Ihrer Organisation und Personen aus kürzlichen Unterhaltungen (z. B. E-Mail und Skype) sein.</span><span class="sxs-lookup"><span data-stu-id="31fb5-p101">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="31fb5-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="31fb5-104">Methods</span></span>

| <span data-ttu-id="31fb5-105">Methode</span><span class="sxs-lookup"><span data-stu-id="31fb5-105">Method</span></span>           | <span data-ttu-id="31fb5-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="31fb5-106">Return Type</span></span>    |<span data-ttu-id="31fb5-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31fb5-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="31fb5-108">List people</span><span class="sxs-lookup"><span data-stu-id="31fb5-108">List people</span></span>](../api/user_list_people.md) | <span data-ttu-id="31fb5-109">**Person**</span><span class="sxs-lookup"><span data-stu-id="31fb5-109">**Person**</span></span> |<span data-ttu-id="31fb5-110">Dient zum Abrufen einer Sammlung von person-Objekten, sortiert nach ihrer Relevanz für den [Benutzer](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="31fb5-110">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|
|[<span data-ttu-id="31fb5-111">Get person</span><span class="sxs-lookup"><span data-stu-id="31fb5-111">Get person</span></span>](../api/person_get.md) | <span data-ttu-id="31fb5-112">**Person**</span><span class="sxs-lookup"><span data-stu-id="31fb5-112">**Person**</span></span> |<span data-ttu-id="31fb5-113">Dient zum Abrufen der Eigenschaften und der Beziehungen eines person-Objekts.</span><span class="sxs-lookup"><span data-stu-id="31fb5-113">Get the properties and relationships of a device object.</span></span>|


## <a name="properties"></a><span data-ttu-id="31fb5-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="31fb5-114">Properties</span></span>
| <span data-ttu-id="31fb5-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="31fb5-115">Property</span></span>     | <span data-ttu-id="31fb5-116">Typ</span><span class="sxs-lookup"><span data-stu-id="31fb5-116">Type</span></span>   |<span data-ttu-id="31fb5-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31fb5-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31fb5-118">birthday</span><span class="sxs-lookup"><span data-stu-id="31fb5-118">birthday</span></span>|<span data-ttu-id="31fb5-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-119">String</span></span>|<span data-ttu-id="31fb5-120">Der Geburtstag der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-120">The person's birthday.</span></span>|
|<span data-ttu-id="31fb5-121">companyName</span><span class="sxs-lookup"><span data-stu-id="31fb5-121">companyName</span></span>|<span data-ttu-id="31fb5-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-122">String</span></span>|<span data-ttu-id="31fb5-123">Der Name des Unternehmens der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-123">The name of the contact's company.</span></span>|
|<span data-ttu-id="31fb5-124">department</span><span class="sxs-lookup"><span data-stu-id="31fb5-124">department</span></span>|<span data-ttu-id="31fb5-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-125">String</span></span>|<span data-ttu-id="31fb5-126">Die Abteilung der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-126">The person's department.</span></span>|
|<span data-ttu-id="31fb5-127">displayName</span><span class="sxs-lookup"><span data-stu-id="31fb5-127">displayName</span></span>|<span data-ttu-id="31fb5-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-128">String</span></span>|<span data-ttu-id="31fb5-129">Der Anzeigename der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-129">The person's display name.</span></span>|
|<span data-ttu-id="31fb5-130">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="31fb5-130">scoredEmailAddresses</span></span>|<span data-ttu-id="31fb5-131">[scoredEmailAddress](scoredemailaddress.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="31fb5-131">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="31fb5-132">Die E-Mail-Adressen der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-132">The contact's email addresses.</span></span>|
|<span data-ttu-id="31fb5-133">givenName</span><span class="sxs-lookup"><span data-stu-id="31fb5-133">givenName</span></span>|<span data-ttu-id="31fb5-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-134">String</span></span>|<span data-ttu-id="31fb5-135">Der Vorname der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-135">The contact's given name.</span></span>|
|<span data-ttu-id="31fb5-136">id</span><span class="sxs-lookup"><span data-stu-id="31fb5-136">id</span></span>|<span data-ttu-id="31fb5-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-137">String</span></span>|<span data-ttu-id="31fb5-p102">Eindeutiger Bezeichner für die Person. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="31fb5-p102">The group's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="31fb5-140">imAddress</span><span class="sxs-lookup"><span data-stu-id="31fb5-140">IMAddress</span></span>|<span data-ttu-id="31fb5-141">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="31fb5-141">String collection</span></span>|<span data-ttu-id="31fb5-p103">Die VOIP-SIP-Adresse (Voice oder IP; Session Initiation Protocol) der Chatnachricht für den Benutzer. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="31fb5-p103">The instant message voice over IP (VOIP) session initiation protocol (SIP) addresses for the user. Read-only.</span></span>|
|<span data-ttu-id="31fb5-144">isFavorite</span><span class="sxs-lookup"><span data-stu-id="31fb5-144">isFavorite</span></span>|<span data-ttu-id="31fb5-145">Boolesch</span><span class="sxs-lookup"><span data-stu-id="31fb5-145">Boolean</span></span>|<span data-ttu-id="31fb5-146">`true`, wenn der Benutzer diese Person als Favorit gekennzeichnet hat.</span><span class="sxs-lookup"><span data-stu-id="31fb5-146">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="31fb5-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="31fb5-147">jobTitle</span></span>|<span data-ttu-id="31fb5-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-148">String</span></span>|<span data-ttu-id="31fb5-149">Die Position der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-149">The contact’s job title.</span></span>|
|<span data-ttu-id="31fb5-150">officeLocation</span><span class="sxs-lookup"><span data-stu-id="31fb5-150">officeLocation</span></span>|<span data-ttu-id="31fb5-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-151">String</span></span>|<span data-ttu-id="31fb5-152">Der Bürostandort der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-152">The location of the contact's office.</span></span>|
|<span data-ttu-id="31fb5-153">personNotes</span><span class="sxs-lookup"><span data-stu-id="31fb5-153">personNotes</span></span>|<span data-ttu-id="31fb5-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-154">String</span></span>|<span data-ttu-id="31fb5-155">Frei formatierbare Notizen, die der Benutzer zu dieser Person hinzugefügt hat.</span><span class="sxs-lookup"><span data-stu-id="31fb5-155">Free-form notes that the the user has taken about this person.</span></span>|
|<span data-ttu-id="31fb5-156">personType</span><span class="sxs-lookup"><span data-stu-id="31fb5-156">personType</span></span>|<span data-ttu-id="31fb5-157">[personType](persontype.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="31fb5-157">[personType](persontype.md) collection</span></span>|<span data-ttu-id="31fb5-158">Der Personentyp.</span><span class="sxs-lookup"><span data-stu-id="31fb5-158">The type of person.</span></span>|
|<span data-ttu-id="31fb5-159">phones</span><span class="sxs-lookup"><span data-stu-id="31fb5-159">phones</span></span>|<span data-ttu-id="31fb5-160">[phone](phone.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="31fb5-160">[phone](phone.md) collection</span></span>|<span data-ttu-id="31fb5-161">Die Telefonnummern der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-161">The user's phone numbers.</span></span>|
|<span data-ttu-id="31fb5-162">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="31fb5-162">postalAddresses</span></span>|<span data-ttu-id="31fb5-163">[location](location.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="31fb5-163">[location](location.md) collection</span></span>|<span data-ttu-id="31fb5-164">Die Adressen der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-164">The person's addresses.</span></span>|
|<span data-ttu-id="31fb5-165">profession</span><span class="sxs-lookup"><span data-stu-id="31fb5-165">profession</span></span>|<span data-ttu-id="31fb5-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-166">String</span></span>|<span data-ttu-id="31fb5-167">Der Beruf der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-167">The person's profession.</span></span>|
|<span data-ttu-id="31fb5-168">surname</span><span class="sxs-lookup"><span data-stu-id="31fb5-168">surname</span></span>|<span data-ttu-id="31fb5-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-169">String</span></span>|<span data-ttu-id="31fb5-170">Der Nachname der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-170">The person's surname.</span></span>|
|<span data-ttu-id="31fb5-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="31fb5-171">userPrincipalName</span></span>|<span data-ttu-id="31fb5-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-172">String</span></span>|<span data-ttu-id="31fb5-p104">Der Benutzerprinzipalname der Person. Der UPN ist ein Anmeldename der Person im Internetformat, der auf dem Internetstandard [RFC 822](http://www.ietf.org/rfc/rfc0822.txt) basiert. Gemäß der Konvention sollte er dem E-Mail-Namen der Person zugeordnet sein. Das allgemeine Format lautet alias@domäne.</span><span class="sxs-lookup"><span data-stu-id="31fb5-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](http://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="31fb5-177">websites</span><span class="sxs-lookup"><span data-stu-id="31fb5-177">Websites</span></span>|<span data-ttu-id="31fb5-178">[website](website.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="31fb5-178">[website](website.md) collection</span></span>|<span data-ttu-id="31fb5-179">Die Websites der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-179">The person's websites.</span></span>|
|<span data-ttu-id="31fb5-180">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="31fb5-180">yomiCompany</span></span>|<span data-ttu-id="31fb5-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="31fb5-181">String</span></span>|<span data-ttu-id="31fb5-182">Der phonetische japanische Firmenname des Unternehmens der Person.</span><span class="sxs-lookup"><span data-stu-id="31fb5-182">The phonetic Japanese company name of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31fb5-183">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="31fb5-183">Relationships</span></span>
<span data-ttu-id="31fb5-184">Keine.</span><span class="sxs-lookup"><span data-stu-id="31fb5-184">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="31fb5-185">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="31fb5-185">JSON representation</span></span>

<span data-ttu-id="31fb5-186">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="31fb5-186">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredemailaddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": [{"@odata.type": "microsoft.graph.persontype"}],
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "surname": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
