---
title: Personen auflisten
description: Abrufen einer Liste von Person-Objekten sortiert nach ihrer Relevanz für den Benutzer, die durch des Benutzers Kommunikation und Zusammenarbeit Muster und geschäftliche Beziehungen bestimmt wird.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 3bd9c8cdd3737cbd8d96fd4f9b24f5382ce04793
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872779"
---
# <a name="list-people"></a><span data-ttu-id="d667c-103">Personen auflisten</span><span class="sxs-lookup"><span data-stu-id="d667c-103">List people</span></span>

> <span data-ttu-id="d667c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d667c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d667c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d667c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d667c-106">Abrufen einer Liste von [Person](../resources/person.md) -Objekten sortiert nach ihrer Relevanz für den [Benutzer](../resources/user.md), die durch des Benutzers Kommunikation und Zusammenarbeit Muster und geschäftliche Beziehungen bestimmt wird.</span><span class="sxs-lookup"><span data-stu-id="d667c-106">Retrieve a list of [person](../resources/person.md) objects ordered by their relevance to the [user](../resources/user.md), which is determined by the user's communication and collaboration patterns, and business relationships.</span></span>

## <a name="permissions"></a><span data-ttu-id="d667c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d667c-107">Permissions</span></span>

<span data-ttu-id="d667c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d667c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d667c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d667c-110">Permission type</span></span>      | <span data-ttu-id="d667c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d667c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d667c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d667c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d667c-113">People.Read</span><span class="sxs-lookup"><span data-stu-id="d667c-113">People.Read</span></span>    |
|<span data-ttu-id="d667c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d667c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d667c-115">People.Read</span><span class="sxs-lookup"><span data-stu-id="d667c-115">People.Read</span></span>    |
|<span data-ttu-id="d667c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d667c-116">Application</span></span> | <span data-ttu-id="d667c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d667c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d667c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d667c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/people
GET /users/{id | userPrincipalName}/people
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d667c-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="d667c-119">Optional query parameters</span></span>

<span data-ttu-id="d667c-120">Diese Methode unterstützt die folgenden Parameter der OData-Abfrage, mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="d667c-120">This method supports the following OData query parameters to help customize the response.</span></span>

