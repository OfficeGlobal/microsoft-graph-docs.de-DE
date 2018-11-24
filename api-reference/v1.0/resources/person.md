# <a name="person-resource-type"></a><span data-ttu-id="363ca-101">Personenressourcentyp</span><span class="sxs-lookup"><span data-stu-id="363ca-101">person resource type</span></span>

<span data-ttu-id="363ca-p101">Eine Ansammlung von Informationen über eine Person aus E-Mails, Kontakten und sozialen Netzwerken. Personen können lokale Kontakte, Kontakte aus sozialen Netzwerken, aus dem Verzeichnis Ihrer Organisation und Personen aus kürzlichen Unterhaltungen (z. B. E-Mail und Skype) sein.</span><span class="sxs-lookup"><span data-stu-id="363ca-p101">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="363ca-104">Methoden</span><span class="sxs-lookup"><span data-stu-id="363ca-104">Methods</span></span>

| <span data-ttu-id="363ca-105">Methode</span><span class="sxs-lookup"><span data-stu-id="363ca-105">Method</span></span> | <span data-ttu-id="363ca-106">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="363ca-106">Return Type</span></span> | <span data-ttu-id="363ca-107">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="363ca-107">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="363ca-108">List people</span><span class="sxs-lookup"><span data-stu-id="363ca-108">List people</span></span>](../api/user_list_people.md) | <span data-ttu-id="363ca-109">**Person**</span><span class="sxs-lookup"><span data-stu-id="363ca-109">**person**</span></span> |<span data-ttu-id="363ca-110">Dient zum Abrufen einer Sammlung von person-Objekten, sortiert nach ihrer Relevanz für den [Benutzer](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="363ca-110">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="363ca-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="363ca-111">Properties</span></span>

| <span data-ttu-id="363ca-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="363ca-112">Property</span></span> | <span data-ttu-id="363ca-113">Typ</span><span class="sxs-lookup"><span data-stu-id="363ca-113">Type</span></span> | <span data-ttu-id="363ca-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="363ca-114">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="363ca-115">birthday</span><span class="sxs-lookup"><span data-stu-id="363ca-115">birthday</span></span>|<span data-ttu-id="363ca-116">String</span><span class="sxs-lookup"><span data-stu-id="363ca-116">String</span></span>|<span data-ttu-id="363ca-117">Der Geburtstag der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-117">The person's birthday.</span></span>|
|<span data-ttu-id="363ca-118">companyName</span><span class="sxs-lookup"><span data-stu-id="363ca-118">companyName</span></span>|<span data-ttu-id="363ca-119">String</span><span class="sxs-lookup"><span data-stu-id="363ca-119">String</span></span>|<span data-ttu-id="363ca-120">Der Name des Unternehmens der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-120">The name of the person's company.</span></span>|
|<span data-ttu-id="363ca-121">department</span><span class="sxs-lookup"><span data-stu-id="363ca-121">department</span></span>|<span data-ttu-id="363ca-122">String</span><span class="sxs-lookup"><span data-stu-id="363ca-122">String</span></span>|<span data-ttu-id="363ca-123">Die Abteilung der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-123">The person's department.</span></span>|
|<span data-ttu-id="363ca-124">displayName</span><span class="sxs-lookup"><span data-stu-id="363ca-124">displayName</span></span>|<span data-ttu-id="363ca-125">String</span><span class="sxs-lookup"><span data-stu-id="363ca-125">String</span></span>|<span data-ttu-id="363ca-126">Der Anzeigename der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-126">The person's display name.</span></span>|
|<span data-ttu-id="363ca-127">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="363ca-127">scoredEmailAddresses</span></span>|<span data-ttu-id="363ca-128">[scoredEmailAddress](scoredemailaddress.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="363ca-128">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="363ca-129">Die E-Mail-Adressen der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-129">The person's email addresses.</span></span>|
|<span data-ttu-id="363ca-130">givenName</span><span class="sxs-lookup"><span data-stu-id="363ca-130">givenName</span></span>|<span data-ttu-id="363ca-131">String</span><span class="sxs-lookup"><span data-stu-id="363ca-131">String</span></span>|<span data-ttu-id="363ca-132">Der Vorname der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-132">The person's given name.</span></span>|
|<span data-ttu-id="363ca-133">id</span><span class="sxs-lookup"><span data-stu-id="363ca-133">id</span></span>|<span data-ttu-id="363ca-134">String</span><span class="sxs-lookup"><span data-stu-id="363ca-134">String</span></span>|<span data-ttu-id="363ca-p102">Eindeutiger Bezeichner für die Person. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="363ca-p102">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="363ca-137">imAddress</span><span class="sxs-lookup"><span data-stu-id="363ca-137">imAddress</span></span>|<span data-ttu-id="363ca-138">String</span><span class="sxs-lookup"><span data-stu-id="363ca-138">String</span></span>|<span data-ttu-id="363ca-p103">Die VOIP-SIP-Adresse (Voice oder IP; Session Initiation Protocol) der Chatnachricht für den Benutzer. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="363ca-p103">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="363ca-141">isFavorite</span><span class="sxs-lookup"><span data-stu-id="363ca-141">isFavorite</span></span>|<span data-ttu-id="363ca-142">Boolesch</span><span class="sxs-lookup"><span data-stu-id="363ca-142">Boolean</span></span>|<span data-ttu-id="363ca-143">`true`, wenn der Benutzer diese Person als Favorit gekennzeichnet hat.</span><span class="sxs-lookup"><span data-stu-id="363ca-143">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="363ca-144">jobTitle</span><span class="sxs-lookup"><span data-stu-id="363ca-144">jobTitle</span></span>|<span data-ttu-id="363ca-145">String</span><span class="sxs-lookup"><span data-stu-id="363ca-145">String</span></span>|<span data-ttu-id="363ca-146">Die Position der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-146">The person's job title.</span></span>|
|<span data-ttu-id="363ca-147">officeLocation</span><span class="sxs-lookup"><span data-stu-id="363ca-147">officeLocation</span></span>|<span data-ttu-id="363ca-148">String</span><span class="sxs-lookup"><span data-stu-id="363ca-148">String</span></span>|<span data-ttu-id="363ca-149">Der Bürostandort der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-149">The location of the person's office.</span></span>|
|<span data-ttu-id="363ca-150">personNotes</span><span class="sxs-lookup"><span data-stu-id="363ca-150">personNotes</span></span>|<span data-ttu-id="363ca-151">String</span><span class="sxs-lookup"><span data-stu-id="363ca-151">String</span></span>|<span data-ttu-id="363ca-152">Frei formatierbare Notizen, die der Benutzer zu dieser Person hinzugefügt hat.</span><span class="sxs-lookup"><span data-stu-id="363ca-152">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="363ca-153">personType</span><span class="sxs-lookup"><span data-stu-id="363ca-153">personType</span></span>|[<span data-ttu-id="363ca-154">personType</span><span class="sxs-lookup"><span data-stu-id="363ca-154">personType</span></span>](persontype.md) |<span data-ttu-id="363ca-155">Der Personentyp.</span><span class="sxs-lookup"><span data-stu-id="363ca-155">The type of person.</span></span>|
|<span data-ttu-id="363ca-156">phones</span><span class="sxs-lookup"><span data-stu-id="363ca-156">phones</span></span>|<span data-ttu-id="363ca-157">[phone](phone.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="363ca-157">[phone](phone.md) collection</span></span>|<span data-ttu-id="363ca-158">Die Telefonnummern der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-158">The person's phone numbers.</span></span>|
|<span data-ttu-id="363ca-159">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="363ca-159">postalAddresses</span></span>|<span data-ttu-id="363ca-160">[location](location.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="363ca-160">[location](location.md) collection</span></span>|<span data-ttu-id="363ca-161">Die Adressen der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-161">The person's addresses.</span></span>|
|<span data-ttu-id="363ca-162">profession</span><span class="sxs-lookup"><span data-stu-id="363ca-162">profession</span></span>|<span data-ttu-id="363ca-163">String</span><span class="sxs-lookup"><span data-stu-id="363ca-163">String</span></span>|<span data-ttu-id="363ca-164">Der Beruf der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-164">The person's profession.</span></span>|
|<span data-ttu-id="363ca-165">surname</span><span class="sxs-lookup"><span data-stu-id="363ca-165">surname</span></span>|<span data-ttu-id="363ca-166">String</span><span class="sxs-lookup"><span data-stu-id="363ca-166">String</span></span>|<span data-ttu-id="363ca-167">Der Nachname der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-167">The person's surname.</span></span>|
|<span data-ttu-id="363ca-168">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="363ca-168">userPrincipalName</span></span>|<span data-ttu-id="363ca-169">String</span><span class="sxs-lookup"><span data-stu-id="363ca-169">String</span></span>|<span data-ttu-id="363ca-p104">Der Benutzerprinzipalname der Person. Der UPN ist ein Anmeldename der Person im Internetformat, der auf dem Internetstandard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) basiert. Gemäß der Konvention sollte er dem E-Mail-Namen der Person zugeordnet sein. Das allgemeine Format lautet alias@domäne.</span><span class="sxs-lookup"><span data-stu-id="363ca-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="363ca-174">websites</span><span class="sxs-lookup"><span data-stu-id="363ca-174">websites</span></span>|<span data-ttu-id="363ca-175">[website](website.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="363ca-175">[website](website.md) collection</span></span>|<span data-ttu-id="363ca-176">Die Websites der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-176">The person's websites.</span></span>|
|<span data-ttu-id="363ca-177">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="363ca-177">yomiCompany</span></span>|<span data-ttu-id="363ca-178">String</span><span class="sxs-lookup"><span data-stu-id="363ca-178">String</span></span>|<span data-ttu-id="363ca-179">Der phonetische japanische Firmenname des Unternehmens der Person.</span><span class="sxs-lookup"><span data-stu-id="363ca-179">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="363ca-180">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="363ca-180">Relationships</span></span>

<span data-ttu-id="363ca-181">Keine.</span><span class="sxs-lookup"><span data-stu-id="363ca-181">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="363ca-182">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="363ca-182">JSON representation</span></span>

<span data-ttu-id="363ca-183">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="363ca-183">The following is a JSON representation of the resource.</span></span>

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
