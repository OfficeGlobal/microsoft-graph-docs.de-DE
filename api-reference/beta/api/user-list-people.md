---
title: Personen auflisten
description: Abrufen einer Liste von Person-Objekten sortiert nach ihrer Relevanz für den Benutzer, die durch des Benutzers Kommunikation und Zusammenarbeit Muster und geschäftliche Beziehungen bestimmt wird.
author: dkershaw10
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: deb9fd929a2b0b8ce4da9392cb465497c2236b0c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517813"
---
# <a name="list-people"></a><span data-ttu-id="a26ef-103">Personen auflisten</span><span class="sxs-lookup"><span data-stu-id="a26ef-103">List people</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a26ef-104">Abrufen einer Liste von [Person](../resources/person.md) -Objekten sortiert nach ihrer Relevanz für den [Benutzer](../resources/user.md), die durch des Benutzers Kommunikation und Zusammenarbeit Muster und geschäftliche Beziehungen bestimmt wird.</span><span class="sxs-lookup"><span data-stu-id="a26ef-104">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="a26ef-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a26ef-105">Permissions</span></span>

<span data-ttu-id="a26ef-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a26ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a26ef-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a26ef-108">Permission type</span></span>      | <span data-ttu-id="a26ef-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a26ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a26ef-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a26ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a26ef-111">People.Read</span><span class="sxs-lookup"><span data-stu-id="a26ef-111">People.Read</span></span>    |
|<span data-ttu-id="a26ef-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a26ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a26ef-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="a26ef-113">People.Read</span></span>    |
|<span data-ttu-id="a26ef-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a26ef-114">Application</span></span> | <span data-ttu-id="a26ef-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a26ef-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a26ef-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a26ef-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a26ef-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a26ef-117">Optional query parameters</span></span>