|<span data-ttu-id="d667c-121">Name</span><span class="sxs-lookup"><span data-stu-id="d667c-121">Name</span></span>|<span data-ttu-id="d667c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="d667c-122">Value</span></span>|<span data-ttu-id="d667c-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d667c-123">Description</span></span>|
|:---------------|:--------|:-------|
|<span data-ttu-id="d667c-124">$filter</span><span class="sxs-lookup"><span data-stu-id="d667c-124">$filter</span></span>|<span data-ttu-id="d667c-125">string</span><span class="sxs-lookup"><span data-stu-id="d667c-125">string</span></span>|<span data-ttu-id="d667c-126">Dient zum Einschränken der Antwort auf diejenigen Personen, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="d667c-126">Limits the response to only those people whose record contains the specified criteria.</span></span>|
|<span data-ttu-id="d667c-127">$orderby</span><span class="sxs-lookup"><span data-stu-id="d667c-127">$orderby</span></span>|<span data-ttu-id="d667c-128">string</span><span class="sxs-lookup"><span data-stu-id="d667c-128">string</span></span>|<span data-ttu-id="d667c-129">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert.</span><span class="sxs-lookup"><span data-stu-id="d667c-129">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="d667c-130">Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.</span><span class="sxs-lookup"><span data-stu-id="d667c-130">You can change the order of the people in the response using the *$orderby* parameter.</span></span>|
|<span data-ttu-id="d667c-131">$search</span><span class="sxs-lookup"><span data-stu-id="d667c-131">$search</span></span>|<span data-ttu-id="d667c-132">string</span><span class="sxs-lookup"><span data-stu-id="d667c-132">string</span></span>|<span data-ttu-id="d667c-133">Dient für die Suche nach Personen anhand des Namens oder des Alias.</span><span class="sxs-lookup"><span data-stu-id="d667c-133">Search for people by name or alias.</span></span> <span data-ttu-id="d667c-134">Unterstützt Fuzzyübereinstimmung.</span><span class="sxs-lookup"><span data-stu-id="d667c-134">Supports Fuzzy matching.</span></span> <span data-ttu-id="d667c-135">Parameter funktioniert nur für die Suche des angemeldeten Benutzers zuständigen Personen, nicht zum Suchen von Personen, die für andere Benutzer relevant.</span><span class="sxs-lookup"><span data-stu-id="d667c-135">Parameter only works for searching the signed-in user's relevant people, not for searching people relevant to other users.</span></span> <span data-ttu-id="d667c-136">Unterstützt außerdem die `topic` Schlüsselwort Personensuche basierend auf Themen aus E-mail-Konversationen mit dieser Person extrahiert.</span><span class="sxs-lookup"><span data-stu-id="d667c-136">Also supports the `topic` keyword to find people based on topics extracted from e-mail conversations with that person.</span></span> <span data-ttu-id="d667c-137">Siehe Abschnitt *Perform eine fuzzy-Suche* unter [Abrufen von relevante Informationen über Personen](/graph/people-example#perform-a-fuzzy-search) Informationen und Beispiele.</span><span class="sxs-lookup"><span data-stu-id="d667c-137">See the *Perform a fuzzy search* section at [Get relevant information about people](/graph/people-example#perform-a-fuzzy-search) for information and examples.</span></span>|
|<span data-ttu-id="d667c-138">$select</span><span class="sxs-lookup"><span data-stu-id="d667c-138">$select</span></span>|<span data-ttu-id="d667c-139">string</span><span class="sxs-lookup"><span data-stu-id="d667c-139">string</span></span>|<span data-ttu-id="d667c-p105">Durch Trennzeichen getrennte Liste der Eigenschaften, die in die Antwort eingeschlossen werden sollen. Wählen Sie für optimale Leistung nur eine Teilmenge der benötigten Eigenschaften.</span><span class="sxs-lookup"><span data-stu-id="d667c-p105">Comma-separated list of properties to include in the response. For optimal performance, only select the subset of properties needed.</span></span>|
|<span data-ttu-id="d667c-142">$skip</span><span class="sxs-lookup"><span data-stu-id="d667c-142">$skip</span></span>|<span data-ttu-id="d667c-143">int</span><span class="sxs-lookup"><span data-stu-id="d667c-143">int</span></span>|<span data-ttu-id="d667c-p106">Die ersten n Ergebnisse werden übersprungen. Hilfreich für Paging. Wird bei Verwendung von *$search* nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d667c-p106">Skip the first n results, useful for paging. This is not supported when using *$search*.</span></span>|
|<span data-ttu-id="d667c-146">$top</span><span class="sxs-lookup"><span data-stu-id="d667c-146">$top</span></span>|<span data-ttu-id="d667c-147">int</span><span class="sxs-lookup"><span data-stu-id="d667c-147">int</span></span>|<span data-ttu-id="d667c-148">Anzahl der Ergebnisse, die zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="d667c-148">Number of results to be returned.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="d667c-149">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d667c-149">Request headers</span></span>

| <span data-ttu-id="d667c-150">Name</span><span class="sxs-lookup"><span data-stu-id="d667c-150">Name</span></span>      |<span data-ttu-id="d667c-151">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d667c-151">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d667c-152">Authorization</span><span class="sxs-lookup"><span data-stu-id="d667c-152">Authorization</span></span>  | <span data-ttu-id="d667c-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d667c-p107">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d667c-155">Annehmen</span><span class="sxs-lookup"><span data-stu-id="d667c-155">Accept</span></span> | <span data-ttu-id="d667c-156">application/json</span><span class="sxs-lookup"><span data-stu-id="d667c-156">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d667c-157">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d667c-157">Request body</span></span>

<span data-ttu-id="d667c-158">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d667c-158">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d667c-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="d667c-159">Response</span></span>

