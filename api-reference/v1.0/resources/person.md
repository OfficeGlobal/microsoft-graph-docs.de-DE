---
title: Personenressourcentyp
description: Eine Ansammlung von Informationen über eine Person aus E-Mails, Kontakten und sozialen Netzwerken. Personen können lokale Kontakte, Kontakte aus sozialen Netzwerken, aus dem Verzeichnis Ihrer Organisation und Personen aus kürzlichen Unterhaltungen (z. B. E-Mail und Skype) sein.
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: c92709143ee7def0ede98dfdb81a419df43c4493
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940295"
---
# <a name="person-resource-type"></a><span data-ttu-id="a3336-104">Personenressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a3336-104">person resource type</span></span>

<span data-ttu-id="a3336-p102">Eine Ansammlung von Informationen über eine Person aus E-Mails, Kontakten und sozialen Netzwerken. Personen können lokale Kontakte, Kontakte aus sozialen Netzwerken, aus dem Verzeichnis Ihrer Organisation und Personen aus kürzlichen Unterhaltungen (z. B. E-Mail und Skype) sein.</span><span class="sxs-lookup"><span data-stu-id="a3336-p102">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="a3336-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="a3336-107">Methods</span></span>

| <span data-ttu-id="a3336-108">Methode</span><span class="sxs-lookup"><span data-stu-id="a3336-108">Method</span></span> | <span data-ttu-id="a3336-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="a3336-109">Return Type</span></span> | <span data-ttu-id="a3336-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3336-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="a3336-111">List people</span><span class="sxs-lookup"><span data-stu-id="a3336-111">List people</span></span>](../api/user-list-people.md) | <span data-ttu-id="a3336-112">**Person**</span><span class="sxs-lookup"><span data-stu-id="a3336-112">**person**</span></span> |<span data-ttu-id="a3336-113">Dient zum Abrufen einer Sammlung von person-Objekten, sortiert nach ihrer Relevanz für den [Benutzer](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="a3336-113">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|

## <a name="properties"></a><span data-ttu-id="a3336-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a3336-114">Properties</span></span>

| <span data-ttu-id="a3336-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a3336-115">Property</span></span> | <span data-ttu-id="a3336-116">Typ</span><span class="sxs-lookup"><span data-stu-id="a3336-116">Type</span></span> | <span data-ttu-id="a3336-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a3336-117">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a3336-118">birthday</span><span class="sxs-lookup"><span data-stu-id="a3336-118">birthday</span></span>|<span data-ttu-id="a3336-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-119">String</span></span>|<span data-ttu-id="a3336-120">Der Geburtstag der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-120">The person's birthday.</span></span>|
|<span data-ttu-id="a3336-121">companyName</span><span class="sxs-lookup"><span data-stu-id="a3336-121">companyName</span></span>|<span data-ttu-id="a3336-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-122">String</span></span>|<span data-ttu-id="a3336-123">Der Name des Unternehmens der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-123">The name of the person's company.</span></span>|
|<span data-ttu-id="a3336-124">department</span><span class="sxs-lookup"><span data-stu-id="a3336-124">department</span></span>|<span data-ttu-id="a3336-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-125">String</span></span>|<span data-ttu-id="a3336-126">Die Abteilung der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-126">The person's department.</span></span>|
|<span data-ttu-id="a3336-127">displayName</span><span class="sxs-lookup"><span data-stu-id="a3336-127">displayName</span></span>|<span data-ttu-id="a3336-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-128">String</span></span>|<span data-ttu-id="a3336-129">Der Anzeigename der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-129">The person's display name.</span></span>|
|<span data-ttu-id="a3336-130">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="a3336-130">scoredEmailAddresses</span></span>|<span data-ttu-id="a3336-131">[scoredEmailAddress](scoredemailaddress.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a3336-131">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="a3336-132">Die E-Mail-Adressen der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-132">The person's email addresses.</span></span>|
|<span data-ttu-id="a3336-133">givenName</span><span class="sxs-lookup"><span data-stu-id="a3336-133">givenName</span></span>|<span data-ttu-id="a3336-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-134">String</span></span>|<span data-ttu-id="a3336-135">Der Vorname der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-135">The person's given name.</span></span>|
|<span data-ttu-id="a3336-136">id</span><span class="sxs-lookup"><span data-stu-id="a3336-136">id</span></span>|<span data-ttu-id="a3336-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-137">String</span></span>|<span data-ttu-id="a3336-p103">Eindeutiger Bezeichner für die Person. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a3336-p103">The person's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="a3336-140">imAddress</span><span class="sxs-lookup"><span data-stu-id="a3336-140">imAddress</span></span>|<span data-ttu-id="a3336-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-141">String</span></span>|<span data-ttu-id="a3336-p104">Die VOIP-SIP-Adresse (Voice oder IP; Session Initiation Protocol) der Chatnachricht für den Benutzer. Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="a3336-p104">The instant message voice over IP (VOIP) session initiation protocol (SIP) address for the user. Read-only.</span></span>|
|<span data-ttu-id="a3336-144">isFavorite</span><span class="sxs-lookup"><span data-stu-id="a3336-144">isFavorite</span></span>|<span data-ttu-id="a3336-145">Boolesch</span><span class="sxs-lookup"><span data-stu-id="a3336-145">Boolean</span></span>|<span data-ttu-id="a3336-146">`true`, wenn der Benutzer diese Person als Favorit gekennzeichnet hat.</span><span class="sxs-lookup"><span data-stu-id="a3336-146">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="a3336-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="a3336-147">jobTitle</span></span>|<span data-ttu-id="a3336-148">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-148">String</span></span>|<span data-ttu-id="a3336-149">Die Position der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-149">The person's job title.</span></span>|
|<span data-ttu-id="a3336-150">officeLocation</span><span class="sxs-lookup"><span data-stu-id="a3336-150">officeLocation</span></span>|<span data-ttu-id="a3336-151">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-151">String</span></span>|<span data-ttu-id="a3336-152">Der Bürostandort der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-152">The location of the person's office.</span></span>|
|<span data-ttu-id="a3336-153">personNotes</span><span class="sxs-lookup"><span data-stu-id="a3336-153">personNotes</span></span>|<span data-ttu-id="a3336-154">String</span><span class="sxs-lookup"><span data-stu-id="a3336-154">String</span></span>|<span data-ttu-id="a3336-155">Frei formatierbare Notizen, die der Benutzer zu dieser Person hinzugefügt hat.</span><span class="sxs-lookup"><span data-stu-id="a3336-155">Free-form notes that the user has taken about this person.</span></span>|
|<span data-ttu-id="a3336-156">personType</span><span class="sxs-lookup"><span data-stu-id="a3336-156">personType</span></span>|[<span data-ttu-id="a3336-157">personType</span><span class="sxs-lookup"><span data-stu-id="a3336-157">personType</span></span>](persontype.md) |<span data-ttu-id="a3336-158">Der Personentyp.</span><span class="sxs-lookup"><span data-stu-id="a3336-158">The type of person.</span></span>|
|<span data-ttu-id="a3336-159">phones</span><span class="sxs-lookup"><span data-stu-id="a3336-159">phones</span></span>|<span data-ttu-id="a3336-160">[phone](phone.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a3336-160">[phone](phone.md) collection</span></span>|<span data-ttu-id="a3336-161">Die Telefonnummern der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-161">The person's phone numbers.</span></span>|
|<span data-ttu-id="a3336-162">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="a3336-162">postalAddresses</span></span>|<span data-ttu-id="a3336-163">[location](location.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a3336-163">[location](location.md) collection</span></span>|<span data-ttu-id="a3336-164">Die Adressen der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-164">The person's addresses.</span></span>|
|<span data-ttu-id="a3336-165">profession</span><span class="sxs-lookup"><span data-stu-id="a3336-165">profession</span></span>|<span data-ttu-id="a3336-166">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-166">String</span></span>|<span data-ttu-id="a3336-167">Der Beruf der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-167">The person's profession.</span></span>|
|<span data-ttu-id="a3336-168">surname</span><span class="sxs-lookup"><span data-stu-id="a3336-168">surname</span></span>|<span data-ttu-id="a3336-169">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-169">String</span></span>|<span data-ttu-id="a3336-170">Der Nachname der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-170">The person's surname.</span></span>|
|<span data-ttu-id="a3336-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a3336-171">userPrincipalName</span></span>|<span data-ttu-id="a3336-172">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-172">String</span></span>|<span data-ttu-id="a3336-p105">Der Benutzerprinzipalname der Person. Der UPN ist ein Anmeldename der Person im Internetformat, der auf dem Internetstandard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) basiert. Gemäß der Konvention sollte er dem E-Mail-Namen der Person zugeordnet sein. Das allgemeine Format lautet alias@domäne.</span><span class="sxs-lookup"><span data-stu-id="a3336-p105">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="a3336-177">websites</span><span class="sxs-lookup"><span data-stu-id="a3336-177">websites</span></span>|<span data-ttu-id="a3336-178">[website](website.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="a3336-178">[website](website.md) collection</span></span>|<span data-ttu-id="a3336-179">Die Websites der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-179">The person's websites.</span></span>|
|<span data-ttu-id="a3336-180">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="a3336-180">yomiCompany</span></span>|<span data-ttu-id="a3336-181">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a3336-181">String</span></span>|<span data-ttu-id="a3336-182">Der phonetische japanische Firmenname des Unternehmens der Person.</span><span class="sxs-lookup"><span data-stu-id="a3336-182">The phonetic Japanese name of the person's company.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a3336-183">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a3336-183">Relationships</span></span>

<span data-ttu-id="a3336-184">Keine.</span><span class="sxs-lookup"><span data-stu-id="a3336-184">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a3336-185">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a3336-185">JSON representation</span></span>

<span data-ttu-id="a3336-186">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a3336-186">The following is a JSON representation of the resource.</span></span>

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
