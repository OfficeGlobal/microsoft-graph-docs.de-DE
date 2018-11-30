---
title: Aktivität erstellen oder ersetzen
description: Erstellen Sie ein neues, oder Ersetzen Sie eine vorhandene Benutzeraktivität für Ihre app. Wenn Sie eine Benutzeraktivität und die zugehörigen **HistoryItems** in einer Anforderung erstellen möchten, können Sie die Tiefe einfügen.
ms.openlocfilehash: 1a749f0c4303551ab9915c89d84e6757c61bd0a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062874"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="cddd6-104">Aktivität erstellen oder ersetzen</span><span class="sxs-lookup"><span data-stu-id="cddd6-104">Create or replace an activity</span></span>

> <span data-ttu-id="cddd6-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cddd6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cddd6-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cddd6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cddd6-107">Erstellen Sie ein neues, oder Ersetzen Sie eine vorhandene Benutzeraktivität für Ihre app.</span><span class="sxs-lookup"><span data-stu-id="cddd6-107">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="cddd6-108">Wenn Sie eine Benutzeraktivität und die zugehörigen **HistoryItems** in einer Anforderung erstellen möchten, können Sie [intensive einfügen](projectrome-put-activity.md#example-2---deep-insert).</span><span class="sxs-lookup"><span data-stu-id="cddd6-108">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome-put-activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="cddd6-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cddd6-109">Permissions</span></span>

<span data-ttu-id="cddd6-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cddd6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cddd6-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cddd6-112">Permission type</span></span>      | <span data-ttu-id="cddd6-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cddd6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cddd6-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cddd6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cddd6-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="cddd6-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="cddd6-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cddd6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cddd6-117">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="cddd6-117">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="cddd6-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cddd6-118">Application</span></span> | <span data-ttu-id="cddd6-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cddd6-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cddd6-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cddd6-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="cddd6-121">**Hinweis:** Die AppActivityId in der URL muss URL-sichere (alle Zeichen mit Ausnahme der RFC 2396 nicht reservierte Zeichen in ihre hexadezimale Darstellung konvertiert werden müssen) sein, aber die ursprünglichen AppActivityId benötigt keinen URL-sicheren.</span><span class="sxs-lookup"><span data-stu-id="cddd6-121">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cddd6-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cddd6-122">Request headers</span></span>

|<span data-ttu-id="cddd6-123">Name</span><span class="sxs-lookup"><span data-stu-id="cddd6-123">Name</span></span> | <span data-ttu-id="cddd6-124">Typ</span><span class="sxs-lookup"><span data-stu-id="cddd6-124">Type</span></span> | <span data-ttu-id="cddd6-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cddd6-125">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="cddd6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="cddd6-126">Authorization</span></span> | <span data-ttu-id="cddd6-127">string</span><span class="sxs-lookup"><span data-stu-id="cddd6-127">string</span></span> | <span data-ttu-id="cddd6-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cddd6-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cddd6-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cddd6-130">Request body</span></span>

<span data-ttu-id="cddd6-131">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines Objekts [Aktivität](../resources/projectrome-activity.md) aus.</span><span class="sxs-lookup"><span data-stu-id="cddd6-131">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cddd6-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="cddd6-132">Response</span></span>

<span data-ttu-id="cddd6-133">Wenn der Vorgang erfolgreich war, gibt diese Methode die `201 Created` Antwortcode, wenn die Aktivität erstellt wurde oder `200 OK` , wenn die Aktivität ersetzt wurde.</span><span class="sxs-lookup"><span data-stu-id="cddd6-133">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="cddd6-134">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="cddd6-134">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="cddd6-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cddd6-135">Request</span></span>

<span data-ttu-id="cddd6-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cddd6-136">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/%2Farticle%3F12345
Content-type: application/json
Content-length: 364

{
    "appActivityId": "/article?12345",
    "activitySourceHost": "https://www.contoso.com",
    "userTimezone": "Africa/Casablanca",
    "appDisplayName": "Contoso, Ltd.",
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": "false"
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "content": {
            "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="cddd6-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="cddd6-137">Response</span></span>

<span data-ttu-id="cddd6-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cddd6-138">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/beta/me/activities/14332800362997268276

{
    "activitySourceHost": "https://contoso.com",
    "createdDateTime": "2017-06-09T20:54:43.969Z",
    "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
    "id": "14332800362997268276",
    "appActivityId": "/article?12345",
    "status":"updated",
    "expirationDateTime": "2017-02-26T20:20:48.114Z",
    "id": "14332800362997268276",
    "visualElements": {
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
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
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
}
```

## <a name="example-2---deep-insert"></a><span data-ttu-id="cddd6-139">Beispiel 2 – Tiefe einfügen</span><span class="sxs-lookup"><span data-stu-id="cddd6-139">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="cddd6-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cddd6-140">Request</span></span>

<span data-ttu-id="cddd6-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cddd6-141">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/%2Farticle%3F12345
Content-type: application/json
Content-length: 364

{
    "appActivityId": "/article?12345",
    "activitySourceHost": "https://www.contoso.com",
    "userTimezone": "Africa/Casablanca",
    "appDisplayName": "Contoso, Ltd.",
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": "false",
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
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
    "historyItems":[
        {
            "userTimezone": "Africa/Casablanca",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="cddd6-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="cddd6-142">Response</span></span>

<span data-ttu-id="cddd6-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cddd6-143">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/beta/me/activities/14332800362997268276

{
    "activitySourceHost": "https://contoso.com",
    "createdDateTime": "2017-06-09T20:54:43.969Z",
    "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
    "id": "14332800362997268276",
    "appActivityId": "/article?12345",
    "status":"updated",
    "expirationDateTime": "2017-02-26T20:20:48.114Z",
    "id": "14332800362997268276",
    "visualElements": {
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
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
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "historyItems":[
        {
            "status": "updated",
            "userTimezone": "Africa/Casablanca",
            "createdDateTime": "2018-04-12T21:42:42.495Z",
            "lastModifiedDateTime": "2018-04-12T21:42:42.495Z",
            "id": "61fc8f36-919f-4b73-89d4-1cb7b159d912",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
            "expirationDateTime": "2018-05-12T21:42:42.495Z",
            "activeDurationSeconds": 20
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