<span data-ttu-id="d667c-160">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [Person](../resources/person.md) .</span><span class="sxs-lookup"><span data-stu-id="d667c-160">If successful, this method returns a `200 OK` response code and a collection of [person](../resources/person.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d667c-161">Beispiele</span><span class="sxs-lookup"><span data-stu-id="d667c-161">Examples</span></span>

### <a name="browse"></a><span data-ttu-id="d667c-162">Durchsuchen</span><span class="sxs-lookup"><span data-stu-id="d667c-162">Browse</span></span>

<span data-ttu-id="d667c-163">Die Anforderungen in diesem Abschnitt die Personen Abrufen der angemeldeten Benutzer am relevantesten (`/me`), basierend auf Kommunikation, Zusammenarbeit und Business Beziehungen.</span><span class="sxs-lookup"><span data-stu-id="d667c-163">The requests in this section get the people most relevant to the signed-in user (`/me`), based on communication, collaboration, and business relationships.</span></span>

<span data-ttu-id="d667c-164">Standardmäßig gibt jede Antwort 10 Datensätze zurück, aber Sie können dies mit dem Parameter *$top* ändern.</span><span class="sxs-lookup"><span data-stu-id="d667c-164">By default, each response returns 10 records, but you can change this using the *$top* parameter.</span></span> <span data-ttu-id="d667c-165">Diese Anfragen erfordern die People.Read-Berechtigung an.</span><span class="sxs-lookup"><span data-stu-id="d667c-165">These requests require the People.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="d667c-166">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d667c-166">Request</span></span>

<span data-ttu-id="d667c-167">Es folgt ein Beispiel für die Standard-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d667c-167">The following is an example of the default request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_person_collection_beta"
}-->

```http
GET https://graph.microsoft.com/beta/me/people
```

#### <a name="response"></a><span data-ttu-id="d667c-168">Antwort</span><span class="sxs-lookup"><span data-stu-id="d667c-168">Response</span></span>

<span data-ttu-id="d667c-169">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d667c-169">The following is an example of the response.</span></span>
><span data-ttu-id="d667c-p109">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d667c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

#### <a name="requesting-a-subsequent-page-of-people"></a><span data-ttu-id="d667c-172">Anfordern einer nachfolgenden Seite von Personen</span><span class="sxs-lookup"><span data-stu-id="d667c-172">Requesting a subsequent page of people</span></span>

<span data-ttu-id="d667c-p110">Wenn die erste Antwort nicht die vollständige Liste der relevanten Personen enthält, können Sie mit *$top* und *$skip* eine zweite Anforderung für das Abrufen weiterer Seiten mit Informationen einreichen. Wenn die vorherige Anforderung zusätzliche Informationen enthält, ruft die darauf folgende Anforderung die nächste Seite der Personen vom Server ab.</span><span class="sxs-lookup"><span data-stu-id="d667c-p110">If the first response does not contain the complete list of relevant people, you can make a second request using *$top* and *$skip* to request additional pages of information. If the previous request has additional information, the following request gets the next page of people from the server.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=10&$skip=10
```

#### <a name="sort-the-response"></a><span data-ttu-id="d667c-175">Sortieren der Antwort</span><span class="sxs-lookup"><span data-stu-id="d667c-175">Sort the response</span></span>

<span data-ttu-id="d667c-176">Standardmäßig werden die Personen in der Antwort nach ihrer Relevanz für die Abfrage sortiert.</span><span class="sxs-lookup"><span data-stu-id="d667c-176">By default the people in the response are sorted by their relevance to your query.</span></span> <span data-ttu-id="d667c-177">Sie können die Reihenfolge der Personen in der Antwort mit dem *$orderby*-Parameter ändern.</span><span class="sxs-lookup"><span data-stu-id="d667c-177">You can change the order of the people in the response using the *$orderby* parameter.</span></span> <span data-ttu-id="d667c-178">Diese Abfrage wählt die für Sie relevantesten Personen aus, sortiert sie nach ihrem Anzeigenamen und gibt dann die ersten 10 Personen auf der sortierten Liste zurück.</span><span class="sxs-lookup"><span data-stu-id="d667c-178">This query selects the people most relevant to you, sorts them by their display name, and then returns the first 10 people on the sorted list.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$orderby=DisplayName
```

#### <a name="changing-the-number-of-people-returned-and-the-fields-returned"></a><span data-ttu-id="d667c-179">Ändern der Anzahl der zurückgegebenen Personen und der zurückgegebenen Felder</span><span class="sxs-lookup"><span data-stu-id="d667c-179">Changing the number of people returned and the fields returned</span></span>

<span data-ttu-id="d667c-180">Sie können die Anzahl der Personen ändern, die in der Antwort zurückgegeben wird, indem Sie den *$top*-Parameter festlegen.</span><span class="sxs-lookup"><span data-stu-id="d667c-180">You can change the number of people returned in the response by setting the *$top* parameter.</span></span>

