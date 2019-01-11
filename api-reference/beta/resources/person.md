---
title: Personenressourcentyp
description: Die Aggregation von Informationen über die von einer Person über e-Mail, Kontakte und sozialen Netzwerken. Personen können lokalen Kontakten, Kontakte aus für soziale Netzwerke, Ihrer Organisation Verzeichnis und Personen von letzte Kommunikation (wie e-Mail und Skype) sein.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: c0318986b01704501a2b7910888d6a5e962a5dca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865380"
---
# <a name="person-resource-type"></a><span data-ttu-id="74634-104">Personenressourcentyp</span><span class="sxs-lookup"><span data-stu-id="74634-104">person resource type</span></span>

> <span data-ttu-id="74634-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="74634-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74634-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="74634-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="74634-107">Die Aggregation von Informationen über die von einer Person über e-Mail, Kontakte und sozialen Netzwerken.</span><span class="sxs-lookup"><span data-stu-id="74634-107">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="74634-108">Personen können lokalen Kontakten, Kontakte aus für soziale Netzwerke, Ihrer Organisation Verzeichnis und Personen von letzte Kommunikation (wie e-Mail und Skype) sein.</span><span class="sxs-lookup"><span data-stu-id="74634-108">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="74634-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="74634-109">Methods</span></span>

| <span data-ttu-id="74634-110">Methode</span><span class="sxs-lookup"><span data-stu-id="74634-110">Method</span></span> | <span data-ttu-id="74634-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="74634-111">Return Type</span></span> | <span data-ttu-id="74634-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74634-112">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="74634-113">List people</span><span class="sxs-lookup"><span data-stu-id="74634-113">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="74634-114">**Person**</span><span class="sxs-lookup"><span data-stu-id="74634-114">**person**</span></span> |<span data-ttu-id="74634-115">Dient zum Abrufen einer Sammlung von person-Objekten, sortiert nach ihrer Relevanz für den [Benutzer](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="74634-115">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="74634-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="74634-116">Properties</span></span>

