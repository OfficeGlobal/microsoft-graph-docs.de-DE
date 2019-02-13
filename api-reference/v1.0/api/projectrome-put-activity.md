---
title: Aktivität erstellen oder ersetzen
description: Erstellen Sie ein neues, oder Ersetzen Sie eine vorhandene Benutzeraktivität für Ihre app. Wenn Sie eine Benutzeraktivität und die zugehörigen **HistoryItems** in einer Anforderung erstellen möchten, können Sie die Tiefe einfügen.
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 3f0864d5bdd8e393a21df49ec3fade6930fdcbde
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967284"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="f8de0-104">Aktivität erstellen oder ersetzen</span><span class="sxs-lookup"><span data-stu-id="f8de0-104">Create or replace an activity</span></span>

<span data-ttu-id="f8de0-105">Erstellen Sie ein neues, oder Ersetzen Sie eine vorhandene Benutzeraktivität für Ihre app.</span><span class="sxs-lookup"><span data-stu-id="f8de0-105">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="f8de0-106">Wenn Sie eine Benutzeraktivität und die zugehörigen **HistoryItems** in einer Anforderung erstellen möchten, können Sie [intensive einfügen](#example-2-deep-insert).</span><span class="sxs-lookup"><span data-stu-id="f8de0-106">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](#example-2-deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="f8de0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f8de0-107">Permissions</span></span>

<span data-ttu-id="f8de0-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8de0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f8de0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8de0-110">Permission type</span></span>                        | <span data-ttu-id="f8de0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8de0-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="f8de0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8de0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f8de0-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f8de0-113">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="f8de0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8de0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8de0-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f8de0-115">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="f8de0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8de0-116">Application</span></span>                            | <span data-ttu-id="f8de0-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="f8de0-117">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="f8de0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8de0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

> <span data-ttu-id="f8de0-119">**Hinweis:** Die AppActivityId in der URL muss URL-sichere (alle Zeichen mit Ausnahme der RFC 2396 nicht reservierte Zeichen in ihre hexadezimale Darstellung konvertiert werden müssen) sein, aber die ursprünglichen AppActivityId benötigt keinen URL-sicheren.</span><span class="sxs-lookup"><span data-stu-id="f8de0-119">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f8de0-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8de0-120">Request headers</span></span>

| <span data-ttu-id="f8de0-121">Name</span><span class="sxs-lookup"><span data-stu-id="f8de0-121">Name</span></span>          | <span data-ttu-id="f8de0-122">Typ</span><span class="sxs-lookup"><span data-stu-id="f8de0-122">Type</span></span>   | <span data-ttu-id="f8de0-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f8de0-123">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="f8de0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8de0-124">Authorization</span></span> | <span data-ttu-id="f8de0-125">string</span><span class="sxs-lookup"><span data-stu-id="f8de0-125">string</span></span> | <span data-ttu-id="f8de0-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f8de0-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8de0-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8de0-128">Request body</span></span>

<span data-ttu-id="f8de0-129">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines Objekts [Aktivität](../resources/projectrome-activity.md) aus.</span><span class="sxs-lookup"><span data-stu-id="f8de0-129">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f8de0-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8de0-130">Response</span></span>

<span data-ttu-id="f8de0-131">Wenn der Vorgang erfolgreich war, gibt diese Methode die `201 Created` Antwortcode, wenn die Aktivität erstellt wurde oder `200 OK` , wenn die Aktivität ersetzt wurde.</span><span class="sxs-lookup"><span data-stu-id="f8de0-131">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="examples"></a><span data-ttu-id="f8de0-132">Beispiele</span><span class="sxs-lookup"><span data-stu-id="f8de0-132">Examples</span></span>

### <a name="example-1-create-an-activity"></a><span data-ttu-id="f8de0-133">In Beispiel 1: Erstellen einer Aktivitätsfeeds</span><span class="sxs-lookup"><span data-stu-id="f8de0-133">Example 1: Create an activity</span></span>

#### <a name="request"></a><span data-ttu-id="f8de0-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8de0-134">Request</span></span>

<span data-ttu-id="f8de0-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8de0-135">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json

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
      "addImageQuery": false
    },
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "backgroundColor": "#ff0000",
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="f8de0-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8de0-136">Response</span></span>

<span data-ttu-id="f8de0-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f8de0-137">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "activitySourceHost": "https://contoso.com",
  "createdDateTime": "2017-06-09T20:54:43.969Z",
  "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
  "id": "14332800362997268276",
  "appActivityId": "/article?12345",
  "status": "updated",
  "expirationDateTime": "2017-02-26T20:20:48.114Z",
  "visualElements": {
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "backgroundColor": "#ff0000",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
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
  }
}
```

### <a name="example-2-deep-insert"></a><span data-ttu-id="f8de0-138">Beispiel 2: Tiefe einfügen</span><span class="sxs-lookup"><span data-stu-id="f8de0-138">Example 2: Deep insert</span></span>

<span data-ttu-id="f8de0-139">Dieses Beispiel erstellt eine neue Aktivität und Historienelement für diese Aktivität in einer Anforderung an.</span><span class="sxs-lookup"><span data-stu-id="f8de0-139">This example creates a new activity and a history item for that activity in one request.</span></span>

#### <a name="request"></a><span data-ttu-id="f8de0-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8de0-140">Request</span></span>

<span data-ttu-id="f8de0-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8de0-141">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json

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
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  },
  "historyItems": [
    {
      "userTimezone": "Africa/Casablanca",
      "startedDateTime": "2018-02-26T20:54:04.345Z",
      "lastActiveDateTime": "2018-02-26T20:54:24.345Z"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="f8de0-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8de0-142">Response</span></span>

<span data-ttu-id="f8de0-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f8de0-143">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "activitySourceHost": "https://contoso.com",
  "createdDateTime": "2017-06-09T20:54:43.969Z",
  "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
  "id": "14332800362997268276",
  "appActivityId": "/article?12345",
  "status": "updated",
  "expirationDateTime": "2017-02-26T20:20:48.114Z",
  "visualElements": {
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "backgroundColor": "#ff0000",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
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
  "historyItems": [
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