<span data-ttu-id="d667c-181">Das folgende Beispiel fordert den 1.000 Mitarbeiter am relevantesten `/me`.</span><span class="sxs-lookup"><span data-stu-id="d667c-181">The following example requests the 1,000 people most relevant to `/me`.</span></span> <span data-ttu-id="d667c-182">Die Anforderung schränkt auch die Menge der Daten, die vom Server gesendet werden, indem nur den Anzeigenamen der Person anfordern.</span><span class="sxs-lookup"><span data-stu-id="d667c-182">The request also limits the amount of data sent back from the server by requesting only the display name of the person.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$top=1000&$select=DisplayName
```

#### <a name="selecting-the-fields-to-return"></a><span data-ttu-id="d667c-183">Auswahl der zurückzugebenden Felder</span><span class="sxs-lookup"><span data-stu-id="d667c-183">Selecting the fields to return</span></span>

<span data-ttu-id="d667c-184">Sie können die Menge der Daten vom Server mithilfe des *$select* -Parameters ein oder mehrere Felder auswählen zurückgegebenen einschränken.</span><span class="sxs-lookup"><span data-stu-id="d667c-184">You can limit the amount of data returned from the server by using the *$select* parameter to choose one or more fields.</span></span> <span data-ttu-id="d667c-185">Das Feld *@odata.id* wird immer zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d667c-185">The *@odata.id* field is always returned.</span></span>

<span data-ttu-id="d667c-186">Im folgende Beispiel wird die Antwort auf die *DisplayName* und *EmailAddress* die 10 wichtigsten Benutzer beschränkt.</span><span class="sxs-lookup"><span data-stu-id="d667c-186">The following example limits the response to the *DisplayName* and *EmailAddress* of the 10 most relevant people.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses
```

#### <a name="using-a-filter-to-limit-the-response"></a><span data-ttu-id="d667c-187">Verwendung eines Filters zur Begrenzung der Antwort</span><span class="sxs-lookup"><span data-stu-id="d667c-187">Using a filter to limit the response</span></span>

<span data-ttu-id="d667c-188">Sie können den *$filter*-Parameter zum Einschränken der Antwort auf diejenigen Personen einschränken, deren Datensätze die angegebenen Kriterien enthalten.</span><span class="sxs-lookup"><span data-stu-id="d667c-188">You can use the *$filter* parameter to limit the response to only those people whose record contains the specified criteria.</span></span>

<span data-ttu-id="d667c-189">Die folgende Abfrage beschränkt die Antwort an Personen mit der Quelle "Verzeichnis".</span><span class="sxs-lookup"><span data-stu-id="d667c-189">The following query limits the response to people with the source "Directory."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$filter=Sources/Any (source: source/Type  eq 'Directory')
```

#### <a name="selecting-the-fields-to-return-in-a-filtered-response"></a><span data-ttu-id="d667c-190">Auswählen der Felder, die in eine gefilterte Antwort zurückgegeben</span><span class="sxs-lookup"><span data-stu-id="d667c-190">Selecting the fields to return in a filtered response</span></span>

<span data-ttu-id="d667c-191">Sie können die *$select*- und *$filter*-Parameter gemeinsam verwenden, um eine benutzerdefinierte Liste der für den Benutzer relevanten Personen zu erstellen und nur die Felder abzurufen, die Ihre Anwendung benötigt.</span><span class="sxs-lookup"><span data-stu-id="d667c-191">You can combine the *$select* and *$filter* parameters to create a custom list of people relevant to the user and get only the fields that your application needs.</span></span>

<span data-ttu-id="d667c-192">Das folgende Beispiel ruft die *DisplayName* und *EmailAddress* von Personen, deren Anzeigename den angegebenen Namen entspricht.</span><span class="sxs-lookup"><span data-stu-id="d667c-192">The following example gets the *DisplayName* and *EmailAddress* of people whose display name equals the specified name.</span></span> <span data-ttu-id="d667c-193">In diesem Beispiel werden nur Personen zurückgegeben, deren Anzeigename "Nestor Kellum" ist.</span><span class="sxs-lookup"><span data-stu-id="d667c-193">In this example, only people whose display name equals "Nestor Kellum" are returned.</span></span>

```http
+GET https://graph.microsoft.com/beta/me/people/?$select=DisplayName,EmailAddresses&$filter=DisplayName eq 'Nestor Kellum'
```

### <a name="search-people"></a><span data-ttu-id="d667c-194">Durchsuchen von Personen</span><span class="sxs-lookup"><span data-stu-id="d667c-194">Search people</span></span>

<span data-ttu-id="d667c-195">Die Anforderungen in diesem Abschnitt auch die Personen Abrufen der angemeldeten Benutzer am relevantesten (`/me`).</span><span class="sxs-lookup"><span data-stu-id="d667c-195">The requests in this section also get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="d667c-196">Suchanforderungen erfordern die People.Read-Berechtigung an.</span><span class="sxs-lookup"><span data-stu-id="d667c-196">Search requests require the People.Read permission.</span></span>

#### <a name="using-search-to-select-people"></a><span data-ttu-id="d667c-197">Wählen Sie Personen mithilfe der Suche</span><span class="sxs-lookup"><span data-stu-id="d667c-197">Using search to select people</span></span>

<span data-ttu-id="d667c-198">Verwenden Sie den *$search*-Parameter zum Auswählen von Personen, die bestimmte Kriterien erfüllen.</span><span class="sxs-lookup"><span data-stu-id="d667c-198">Use the *$search* parameter to select people who meet a particular set of criteria.</span></span>

<span data-ttu-id="d667c-199">Die folgenden Suchabfrage zurückgibt Personen für die Überprüfung relevante `/me` , deren Vorname oder Nachname beginnt mit dem Buchstaben "j".</span><span class="sxs-lookup"><span data-stu-id="d667c-199">The following search query returns people relevant to `/me` whose GivenName or Surname begins with the letter "j".</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search=j
```

