# <a name="person-resource-type"></a><span data-ttu-id="d026e-101">Personenressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d026e-101">person resource type</span></span>

<span data-ttu-id="d026e-p101">Eine Ansammlung von Informationen über eine Person aus E-Mails, Kontakten und sozialen Netzwerken. Personen können lokale Kontakte, Kontakte aus sozialen Netzwerken, aus dem Verzeichnis Ihrer Organisation und Personen aus kürzlichen Unterhaltungen (z. B. E-Mail und Skype) sein.</span><span class="sxs-lookup"><span data-stu-id="d026e-p101">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="d026e-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="d026e-104">Methods</span></span>

| <span data-ttu-id="d026e-105">Methode</span><span class="sxs-lookup"><span data-stu-id="d026e-105">Method</span></span> | <span data-ttu-id="d026e-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d026e-106">Return Type</span></span> | <span data-ttu-id="d026e-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d026e-107">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="d026e-108">Personen auflisten</span><span class="sxs-lookup"><span data-stu-id="d026e-108">List people</span></span>](../api/user_list_people.md) | <span data-ttu-id="d026e-109">**Person**</span><span class="sxs-lookup"><span data-stu-id="d026e-109">**person**</span></span> |<span data-ttu-id="d026e-110">Dient zum Abrufen einer Sammlung von person-Objekten, sortiert nach ihrer Relevanz für den [Benutzer](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="d026e-110">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="d026e-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d026e-111">Properties</span></span>

| <span data-ttu-id="d026e-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d026e-112">Property</span></span> | <span data-ttu-id="d026e-113">Typ</span><span class="sxs-lookup"><span data-stu-id="d026e-113">Type</span></span> | <span data-ttu-id="d026e-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d026e-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d026e-115">Geburtsdatum</span><span class="sxs-lookup"><span data-stu-id="d026e-115">birthday</span></span>|<span data-ttu-id="d026e-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-116">String</span></span>|<span data-ttu-id="d026e-117">Der Geburtstag der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-117">The person's birthday.</span></span>|
|<span data-ttu-id="d026e-118">companyName</span><span class="sxs-lookup"><span data-stu-id="d026e-118">companyName</span></span>|<span data-ttu-id="d026e-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-119">String</span></span>|<span data-ttu-id="d026e-120">Der Name des Unternehmens der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-120">The name of the person's company.</span></span>|
|<span data-ttu-id="d026e-121">Abteilung</span><span class="sxs-lookup"><span data-stu-id="d026e-121">department</span></span>|<span data-ttu-id="d026e-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-122">String</span></span>|<span data-ttu-id="d026e-123">Die Abteilung der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-123">The person's department.</span></span>|
|<span data-ttu-id="d026e-124">displayName</span><span class="sxs-lookup"><span data-stu-id="d026e-124">displayName</span></span>|<span data-ttu-id="d026e-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-125">String</span></span>|<span data-ttu-id="d026e-126">Der Anzeigename der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-126">The person's display name.</span></span>|
|<span data-ttu-id="d026e-127">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="d026e-127">scoredEmailAddresses</span></span>|<span data-ttu-id="d026e-128">[scoredEmailAddress](scoredemailaddress.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d026e-128">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="d026e-129">Die E-Mail-Adressen der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-129">The person's email addresses.</span></span>|
|<span data-ttu-id="d026e-130">givenName</span><span class="sxs-lookup"><span data-stu-id="d026e-130">givenName</span></span>|<span data-ttu-id="d026e-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-131">String</span></span>|<span data-ttu-id="d026e-132">Der Vorname der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-132">The person's given name.</span></span>|
|<span data-ttu-id="d026e-133">id</span><span class="sxs-lookup"><span data-stu-id="d026e-133">id</span></span>|<span data-ttu-id="d026e-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-134">String</span></span>|<span data-ttu-id="d026e-p102">Eindeutiger Bezeichner für die Person. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d026e-p102">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="d026e-137">imAddress</span><span class="sxs-lookup"><span data-stu-id="d026e-137">imAddress</span></span>|<span data-ttu-id="d026e-138">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-138">String</span></span>|<span data-ttu-id="d026e-p103">Die VOIP-SIP-Adresse (Voice oder IP; Session Initiation Protocol) der Chatnachricht für den Benutzer. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="d026e-p103">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="d026e-141">isFavorite</span><span class="sxs-lookup"><span data-stu-id="d026e-141">isFavorite</span></span>|<span data-ttu-id="d026e-142">Boolesch</span><span class="sxs-lookup"><span data-stu-id="d026e-142">Boolean</span></span>|<span data-ttu-id="d026e-143">`true` , wenn der Benutzer diese Person als Favorit gekennzeichnet hat.</span><span class="sxs-lookup"><span data-stu-id="d026e-143">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="d026e-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="d026e-144">jobTitle</span></span>|<span data-ttu-id="d026e-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-145">String</span></span>|<span data-ttu-id="d026e-146">Die Position der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-146">The person's job title.</span></span>|
|<span data-ttu-id="d026e-147">officeLocation</span><span class="sxs-lookup"><span data-stu-id="d026e-147">officeLocation</span></span>|<span data-ttu-id="d026e-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-148">String</span></span>|<span data-ttu-id="d026e-149">Der Bürostandort der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-149">The location of the person's office.</span></span>|
|<span data-ttu-id="d026e-150">personNotes</span><span class="sxs-lookup"><span data-stu-id="d026e-150">personNotes</span></span>|<span data-ttu-id="d026e-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-151">String</span></span>|<span data-ttu-id="d026e-152">Frei formatierbare Notizen, die der Benutzer zu dieser Person hinzugefügt hat.</span><span class="sxs-lookup"><span data-stu-id="d026e-152">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="d026e-153">personType</span><span class="sxs-lookup"><span data-stu-id="d026e-153">personType</span></span>|[<span data-ttu-id="d026e-154">personType</span><span class="sxs-lookup"><span data-stu-id="d026e-154">personType</span></span>](persontype.md) |<span data-ttu-id="d026e-155">Der Personentyp.</span><span class="sxs-lookup"><span data-stu-id="d026e-155">The type of person.</span></span>|
|<span data-ttu-id="d026e-156">phones</span><span class="sxs-lookup"><span data-stu-id="d026e-156">phones</span></span>|<span data-ttu-id="d026e-157">[phone](phone.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d026e-157">[phone](phone.md) collection</span></span>|<span data-ttu-id="d026e-158">Die Telefonnummern der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-158">The person's phone numbers.</span></span>|
|<span data-ttu-id="d026e-159">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="d026e-159">postalAddresses</span></span>|<span data-ttu-id="d026e-160">[location](location.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d026e-160">[location](location.md) collection</span></span>|<span data-ttu-id="d026e-161">Die Adressen der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-161">The person's addresses.</span></span>|
|<span data-ttu-id="d026e-162">profession</span><span class="sxs-lookup"><span data-stu-id="d026e-162">profession</span></span>|<span data-ttu-id="d026e-163">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-163">String</span></span>|<span data-ttu-id="d026e-164">Der Beruf der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-164">The person's profession.</span></span>|
|<span data-ttu-id="d026e-165">surname</span><span class="sxs-lookup"><span data-stu-id="d026e-165">surname</span></span>|<span data-ttu-id="d026e-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-166">String</span></span>|<span data-ttu-id="d026e-167">Der Nachname der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-167">The person's surname.</span></span>|
|<span data-ttu-id="d026e-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d026e-168">userPrincipalName</span></span>|<span data-ttu-id="d026e-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-169">String</span></span>|<span data-ttu-id="d026e-p104">Der Benutzerprinzipalname der Person. Der UPN ist ein Anmeldename der Person im Internetformat, der auf dem Internetstandard [RFC 822](http://www.ietf.org/rfc/rfc0822.txt) basiert. Gemäß der Konvention sollte er dem E-Mail-Namen der Person zugeordnet sein. Das allgemeine Format lautet alias@domäne.</span><span class="sxs-lookup"><span data-stu-id="d026e-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](http://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="d026e-174">websites</span><span class="sxs-lookup"><span data-stu-id="d026e-174">websites</span></span>|<span data-ttu-id="d026e-175">[website](website.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d026e-175">[website](website.md) collection</span></span>|<span data-ttu-id="d026e-176">Die Websites der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-176">The person's websites.</span></span>|
|<span data-ttu-id="d026e-177">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="d026e-177">yomiCompany</span></span>|<span data-ttu-id="d026e-178">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d026e-178">String</span></span>|<span data-ttu-id="d026e-179">Der phonetische japanische Firmenname des Unternehmens der Person.</span><span class="sxs-lookup"><span data-stu-id="d026e-179">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d026e-180">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d026e-180">Relationships</span></span>

<span data-ttu-id="d026e-181">Keine.</span><span class="sxs-lookup"><span data-stu-id="d026e-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d026e-182">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d026e-182">JSON representation</span></span>

<span data-ttu-id="d026e-183">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d026e-183">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "imAddress": "string",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": {"@odata.type": "microsoft.graph.personType"},
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
