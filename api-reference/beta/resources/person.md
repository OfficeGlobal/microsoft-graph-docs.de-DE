---
title: Personenressourcentyp
description: Die Aggregation von Informationen über die von einer Person über e-Mail, Kontakte und sozialen Netzwerken. Personen können lokalen Kontakten, Kontakte aus für soziale Netzwerke, Ihrer Organisation Verzeichnis und Personen von letzte Kommunikation (wie e-Mail und Skype) sein.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 32a2c9905ab52e9b229bb8673fb4a84d90a706ac
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512402"
---
# <a name="person-resource-type"></a><span data-ttu-id="00926-104">Personenressourcentyp</span><span class="sxs-lookup"><span data-stu-id="00926-104">person resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00926-105">Die Aggregation von Informationen über die von einer Person über e-Mail, Kontakte und sozialen Netzwerken.</span><span class="sxs-lookup"><span data-stu-id="00926-105">An aggregation of information about a person from across mail, contacts and social networks.</span></span> <span data-ttu-id="00926-106">Personen können lokalen Kontakten, Kontakte aus für soziale Netzwerke, Ihrer Organisation Verzeichnis und Personen von letzte Kommunikation (wie e-Mail und Skype) sein.</span><span class="sxs-lookup"><span data-stu-id="00926-106">People can be local contacts, contacts from social networking, your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="00926-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="00926-107">Methods</span></span>