#### <a name="using-search-to-specify-a-relevant-topic"></a><span data-ttu-id="d667c-200">Mit der Suche ein relevantes Thema angeben</span><span class="sxs-lookup"><span data-stu-id="d667c-200">Using search to specify a relevant topic</span></span>

<span data-ttu-id="d667c-201">Die folgende Anforderung gibt Personen für die Überprüfung relevante `/me` , deren Namen enthält "Ma" und besitzen eine Zuordnung mit "Feature planen".</span><span class="sxs-lookup"><span data-stu-id="d667c-201">The following request returns people relevant to `/me` whose name contains "ma" and who have an association with "feature planning."</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="ma topic: feature planning"
```

#### <a name="performing-a-fuzzy-search"></a><span data-ttu-id="d667c-202">Fuzzy-Suche durchführen</span><span class="sxs-lookup"><span data-stu-id="d667c-202">Performing a fuzzy search</span></span>

<span data-ttu-id="d667c-203">Die folgende Anforderung wird eine Suche nach einer Person, die mit dem Namen "Hermaini Saal."</span><span class="sxs-lookup"><span data-stu-id="d667c-203">The following request does a search for a person named "Hermaini Hall."</span></span> <span data-ttu-id="d667c-204">Da eine Person, die mit dem Namen "Herminia Hülle" für den angemeldeten Benutzer relevant ist, wird die Informationen für "Herminia Hülle" zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d667c-204">Because there is a person named "Herminia Hull" relevant to the signed-in user, the information for "Herminia Hull" is returned.</span></span>

```http
GET https://graph.microsoft.com/beta/me/people/?$search="hermaini hall"
```

### <a name="related-people"></a><span data-ttu-id="d667c-205">Verwandte Personen</span><span class="sxs-lookup"><span data-stu-id="d667c-205">Related people</span></span>

<span data-ttu-id="d667c-206">Die folgende Anforderung Ruft die Personen in der Organisation des Benutzers relevantesten an eine andere Person.</span><span class="sxs-lookup"><span data-stu-id="d667c-206">The following request gets the people most relevant to another person in the user's organization.</span></span> <span data-ttu-id="d667c-207">Diese Anforderung erfordert die User.ReadBasic.All für People.Read.All-Berechtigung an.</span><span class="sxs-lookup"><span data-stu-id="d667c-207">This request requires the User.ReadBasic.All for People.Read.All permission.</span></span> <span data-ttu-id="d667c-208">In diesem Beispiel werden die Nestor Kellums entsprechenden Personen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="d667c-208">In this example, Nestor Kellum's relevant people are displayed.</span></span>

```http
GET https://graph.microsoft.com/beta/users('nestork@contoso.com')/people/
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List people",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
