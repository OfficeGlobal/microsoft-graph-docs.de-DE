---
title: Die Benutzeraktivitäten abrufen
description: Rufen Sie Aktivitäten für einen bestimmten Benutzer. Aktivitäten ohne gespeichert werden soll, im Gegensatz zu der **letzte** OData-Funktion zurückgegeben. Die Berechtigung UserActivity.ReadWrite.CreatedByApp gelten zusätzliche Filter auf die Antwort, damit nur Aktivitäten, die von der Anwendung erstellt zurückgegeben werden. Diese serverseitige Filterung auftreten auf leere Seiten, wenn der Benutzer besonders aktiv ist und anderen Applikationen neuere Aktivitäten erstellt haben. Wenn Sie Ihre Anwendung Aktivitäten erhalten möchten, verwenden Sie die **NextLink** -Eigenschaft für die Paginierung.
localization_priority: Normal
ms.openlocfilehash: 8106d1c2cb740033fd81a21068aba5a15fd1b1b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809373"
---
# <a name="get-user-activities"></a><span data-ttu-id="1255c-107">Die Benutzeraktivitäten abrufen</span><span class="sxs-lookup"><span data-stu-id="1255c-107">Get user activities</span></span>

> <span data-ttu-id="1255c-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1255c-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1255c-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1255c-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1255c-110">Rufen Sie Aktivitäten für einen bestimmten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="1255c-110">Get activities for a given user.</span></span> <span data-ttu-id="1255c-111">Aktivitäten ohne gespeichert werden soll, im Gegensatz zu der **letzte** OData-Funktion zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1255c-111">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="1255c-112">Die Berechtigung UserActivity.ReadWrite.CreatedByApp gelten zusätzliche Filter auf die Antwort, damit nur Aktivitäten, die von der Anwendung erstellt zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="1255c-112">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="1255c-113">Diese serverseitige Filterung auftreten auf leere Seiten, wenn der Benutzer besonders aktiv ist und anderen Applikationen neuere Aktivitäten erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="1255c-113">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="1255c-114">Wenn Sie Ihre Anwendung Aktivitäten erhalten möchten, verwenden Sie die **NextLink** -Eigenschaft für die Paginierung.</span><span class="sxs-lookup"><span data-stu-id="1255c-114">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="1255c-115">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1255c-115">Permissions</span></span>

<span data-ttu-id="1255c-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1255c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1255c-118">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1255c-118">Permission type</span></span>      | <span data-ttu-id="1255c-119">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1255c-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1255c-120">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1255c-120">Delegated (work or school account)</span></span> | <span data-ttu-id="1255c-121">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1255c-121">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1255c-122">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1255c-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1255c-123">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1255c-123">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1255c-124">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1255c-124">Application</span></span> | <span data-ttu-id="1255c-125">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1255c-125">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1255c-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1255c-126">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1255c-127">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1255c-127">Optional query parameters</span></span>

<span data-ttu-id="1255c-128">Diese Methode unterstützt einige [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="1255c-128">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="1255c-129">Die folgenden Abfrageparameter werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="1255c-129">The following query parameters are supported:</span></span>

- <span data-ttu-id="1255c-130">$ Erweitern Sie für die Eigenschaft **HistoryItems** Navigation.</span><span class="sxs-lookup"><span data-stu-id="1255c-130">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="1255c-131">$top um die maximale Anzahl von Elementen auf mehreren Seiten zu begrenzen.</span><span class="sxs-lookup"><span data-stu-id="1255c-131">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="1255c-132">$filter auf die **LastModifiedDateTime** -Eigenschaft für **Aktivitäten** oder **HistoryItems**, wenn erweitert.</span><span class="sxs-lookup"><span data-stu-id="1255c-132">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="1255c-133">Es folgen einige Beispiele für unterstützte Abfragen mit URL-Codierung:</span><span class="sxs-lookup"><span data-stu-id="1255c-133">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="1255c-134">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1255c-134">Request headers</span></span>

|<span data-ttu-id="1255c-135">Name</span><span class="sxs-lookup"><span data-stu-id="1255c-135">Name</span></span> | <span data-ttu-id="1255c-136">Typ</span><span class="sxs-lookup"><span data-stu-id="1255c-136">Type</span></span> | <span data-ttu-id="1255c-137">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1255c-137">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="1255c-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="1255c-138">Authorization</span></span> | <span data-ttu-id="1255c-139">string</span><span class="sxs-lookup"><span data-stu-id="1255c-139">string</span></span> | <span data-ttu-id="1255c-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1255c-p106">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1255c-142">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1255c-142">Request body</span></span>

<span data-ttu-id="1255c-143">Keine Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="1255c-143">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="1255c-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="1255c-144">Response</span></span>

<span data-ttu-id="1255c-145">Wenn der Vorgang erfolgreich war, gibt diese Methode die `200 OK` Antwortcode mit die Aktivitäten des Benutzers für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="1255c-145">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="1255c-146">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1255c-146">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1255c-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1255c-147">Request</span></span>

<span data-ttu-id="1255c-148">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1255c-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/beta/me/activities
```

##### <a name="response"></a><span data-ttu-id="1255c-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="1255c-149">Response</span></span>

<span data-ttu-id="1255c-150">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1255c-150">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.activity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": "false",
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "https://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "https://www.contoso.com/article?id=12345",
        "contentUrl": "https://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "https://schema.org",
            "@type": "Article",
            "author": "John Doe",
            "name": "How to Tie a Reef Knot"
        },
        "expirationDateTime": "2018-03-28T18:34:29.607Z",
        "status": "updated"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
