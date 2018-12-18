---
title: Personen auflisten
description: Dient zum Abrufen einer Sammlung von person-Objekten, die nach ihrer Relevanz für den Benutzer sortiert sind, die von den Mustern bei Kommunikation, Zusammenarbeit und den Geschäftsbeziehungen des Benutzers abhängt.
author: simonhult
ms.openlocfilehash: 52f3dade14af76732381bf71f0d8556f543287fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350113"
---
# <a name="list-people"></a><span data-ttu-id="b0317-103">Personen auflisten</span><span class="sxs-lookup"><span data-stu-id="b0317-103">List people</span></span>

<span data-ttu-id="b0317-104">Dient zum Abrufen einer Sammlung von [person](../resources/person.md)-Objekten, die nach ihrer Relevanz für den [Benutzer](../resources/user.md) sortiert sind, die von den Mustern bei Kommunikation, Zusammenarbeit und den Geschäftsbeziehungen des Benutzers abhängt.</span><span class="sxs-lookup"><span data-stu-id="b0317-104">Retrieve a collection of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

<span data-ttu-id="b0317-p101">Sie können diese Informationen über die People API abrufen. Beispiele finden Sie in dem Abschnitt [Beispiele](#examples) sowie im Artikel zum Thema [Abrufen relevanter Informationen über Personen](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="b0317-p101">You can get this information via the People API. For examples, see the [Examples](#examples) section and the article [Get relevant information about people](/graph/people-example).</span></span>

## <a name="permissions"></a><span data-ttu-id="b0317-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b0317-107">Permissions</span></span>

<span data-ttu-id="b0317-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0317-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0317-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b0317-110">Permission type</span></span>      | <span data-ttu-id="b0317-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b0317-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b0317-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b0317-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b0317-113">People.Read, People.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0317-113">People.Read, People.Read.All</span></span>    |
|<span data-ttu-id="b0317-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b0317-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b0317-115">People.Read</span><span class="sxs-lookup"><span data-stu-id="b0317-115">People.Read</span></span>    |
|<span data-ttu-id="b0317-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b0317-116">Application</span></span> | <span data-ttu-id="b0317-117">People.Read.All</span><span class="sxs-lookup"><span data-stu-id="b0317-117">People.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b0317-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0317-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b0317-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="b0317-119">Optional query parameters</span></span>

<span data-ttu-id="b0317-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters), um bei der Anpassung der Antwort zu helfen. Beispiele dazu finden Sie im Artikel [Abrufen relevanter Informationen über Personen](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="b0317-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, as shown in the examples in the article [Get relevant information about people](/graph/people-example).</span></span>

|<span data-ttu-id="b0317-121">Name</span><span class="sxs-lookup"><span data-stu-id="b0317-121">Name</span></span>|<span data-ttu-id="b0317-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b0317-122">Value</span></span>|<span data-ttu-id="b0317-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0317-123">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="b0317-124">$filter</span><span class="sxs-lookup"><span data-stu-id="b0317-124">$filter</span></span>|<span data-ttu-id="b0317-125">string</span><span class="sxs-lookup"><span data-stu-id="b0317-125">string</span></span>|<span data-ttu-id="b0317-126">Dient zum Einschränken der Antwort auf diejenigen Personen, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="b0317-126">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="b0317-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="b0317-127">$orderby</span></span>|<span data-ttu-id="b0317-128">string</span><span class="sxs-lookup"><span data-stu-id="b0317-128">string</span></span>|<span data-ttu-id="b0317-129">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert.</span><span class="sxs-lookup"><span data-stu-id="b0317-129">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="b0317-130">Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.</span><span class="sxs-lookup"><span data-stu-id="b0317-130">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="b0317-131">$search</span><span class="sxs-lookup"><span data-stu-id="b0317-131">$search</span></span>|<span data-ttu-id="b0317-132">string</span><span class="sxs-lookup"><span data-stu-id="b0317-132">string</span></span>|<span data-ttu-id="b0317-133">Dient für die Suche nach Personen anhand des Namens oder des Alias.</span><span class="sxs-lookup"><span data-stu-id="b0317-133">Search for people by name or alias.</span></span> <span data-ttu-id="b0317-134">Unterstützt Fuzzyübereinstimmung.</span><span class="sxs-lookup"><span data-stu-id="b0317-134">Supports Fuzzy matching.</span></span> <span data-ttu-id="b0317-135">Parameter funktioniert nur für die Suche des angemeldeten Benutzers zuständigen Personen, nicht zum Suchen von Personen, die für andere Benutzer relevant.</span><span class="sxs-lookup"><span data-stu-id="b0317-135">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="b0317-136">Unterstützt außerdem die `topic` Schlüsselwort Personensuche basierend auf Themen aus E-mail-Konversationen mit dieser Person extrahiert.</span><span class="sxs-lookup"><span data-stu-id="b0317-136">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="b0317-137">Siehe Abschnitt *Perform eine fuzzy-Suche* unter [Abrufen von relevante Informationen über Personen](/graph/people-example#perform-a-fuzzy-search) Informationen und Beispiele.</span><span class="sxs-lookup"><span data-stu-id="b0317-137">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span> |
|<span data-ttu-id="b0317-138">$select</span><span class="sxs-lookup"><span data-stu-id="b0317-138">$select</span></span>|<span data-ttu-id="b0317-139">string</span><span class="sxs-lookup"><span data-stu-id="b0317-139">string</span></span>|<span data-ttu-id="b0317-p105">Durch Trennzeichen getrennte Liste der Eigenschaften, die in die Antwort eingeschlossen werden sollen. Wählen Sie für optimale Leistung nur eine Teilmenge der benötigten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="b0317-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="b0317-142">$skip</span><span class="sxs-lookup"><span data-stu-id="b0317-142">$skip</span></span>|<span data-ttu-id="b0317-143">int</span><span class="sxs-lookup"><span data-stu-id="b0317-143">int</span></span>|<span data-ttu-id="b0317-p106">Die ersten n Ergebnisse werden übersprungen. Hilfreich für Paging. Wird bei Verwendung von *$search* nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b0317-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="b0317-146">$top</span><span class="sxs-lookup"><span data-stu-id="b0317-146">$top</span></span>|<span data-ttu-id="b0317-147">int</span><span class="sxs-lookup"><span data-stu-id="b0317-147">int</span></span>|<span data-ttu-id="b0317-148">Anzahl der Ergebnisse, die zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="b0317-148">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b0317-149">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b0317-149">Request headers</span></span>

| <span data-ttu-id="b0317-150">Name</span><span class="sxs-lookup"><span data-stu-id="b0317-150">Name</span></span>      |<span data-ttu-id="b0317-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0317-151">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b0317-152">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0317-152">Authorization</span></span>  | <span data-ttu-id="b0317-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b0317-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b0317-155">Accept</span><span class="sxs-lookup"><span data-stu-id="b0317-155">Accept</span></span> | <span data-ttu-id="b0317-156">application/json</span><span class="sxs-lookup"><span data-stu-id="b0317-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b0317-157">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b0317-157">Request body</span></span>

<span data-ttu-id="b0317-158">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b0317-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0317-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0317-159">Response</span></span>

<span data-ttu-id="b0317-p108">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [person](../resources/person.md)-Objekten im Antworttext zurückgegeben. Die Antwort kann ein person-Objekt oder eine Sammlung von person-Objekten enthalten.</span><span class="sxs-lookup"><span data-stu-id="b0317-p108">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body. The response can contain one person object or a collection of person objects.</span></span>

## <a name="examples"></a><span data-ttu-id="b0317-162">Beispiele</span><span class="sxs-lookup"><span data-stu-id="b0317-162">Examples</span></span>

#### <a name="request"></a><span data-ttu-id="b0317-163">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b0317-163">Request</span></span>

<span data-ttu-id="b0317-164">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b0317-164">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_person_collection"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/people
```

#### <a name="response"></a><span data-ttu-id="b0317-165">Antwort</span><span class="sxs-lookup"><span data-stu-id="b0317-165">Response</span></span>

<span data-ttu-id="b0317-166">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b0317-166">The following is an example of the response.</span></span>

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

<span data-ttu-id="b0317-167">Weitere Beispiele finden Sie im Artikel [Abrufen relevanter Informationen über Personen](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="b0317-167">For more examples, see the article [Get relevant information about people](/graph/people-example).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