| <span data-ttu-id="00926-108">Methode</span><span class="sxs-lookup"><span data-stu-id="00926-108">Method</span></span> | <span data-ttu-id="00926-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="00926-109">Return Type</span></span> | <span data-ttu-id="00926-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00926-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="00926-111">List people</span><span class="sxs-lookup"><span data-stu-id="00926-111">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="00926-112">**Person**</span><span class="sxs-lookup"><span data-stu-id="00926-112">**person**</span></span> |<span data-ttu-id="00926-113">Dient zum Abrufen einer Sammlung von person-Objekten, sortiert nach ihrer Relevanz für den [Benutzer](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="00926-113">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="00926-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="00926-114">Properties</span></span>

| <span data-ttu-id="00926-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="00926-115">Property</span></span> | <span data-ttu-id="00926-116">Typ</span><span class="sxs-lookup"><span data-stu-id="00926-116">Type</span></span> | <span data-ttu-id="00926-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="00926-117">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="00926-118">birthday</span><span class="sxs-lookup"><span data-stu-id="00926-118">birthday</span></span>|<span data-ttu-id="00926-119">string</span><span class="sxs-lookup"><span data-stu-id="00926-119">string</span></span>|<span data-ttu-id="00926-120">Der Geburtstag der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-120">The person's birthday.</span></span>|
|<span data-ttu-id="00926-121">companyName</span><span class="sxs-lookup"><span data-stu-id="00926-121">companyName</span></span>|<span data-ttu-id="00926-122">string</span><span class="sxs-lookup"><span data-stu-id="00926-122">string</span></span>|<span data-ttu-id="00926-123">Der Name des Unternehmens der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-123">The name of the person's company.</span></span>|
|<span data-ttu-id="00926-124">department</span><span class="sxs-lookup"><span data-stu-id="00926-124">department</span></span>|<span data-ttu-id="00926-125">string</span><span class="sxs-lookup"><span data-stu-id="00926-125">string</span></span>|<span data-ttu-id="00926-126">Die Abteilung der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-126">The person's department.</span></span>|
|<span data-ttu-id="00926-127">displayName</span><span class="sxs-lookup"><span data-stu-id="00926-127">displayName</span></span>|<span data-ttu-id="00926-128">String</span><span class="sxs-lookup"><span data-stu-id="00926-128">string</span></span>|<span data-ttu-id="00926-129">Der Anzeigename der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-129">The person's display name.</span></span>|
|<span data-ttu-id="00926-130">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="00926-130">emailAddresses</span></span>|<span data-ttu-id="00926-131">[RankedEmailAddress](rankedemailaddress.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="00926-131">[rankedEmailAddress](rankedemailaddress.md) collection</span></span>|<span data-ttu-id="00926-132">Die E-Mail-Adressen der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-132">The person's email addresses.</span></span>|
|<span data-ttu-id="00926-133">givenName</span><span class="sxs-lookup"><span data-stu-id="00926-133">givenName</span></span>|<span data-ttu-id="00926-134">string</span><span class="sxs-lookup"><span data-stu-id="00926-134">string</span></span>|<span data-ttu-id="00926-135">Der Vorname der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-135">The person's given name.</span></span>|
|<span data-ttu-id="00926-136">id</span><span class="sxs-lookup"><span data-stu-id="00926-136">id</span></span>|<span data-ttu-id="00926-137">string</span><span class="sxs-lookup"><span data-stu-id="00926-137">string</span></span>|<span data-ttu-id="00926-p103">Eindeutiger Bezeichner für die Person. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="00926-p103">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="00926-140">isFavorite</span><span class="sxs-lookup"><span data-stu-id="00926-140">isFavorite</span></span>|<span data-ttu-id="00926-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="00926-141">boolean</span></span>|<span data-ttu-id="00926-142">`true`, wenn der Benutzer diese Person als Favorit gekennzeichnet hat.</span><span class="sxs-lookup"><span data-stu-id="00926-142">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="00926-143">MailboxType</span><span class="sxs-lookup"><span data-stu-id="00926-143">mailboxType</span></span>|<span data-ttu-id="00926-144">string</span><span class="sxs-lookup"><span data-stu-id="00926-144">string</span></span>|<span data-ttu-id="00926-145">Der Typ des Postfachs an, die durch die e-Mail-Adresse der Person dargestellt wird.</span><span class="sxs-lookup"><span data-stu-id="00926-145">The type of mailbox that is represented by the person's email address.</span></span>|
|<span data-ttu-id="00926-146">officeLocation</span><span class="sxs-lookup"><span data-stu-id="00926-146">officeLocation</span></span>|<span data-ttu-id="00926-147">string</span><span class="sxs-lookup"><span data-stu-id="00926-147">string</span></span>|<span data-ttu-id="00926-148">Der Bürostandort der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-148">The location of the person's office.</span></span>|
|<span data-ttu-id="00926-149">personNotes</span><span class="sxs-lookup"><span data-stu-id="00926-149">personNotes</span></span>|<span data-ttu-id="00926-150">string</span><span class="sxs-lookup"><span data-stu-id="00926-150">string</span></span>|<span data-ttu-id="00926-151">Frei formatierbare Notizen, die der Benutzer zu dieser Person hinzugefügt hat.</span><span class="sxs-lookup"><span data-stu-id="00926-151">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="00926-152">personType</span><span class="sxs-lookup"><span data-stu-id="00926-152">personType</span></span>|<span data-ttu-id="00926-153">string</span><span class="sxs-lookup"><span data-stu-id="00926-153">string</span></span>|<span data-ttu-id="00926-154">Der Typ der Person, beispielsweise Verteilerliste.</span><span class="sxs-lookup"><span data-stu-id="00926-154">The type of person, for example distribution list.</span></span>|
|<span data-ttu-id="00926-155">phones</span><span class="sxs-lookup"><span data-stu-id="00926-155">phones</span></span>|<span data-ttu-id="00926-156">[phone](phone.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="00926-156">[phone](phone.md) collection</span></span>|<span data-ttu-id="00926-157">Die Telefonnummern der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-157">The person's phone numbers.</span></span>|
|<span data-ttu-id="00926-158">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="00926-158">postalAddresses</span></span>|<span data-ttu-id="00926-159">[location](location.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="00926-159">[location](location.md) collection</span></span>|<span data-ttu-id="00926-160">Die Adressen der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-160">The person's addresses.</span></span>|
|<span data-ttu-id="00926-161">profession</span><span class="sxs-lookup"><span data-stu-id="00926-161">profession</span></span>|<span data-ttu-id="00926-162">string</span><span class="sxs-lookup"><span data-stu-id="00926-162">string</span></span>|<span data-ttu-id="00926-163">Der Beruf der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-163">The person's profession.</span></span>|
|<span data-ttu-id="00926-164">sources</span><span class="sxs-lookup"><span data-stu-id="00926-164">sources</span></span>|<span data-ttu-id="00926-165">[PersonDataSource](persondatasource.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="00926-165">[personDataSource](persondatasource.md) collection</span></span>|<span data-ttu-id="00926-166">Die Quellen die Benutzerdaten stammen aus, beispielsweise Verzeichnis oder Outlook-Kontakte.</span><span class="sxs-lookup"><span data-stu-id="00926-166">The sources the user data comes from, for example Directory or Outlook Contacts.</span></span>|
|<span data-ttu-id="00926-167">surname</span><span class="sxs-lookup"><span data-stu-id="00926-167">surname</span></span>|<span data-ttu-id="00926-168">string</span><span class="sxs-lookup"><span data-stu-id="00926-168">string</span></span>|<span data-ttu-id="00926-169">Der Nachname der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-169">The person's surname.</span></span>|
|<span data-ttu-id="00926-170">title</span><span class="sxs-lookup"><span data-stu-id="00926-170">title</span></span>|<span data-ttu-id="00926-171">string</span><span class="sxs-lookup"><span data-stu-id="00926-171">string</span></span>|<span data-ttu-id="00926-172">Titel der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-172">The person's title.</span></span>|
|<span data-ttu-id="00926-173">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="00926-173">userPrincipalName</span></span>|<span data-ttu-id="00926-174">string</span><span class="sxs-lookup"><span data-stu-id="00926-174">string</span></span>|<span data-ttu-id="00926-p104">Der Benutzerprinzipalname der Person. Der UPN ist ein Anmeldename der Person im Internetformat, der auf dem Internetstandard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) basiert. Gemäß der Konvention sollte er dem E-Mail-Namen der Person zugeordnet sein. Das allgemeine Format lautet alias@domäne.</span><span class="sxs-lookup"><span data-stu-id="00926-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="00926-179">websites</span><span class="sxs-lookup"><span data-stu-id="00926-179">websites</span></span>|<span data-ttu-id="00926-180">[website](website.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="00926-180">[website](website.md) collection</span></span>|<span data-ttu-id="00926-181">Die Websites der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-181">The person's websites.</span></span>|
|<span data-ttu-id="00926-182">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="00926-182">yomiCompany</span></span>|<span data-ttu-id="00926-183">string</span><span class="sxs-lookup"><span data-stu-id="00926-183">string</span></span>|<span data-ttu-id="00926-184">Der phonetische japanische Firmenname des Unternehmens der Person.</span><span class="sxs-lookup"><span data-stu-id="00926-184">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00926-185">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="00926-185">Relationships</span></span>

<span data-ttu-id="00926-186">Keine</span><span class="sxs-lookup"><span data-stu-id="00926-186">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00926-187">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="00926-187">JSON representation</span></span>

<span data-ttu-id="00926-188">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="00926-188">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/person.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
