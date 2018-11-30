---
title: Außerkraftsetzungen auflisten
description: Rufen Sie die Experten Posteingang überschreibt, die ein Benutzer zum Klassifizieren von Nachrichten von bestimmten Absendern immer auf bestimmte Weise eingerichtet hat.
ms.openlocfilehash: 343faaacf47d16b723cd8aebc25a6df79ef7e3db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065416"
---
# <a name="list-overrides"></a><span data-ttu-id="b85b7-103">Außerkraftsetzungen auflisten</span><span class="sxs-lookup"><span data-stu-id="b85b7-103">List overrides</span></span>

> <span data-ttu-id="b85b7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b85b7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b85b7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b85b7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b85b7-106">Rufen Sie die [Experten Posteingang](../resources/manage-focused-inbox.md) überschreibt, die ein Benutzer zum Klassifizieren von Nachrichten von bestimmten Absendern immer auf bestimmte Weise eingerichtet hat.</span><span class="sxs-lookup"><span data-stu-id="b85b7-106">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="b85b7-p102">Jede Außerkraftsetzung entspricht einer SMTP-Adresse eines Absenders. Zu Beginn hat ein Benutzer keine Außerkraftsetzungen.</span><span class="sxs-lookup"><span data-stu-id="b85b7-p102">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="b85b7-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b85b7-109">Permissions</span></span>
<span data-ttu-id="b85b7-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b85b7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b85b7-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b85b7-112">Permission type</span></span>      | <span data-ttu-id="b85b7-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b85b7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b85b7-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b85b7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b85b7-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b85b7-115">Mail.Read</span></span>    |
|<span data-ttu-id="b85b7-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b85b7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b85b7-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b85b7-117">Mail.Read</span></span>    |
|<span data-ttu-id="b85b7-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b85b7-118">Application</span></span> | <span data-ttu-id="b85b7-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="b85b7-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="b85b7-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b85b7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="b85b7-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b85b7-121">Request headers</span></span>
| <span data-ttu-id="b85b7-122">Name</span><span class="sxs-lookup"><span data-stu-id="b85b7-122">Name</span></span>       | <span data-ttu-id="b85b7-123">Typ</span><span class="sxs-lookup"><span data-stu-id="b85b7-123">Type</span></span> | <span data-ttu-id="b85b7-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b85b7-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b85b7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b85b7-125">Authorization</span></span>  | <span data-ttu-id="b85b7-126">string</span><span class="sxs-lookup"><span data-stu-id="b85b7-126">string</span></span>  | <span data-ttu-id="b85b7-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b85b7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b85b7-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b85b7-129">Request body</span></span>
<span data-ttu-id="b85b7-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b85b7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b85b7-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="b85b7-131">Response</span></span>

<span data-ttu-id="b85b7-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [InferenceClassificationOverride](../resources/inferenceclassificationoverride.md) .</span><span class="sxs-lookup"><span data-stu-id="b85b7-132">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b85b7-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b85b7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b85b7-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b85b7-134">Request</span></span>
<span data-ttu-id="b85b7-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b85b7-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="b85b7-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b85b7-136">Response</span></span>
<span data-ttu-id="b85b7-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b85b7-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "classifyAs": "focused",
      "senderEmailAddress": {
        "name": "Samantha Booth",
        "address": "samanthab@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf11a9b9"
    },
    {
      "classifyAs": "other",
      "senderEmailAddress": {
        "name": "Randi Welch",
        "address": "randiw@adatum.onmicrosoft.com"
      },
      "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->