<span data-ttu-id="a26ef-118">Diese Methode unterstützt die folgenden Parameter der OData-Abfrage, mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="a26ef-118">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="a26ef-119">Name</span><span class="sxs-lookup"><span data-stu-id="a26ef-119">Name</span></span>|<span data-ttu-id="a26ef-120">Wert</span><span class="sxs-lookup"><span data-stu-id="a26ef-120">Value</span></span>|<span data-ttu-id="a26ef-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a26ef-121">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="a26ef-122">$filter</span><span class="sxs-lookup"><span data-stu-id="a26ef-122">$filter</span></span>|<span data-ttu-id="a26ef-123">string</span><span class="sxs-lookup"><span data-stu-id="a26ef-123">string</span></span>|<span data-ttu-id="a26ef-124">Dient zum Einschränken der Antwort auf diejenigen Personen, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="a26ef-124">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="a26ef-125">$orderby</span><span class="sxs-lookup"><span data-stu-id="a26ef-125">$orderby</span></span>|<span data-ttu-id="a26ef-126">string</span><span class="sxs-lookup"><span data-stu-id="a26ef-126">string</span></span>|<span data-ttu-id="a26ef-127">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert.</span><span class="sxs-lookup"><span data-stu-id="a26ef-127">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="a26ef-128">Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.</span><span class="sxs-lookup"><span data-stu-id="a26ef-128">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="a26ef-129">$search</span><span class="sxs-lookup"><span data-stu-id="a26ef-129">$search</span></span>|<span data-ttu-id="a26ef-130">string</span><span class="sxs-lookup"><span data-stu-id="a26ef-130">string</span></span>|<span data-ttu-id="a26ef-131">Dient für die Suche nach Personen anhand des Namens oder des Alias.</span><span class="sxs-lookup"><span data-stu-id="a26ef-131">Search for people by name or alias.</span></span> <span data-ttu-id="a26ef-132">Unterstützt Fuzzyübereinstimmung.</span><span class="sxs-lookup"><span data-stu-id="a26ef-132">Supports Fuzzy matching.</span></span> <span data-ttu-id="a26ef-133">Parameter funktioniert nur für die Suche des angemeldeten Benutzers zuständigen Personen, nicht zum Suchen von Personen, die für andere Benutzer relevant.</span><span class="sxs-lookup"><span data-stu-id="a26ef-133">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="a26ef-134">Unterstützt außerdem die `topic` Schlüsselwort Personensuche basierend auf Themen aus E-mail-Konversationen mit dieser Person extrahiert.</span><span class="sxs-lookup"><span data-stu-id="a26ef-134">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="a26ef-135">Siehe Abschnitt *Perform eine fuzzy-Suche* unter [Abrufen von relevante Informationen über Personen](/graph/people-example#perform-a-fuzzy-search) Informationen und Beispiele.</span><span class="sxs-lookup"><span data-stu-id="a26ef-135">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="a26ef-136">$select</span><span class="sxs-lookup"><span data-stu-id="a26ef-136">$select</span></span>|<span data-ttu-id="a26ef-137">string</span><span class="sxs-lookup"><span data-stu-id="a26ef-137">string</span></span>|<span data-ttu-id="a26ef-p104">Durch Trennzeichen getrennte Liste der Eigenschaften, die in die Antwort eingeschlossen werden sollen. Wählen Sie für optimale Leistung nur eine Teilmenge der benötigten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="a26ef-p104">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="a26ef-140">$skip</span><span class="sxs-lookup"><span data-stu-id="a26ef-140">$skip</span></span>|<span data-ttu-id="a26ef-141">int</span><span class="sxs-lookup"><span data-stu-id="a26ef-141">int</span></span>|<span data-ttu-id="a26ef-p105">Die ersten n Ergebnisse werden übersprungen. Hilfreich für Paging. Wird bei Verwendung von *$search* nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a26ef-p105">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="a26ef-144">$top</span><span class="sxs-lookup"><span data-stu-id="a26ef-144">$top</span></span>|<span data-ttu-id="a26ef-145">int</span><span class="sxs-lookup"><span data-stu-id="a26ef-145">int</span></span>|<span data-ttu-id="a26ef-146">Anzahl der Ergebnisse, die zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="a26ef-146">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="a26ef-147">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a26ef-147">Request headers</span></span>

| <span data-ttu-id="a26ef-148">Name</span><span class="sxs-lookup"><span data-stu-id="a26ef-148">Name</span></span>      |<span data-ttu-id="a26ef-149">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a26ef-149">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a26ef-150">Authorization</span><span class="sxs-lookup"><span data-stu-id="a26ef-150">Authorization</span></span>  | <span data-ttu-id="a26ef-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a26ef-p106">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a26ef-153">Annehmen</span><span class="sxs-lookup"><span data-stu-id="a26ef-153">Accept</span></span> | <span data-ttu-id="a26ef-154">application/json</span><span class="sxs-lookup"><span data-stu-id="a26ef-154">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a26ef-155">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a26ef-155">Request body</span></span>

<span data-ttu-id="a26ef-156">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a26ef-156">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a26ef-157">Antwort</span><span class="sxs-lookup"><span data-stu-id="a26ef-157">Response</span></span>

<span data-ttu-id="a26ef-158">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [Person](../resources/person.md) .</span><span class="sxs-lookup"><span data-stu-id="a26ef-158">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a26ef-159">Beispiele</span><span class="sxs-lookup"><span data-stu-id="a26ef-159">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="a26ef-160">Durchsuchen</span><span class="sxs-lookup"><span data-stu-id="a26ef-160">Browse</span></span>

<span data-ttu-id="a26ef-161">Die Anforderungen in diesem Abschnitt die Personen Abrufen der angemeldeten Benutzer am relevantesten (`/me`), basierend auf Kommunikation, Zusammenarbeit und Business Beziehungen.</span><span class="sxs-lookup"><span data-stu-id="a26ef-161">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="a26ef-162">Standardmäßig gibt jede Antwort 10 Datensätze zurück, aber Sie können *dies* mit dem Parameter $top ändern.</span><span class="sxs-lookup"><span data-stu-id="a26ef-162">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="a26ef-163">Diese Anfragen erfordern die People.Read-Berechtigung an.</span><span class="sxs-lookup"><span data-stu-id="a26ef-163">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="a26ef-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a26ef-164">Request</span></span>

<span data-ttu-id="a26ef-165">Es folgt ein Beispiel für die Standard-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a26ef-165">The following is an example of the default request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a><span data-ttu-id="a26ef-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="a26ef-166">Response</span></span>

<span data-ttu-id="a26ef-167">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a26ef-167">The following is an example of the response.</span></span>
><span data-ttu-id="a26ef-p108">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="a26ef-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_person_collection_beta",
  "truncated": true,
  "@odata.type": "microsoft.graph.person",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1326

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
            "title": null,
            "companyName": null,
            "yomiCompany": "",
            "department": null,
            "officeLocation": null,
            "profession": "",
            "mailboxType": "GroupMailbox",
            "personType": "ModernGroup",
            "userPrincipalName": "",
            "emailAddresses": [
                {
                    "address": "Marketing@contoso.com",
                    "rank": 30
                }
            ],
            "phones": [],
            "postalAddresses": [],
            "websites": [],
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        },
        {
            "id": "e3d0513b-449e-4198-ba6f-bd97ae7cae85",
            "displayName": "Isaiah Langer",
            "givenName": "Isaiah",
            "surname": "Langer",
            "birthday": "",
            "personNotes": "",
            "isFavorite": false,
            "title": "Web Marketing Manager",
            "companyName": null,
            "yomiCompany": "",
            "department": "Sales & Marketing",
            "officeLocation": "20/1101",
            "profession": "",
            "mailboxType": "Mailbox",
            "personType": "Person",
            "userPrincipalName": "IsaiahL@contoso.com",
            "emailAddresses": [
                {
                    "address": "IsaiahL@contoso.com",
                    "rank": 20
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
            "sources": [
                {
                    "type": "Directory"
                }
            ]
        }
    ]
}
```

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="a26ef-170">Anfordern einer nachfolgenden Seite von Personen</span><span class="sxs-lookup"><span data-stu-id="a26ef-170">Requesting a subsequent page of people</span></span>

<span data-ttu-id="a26ef-p109">Wenn die erste Antwort nicht die vollständige Liste der relevanten Personen enthält, können Sie mit *$top* und *$skip* eine zweite Anforderung für das Abrufen weiterer Seiten mit Informationen einreichen. Wenn die vorherige Anforderung zusätzliche Informationen enthält, ruft die darauf folgende Anforderung die nächste Seite der Personen vom Server ab.</span><span class="sxs-lookup"><span data-stu-id="a26ef-p109">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="a26ef-173">Sortieren der Antwort</span><span class="sxs-lookup"><span data-stu-id="a26ef-173">Sort the response</span></span>

<span data-ttu-id="a26ef-174">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert.</span><span class="sxs-lookup"><span data-stu-id="a26ef-174">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="a26ef-175">Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.</span><span class="sxs-lookup"><span data-stu-id="a26ef-175">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="a26ef-176">Diese Abfrage wählt die für Sie relevantesten Personen aus, sortiert sie nach ihrem Anzeigenamen und gibt dann die ersten 10 Personen auf der sortierten Liste zurück.</span><span class="sxs-lookup"><span data-stu-id="a26ef-176">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="a26ef-177"> Ändern der Anzahl der zurückgegebenen Personen und der zurückgegebenen Felder</span><span class="sxs-lookup"><span data-stu-id="a26ef-177">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="a26ef-178">Sie können die Anzahl der Personen ändern, die in der Antwort zurückgegeben wird, indem Sie den *$top*-Parameter festlegen.</span><span class="sxs-lookup"><span data-stu-id="a26ef-178">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="a26ef-179">Das folgende Beispiel fordert den 1.000 Mitarbeiter am relevantesten `/me`.</span><span class="sxs-lookup"><span data-stu-id="a26ef-179">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="a26ef-180">Die Anforderung schränkt auch die Menge der Daten, die vom Server gesendet werden, indem nur den Anzeigenamen der Person anfordern.</span><span class="sxs-lookup"><span data-stu-id="a26ef-180">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="a26ef-181"> Auswahl der zurückzugebenden Felder</span><span class="sxs-lookup"><span data-stu-id="a26ef-181">Selecting the fields to return</span></span>

<span data-ttu-id="a26ef-182">Sie können die Menge der Daten vom Server mithilfe des *$select* -Parameters ein oder mehrere Felder auswählen zurückgegebenen einschränken.</span><span class="sxs-lookup"><span data-stu-id="a26ef-182">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="a26ef-183">Das Feld *@odata.id* wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a26ef-183">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="a26ef-184">Im folgende Beispiel wird die Antwort auf die *DisplayName* und *EmailAddress* die 10 wichtigsten Benutzer beschränkt.</span><span class="sxs-lookup"><span data-stu-id="a26ef-184">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="a26ef-185"> Verwendung eines Filters zur Begrenzung der Antwort</span><span class="sxs-lookup"><span data-stu-id="a26ef-185">Using a filter to limit the response</span></span>

<span data-ttu-id="a26ef-186">Sie können den *$filter*-Parameter zum Einschränken der Antwort auf diejenigen Personen einschränken, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="a26ef-186">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="a26ef-187">Die folgende Abfrage beschränkt die Antwort an Personen mit der Quelle "Verzeichnis".</span><span class="sxs-lookup"><span data-stu-id="a26ef-187">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="a26ef-188">Auswählen der Felder, die in eine gefilterte Antwort zurückgegeben</span><span class="sxs-lookup"><span data-stu-id="a26ef-188">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="a26ef-189">Sie können die *$select*- und *$filter*-Parameter gemeinsam verwenden, um eine benutzerdefinierte Liste der für den Benutzer relevanten Personen zu erstellen und nur die Felder abzurufen, die Ihre Anwendung benötigt.</span><span class="sxs-lookup"><span data-stu-id="a26ef-189">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="a26ef-190">Das folgende Beispiel ruft die *DisplayName* und *EmailAddress* von Personen, deren Anzeigename den angegebenen Namen entspricht.</span><span class="sxs-lookup"><span data-stu-id="a26ef-190">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="a26ef-191">In diesem Beispiel werden nur Personen zurückgegeben, deren Anzeigename "Nestor Kellum" ist.</span><span class="sxs-lookup"><span data-stu-id="a26ef-191">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="a26ef-192">Durchsuchen von Personen</span><span class="sxs-lookup"><span data-stu-id="a26ef-192">Search people</span></span>

<span data-ttu-id="a26ef-193">Die Anforderungen in diesem Abschnitt auch die Personen Abrufen der angemeldeten Benutzer am relevantesten (`/me`).</span><span class="sxs-lookup"><span data-stu-id="a26ef-193">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="a26ef-194">Suchanforderungen erfordern die People.Read-Berechtigung an.</span><span class="sxs-lookup"><span data-stu-id="a26ef-194">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="a26ef-195">Wählen Sie Personen mithilfe der Suche</span><span class="sxs-lookup"><span data-stu-id="a26ef-195">Using search to select people</span></span>

<span data-ttu-id="a26ef-196">Verwenden Sie den *$search*-Parameter zum Auswählen von Personen, die bestimmte Kriterien erfüllen.</span><span class="sxs-lookup"><span data-stu-id="a26ef-196">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="a26ef-197">Die folgenden Suchabfrage zurückgibt Personen für die Überprüfung relevante `/me` , deren Vorname oder Nachname beginnt mit dem Buchstaben "j".</span><span class="sxs-lookup"><span data-stu-id="a26ef-197">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="a26ef-198"> Mit der Suche ein relevantes Thema angeben</span><span class="sxs-lookup"><span data-stu-id="a26ef-198">Using search to specify a relevant topic</span></span>

<span data-ttu-id="a26ef-199">Die folgende Anforderung gibt Personen für die Überprüfung relevante `/me` , deren Namen enthält "Ma" und besitzen eine Zuordnung mit "Feature planen".</span><span class="sxs-lookup"><span data-stu-id="a26ef-199">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="a26ef-200">  Fuzzy-Suche durchführen</span><span class="sxs-lookup"><span data-stu-id="a26ef-200">Performing a fuzzy search</span></span>

<span data-ttu-id="a26ef-201">Die folgende Anforderung wird eine Suche nach einer Person, die mit dem Namen "Hermaini Saal."</span><span class="sxs-lookup"><span data-stu-id="a26ef-201">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="a26ef-202">Da eine Person, die mit dem Namen "Herminia Hülle" für den angemeldeten Benutzer relevant ist, wird die Informationen für "Herminia Hülle" zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a26ef-202">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="a26ef-203">Verwandte Personen</span><span class="sxs-lookup"><span data-stu-id="a26ef-203">Related people</span></span>

<span data-ttu-id="a26ef-204">Die folgende Anforderung Ruft die Personen in der Organisation des Benutzers relevantesten an eine andere Person.</span><span class="sxs-lookup"><span data-stu-id="a26ef-204">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="a26ef-205">Diese Anforderung erfordert die User.ReadBasic.All für People.Read.All-Berechtigung an.</span><span class="sxs-lookup"><span data-stu-id="a26ef-205">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="a26ef-206">In diesem Beispiel werden die Nestor Kellums entsprechenden Personen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="a26ef-206">In this example, Nestor Kellum's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-people.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
