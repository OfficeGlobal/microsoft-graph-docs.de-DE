---
title: Die Benutzeraktivitäten abrufen
description: Rufen Sie Aktivitäten für einen bestimmten Benutzer. Aktivitäten ohne gespeichert werden soll, im Gegensatz zu der **letzte** OData-Funktion zurückgegeben. Die Berechtigung UserActivity.ReadWrite.CreatedByApp gelten zusätzliche Filter auf die Antwort, damit nur Aktivitäten, die von der Anwendung erstellt zurückgegeben werden. Diese serverseitige Filterung auftreten auf leere Seiten, wenn der Benutzer besonders aktiv ist und anderen Applikationen neuere Aktivitäten erstellt haben. Wenn Sie Ihre Anwendung Aktivitäten erhalten möchten, verwenden Sie die **NextLink** -Eigenschaft für die Paginierung.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: dce6420e33a5d57eb78d8ea4842ed759ebcdd11c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971795"
---
# <a name="get-user-activities"></a><span data-ttu-id="68a36-107">Die Benutzeraktivitäten abrufen</span><span class="sxs-lookup"><span data-stu-id="68a36-107">Get user activities</span></span>

<span data-ttu-id="68a36-108">Rufen Sie Aktivitäten für einen bestimmten Benutzer.</span><span class="sxs-lookup"><span data-stu-id="68a36-108">Get activities for a given user.</span></span> <span data-ttu-id="68a36-109">Aktivitäten ohne gespeichert werden soll, im Gegensatz zu der **letzte** OData-Funktion zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="68a36-109">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="68a36-110">Die Berechtigung UserActivity.ReadWrite.CreatedByApp gelten zusätzliche Filter auf die Antwort, damit nur Aktivitäten, die von der Anwendung erstellt zurückgegeben werden.</span><span class="sxs-lookup"><span data-stu-id="68a36-110">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="68a36-111">Diese serverseitige Filterung auftreten auf leere Seiten, wenn der Benutzer besonders aktiv ist und anderen Applikationen neuere Aktivitäten erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="68a36-111">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="68a36-112">Wenn Sie Ihre Anwendung Aktivitäten erhalten möchten, verwenden Sie die **NextLink** -Eigenschaft für die Paginierung.</span><span class="sxs-lookup"><span data-stu-id="68a36-112">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="68a36-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="68a36-113">Permissions</span></span>

<span data-ttu-id="68a36-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68a36-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68a36-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="68a36-116">Permission type</span></span>      | <span data-ttu-id="68a36-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="68a36-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68a36-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="68a36-118">Delegated (work or school account)</span></span> | <span data-ttu-id="68a36-119">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="68a36-119">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="68a36-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="68a36-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68a36-121">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="68a36-121">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="68a36-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="68a36-122">Application</span></span> | <span data-ttu-id="68a36-123">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="68a36-123">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="68a36-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="68a36-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68a36-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="68a36-125">Optional query parameters</span></span>

<span data-ttu-id="68a36-126">Diese Methode unterstützt einige [OData-Abfrage-Parameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="68a36-126">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="68a36-127">Die folgenden Abfrageparameter werden unterstützt:</span><span class="sxs-lookup"><span data-stu-id="68a36-127">The following query parameters are supported:</span></span>

- <span data-ttu-id="68a36-128">$ Erweitern Sie für die Eigenschaft **HistoryItems** Navigation.</span><span class="sxs-lookup"><span data-stu-id="68a36-128">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="68a36-129">$top um die maximale Anzahl von Elementen auf mehreren Seiten zu begrenzen.</span><span class="sxs-lookup"><span data-stu-id="68a36-129">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="68a36-130">$filter auf die **LastModifiedDateTime** -Eigenschaft für Aktivitäten oder **HistoryItems**, wenn erweitert.</span><span class="sxs-lookup"><span data-stu-id="68a36-130">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="68a36-131">Es folgen einige Beispiele für unterstützte Abfragen mit URL-Codierung:</span><span class="sxs-lookup"><span data-stu-id="68a36-131">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="68a36-132">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="68a36-132">Request headers</span></span>

|<span data-ttu-id="68a36-133">Name</span><span class="sxs-lookup"><span data-stu-id="68a36-133">Name</span></span> | <span data-ttu-id="68a36-134">Typ</span><span class="sxs-lookup"><span data-stu-id="68a36-134">Type</span></span> | <span data-ttu-id="68a36-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="68a36-135">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="68a36-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="68a36-136">Authorization</span></span> | <span data-ttu-id="68a36-137">string</span><span class="sxs-lookup"><span data-stu-id="68a36-137">string</span></span> | <span data-ttu-id="68a36-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="68a36-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="68a36-140">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="68a36-140">Request body</span></span>

<span data-ttu-id="68a36-141">Keine Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="68a36-141">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="68a36-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="68a36-142">Response</span></span>

<span data-ttu-id="68a36-143">Wenn der Vorgang erfolgreich war, gibt diese Methode die `200 OK` Antwortcode mit die Aktivitäten des Benutzers für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="68a36-143">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="68a36-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="68a36-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="68a36-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="68a36-145">Request</span></span>

<span data-ttu-id="68a36-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="68a36-146">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="68a36-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="68a36-147">Response</span></span>

<span data-ttu-id="68a36-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="68a36-148">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.userActivity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
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