| <span data-ttu-id="74634-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="74634-117">Property</span></span> | <span data-ttu-id="74634-118">Typ</span><span class="sxs-lookup"><span data-stu-id="74634-118">Type</span></span> | <span data-ttu-id="74634-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="74634-119">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="74634-120">birthday</span><span class="sxs-lookup"><span data-stu-id="74634-120">birthday</span></span>|<span data-ttu-id="74634-121">string</span><span class="sxs-lookup"><span data-stu-id="74634-121">string</span></span>|<span data-ttu-id="74634-122">Der Geburtstag der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-122">The person's birthday.</span></span>|
|<span data-ttu-id="74634-123">companyName</span><span class="sxs-lookup"><span data-stu-id="74634-123">companyName</span></span>|<span data-ttu-id="74634-124">string</span><span class="sxs-lookup"><span data-stu-id="74634-124">string</span></span>|<span data-ttu-id="74634-125">Der Name des Unternehmens der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-125">The name of the person's company.</span></span>|
|<span data-ttu-id="74634-126">department</span><span class="sxs-lookup"><span data-stu-id="74634-126">department</span></span>|<span data-ttu-id="74634-127">string</span><span class="sxs-lookup"><span data-stu-id="74634-127">string</span></span>|<span data-ttu-id="74634-128">Die Abteilung der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-128">The person's department.</span></span>|
|<span data-ttu-id="74634-129">displayName</span><span class="sxs-lookup"><span data-stu-id="74634-129">displayName</span></span>|<span data-ttu-id="74634-130">string</span><span class="sxs-lookup"><span data-stu-id="74634-130">string</span></span>|<span data-ttu-id="74634-131">Der Anzeigename der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-131">The person's display name.</span></span>|
|<span data-ttu-id="74634-132">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="74634-132">emailAddresses</span></span>|<span data-ttu-id="74634-133">[RankedEmailAddress](rankedemailaddress.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="74634-133">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="74634-134">Die E-Mail-Adressen der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-134">The person's email addresses.</span></span>|
|<span data-ttu-id="74634-135">givenName</span><span class="sxs-lookup"><span data-stu-id="74634-135">givenName</span></span>|<span data-ttu-id="74634-136">string</span><span class="sxs-lookup"><span data-stu-id="74634-136">string</span></span>|<span data-ttu-id="74634-137">Der Vorname der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-137">The person's given name.</span></span>|
|<span data-ttu-id="74634-138">id</span><span class="sxs-lookup"><span data-stu-id="74634-138">id</span></span>|<span data-ttu-id="74634-139">string</span><span class="sxs-lookup"><span data-stu-id="74634-139">string</span></span>|<span data-ttu-id="74634-p104">Eindeutiger Bezeichner für die Person. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="74634-p104">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="74634-142">isFavorite</span><span class="sxs-lookup"><span data-stu-id="74634-142">isFavorite</span></span>|<span data-ttu-id="74634-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="74634-143">boolean</span></span>|<span data-ttu-id="74634-144">`true`, wenn der Benutzer diese Person als Favorit gekennzeichnet hat.</span><span class="sxs-lookup"><span data-stu-id="74634-144">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="74634-145">mailboxType</span><span class="sxs-lookup"><span data-stu-id="74634-145">mailboxType</span></span>|<span data-ttu-id="74634-146">string</span><span class="sxs-lookup"><span data-stu-id="74634-146">string</span></span>|<span data-ttu-id="74634-147">Der Typ des Postfachs an, die durch die e-Mail-Adresse der Person dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="74634-147">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="74634-148">officeLocation</span><span class="sxs-lookup"><span data-stu-id="74634-148">officeLocation</span></span>|<span data-ttu-id="74634-149">string</span><span class="sxs-lookup"><span data-stu-id="74634-149">string</span></span>|<span data-ttu-id="74634-150">Der Bürostandort der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-150">The location of the person's office.</span></span>|
|<span data-ttu-id="74634-151">personNotes</span><span class="sxs-lookup"><span data-stu-id="74634-151">personNotes</span></span>|<span data-ttu-id="74634-152">string</span><span class="sxs-lookup"><span data-stu-id="74634-152">string</span></span>|<span data-ttu-id="74634-153">Frei formatierbare Notizen, die der Benutzer zu dieser Person hinzugefügt hat.</span><span class="sxs-lookup"><span data-stu-id="74634-153">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="74634-154">personType</span><span class="sxs-lookup"><span data-stu-id="74634-154">personType</span></span>|<span data-ttu-id="74634-155">string</span><span class="sxs-lookup"><span data-stu-id="74634-155">string</span></span>|<span data-ttu-id="74634-156">Der Typ der Person, beispielsweise Verteilerliste.</span><span class="sxs-lookup"><span data-stu-id="74634-156">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="74634-157">phones</span><span class="sxs-lookup"><span data-stu-id="74634-157">phones</span></span>|<span data-ttu-id="74634-158">[phone](phone.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="74634-158">[phone](phone.md) collection</span></span>|<span data-ttu-id="74634-159">Die Telefonnummern der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-159">The person's phone numbers.</span></span>|
|<span data-ttu-id="74634-160">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="74634-160">postalAddresses</span></span>|<span data-ttu-id="74634-161">[location](location.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="74634-161">[location](location.md) collection</span></span>|<span data-ttu-id="74634-162">Die Adressen der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-162">The person's addresses.</span></span>|
|<span data-ttu-id="74634-163">profession</span><span class="sxs-lookup"><span data-stu-id="74634-163">profession</span></span>|<span data-ttu-id="74634-164">string</span><span class="sxs-lookup"><span data-stu-id="74634-164">string</span></span>|<span data-ttu-id="74634-165">Der Beruf der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-165">The person's profession.</span></span>|
|<span data-ttu-id="74634-166">sources</span><span class="sxs-lookup"><span data-stu-id="74634-166">sources</span></span>|<span data-ttu-id="74634-167">[PersonDataSource](persondatasource.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="74634-167">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="74634-168">Die Quellen die Benutzerdaten stammen aus, beispielsweise Verzeichnis oder Outlook-Kontakte.</span><span class="sxs-lookup"><span data-stu-id="74634-168">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="74634-169">surname</span><span class="sxs-lookup"><span data-stu-id="74634-169">surname</span></span>|<span data-ttu-id="74634-170">string</span><span class="sxs-lookup"><span data-stu-id="74634-170">string</span></span>|<span data-ttu-id="74634-171">Der Nachname der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-171">The person's surname.</span></span>|
|<span data-ttu-id="74634-172">title</span><span class="sxs-lookup"><span data-stu-id="74634-172">title</span></span>|<span data-ttu-id="74634-173">string</span><span class="sxs-lookup"><span data-stu-id="74634-173">string</span></span>|<span data-ttu-id="74634-174">Titel der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-174">The person's title.</span></span>|
|<span data-ttu-id="74634-175">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74634-175">userPrincipalName</span></span>|<span data-ttu-id="74634-176">string</span><span class="sxs-lookup"><span data-stu-id="74634-176">string</span></span>|<span data-ttu-id="74634-p105">Der Benutzerprinzipalname der Person. Der UPN ist ein Anmeldename der Person im Internetformat, der auf dem Internetstandard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) basiert. Gemäß der Konvention sollte er dem E-Mail-Namen der Person zugeordnet sein. Das allgemeine Format lautet alias@domäne.</span><span class="sxs-lookup"><span data-stu-id="74634-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="74634-181">websites</span><span class="sxs-lookup"><span data-stu-id="74634-181">websites</span></span>|<span data-ttu-id="74634-182">[website](website.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="74634-182">[website](website.md) collection</span></span>|<span data-ttu-id="74634-183">Die Websites der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-183">The person's websites.</span></span>|
|<span data-ttu-id="74634-184">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="74634-184">yomiCompany</span></span>|<span data-ttu-id="74634-185">string</span><span class="sxs-lookup"><span data-stu-id="74634-185">string</span></span>|<span data-ttu-id="74634-186">Der phonetische japanische Firmenname des Unternehmens der Person.</span><span class="sxs-lookup"><span data-stu-id="74634-186">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74634-187">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="74634-187">Relationships</span></span>

<span data-ttu-id="74634-188">Keine</span><span class="sxs-lookup"><span data-stu-id="74634-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74634-189">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="74634-189">JSON representation</span></span>

<span data-ttu-id="74634-190">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="74634-190">Here is a JSON representation of the resource.</span></span>

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
  "emailAddresses": [{"@odata.type": "microsoft.graph.rankedEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "mailboxType": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "sources": [{"@odata.type": "microsoft.graph.personDataSource"}],
  "surname": "string",
  "title": "string",
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
