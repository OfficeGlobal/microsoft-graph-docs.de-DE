---
title: Außerkraftsetzungen auflisten
description: Rufen Sie die Experten Posteingang überschreibt, die ein Benutzer zum Klassifizieren von Nachrichten von bestimmten Absendern immer auf bestimmte Weise eingerichtet hat.
localization_priority: Normal
ms.openlocfilehash: 6d2d731858ad3a87cad10b4feb23378cb4dab992
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837555"
---
# <a name="list-overrides"></a><span data-ttu-id="f789d-103">Außerkraftsetzungen auflisten</span><span class="sxs-lookup"><span data-stu-id="f789d-103">List overrides</span></span>

> <span data-ttu-id="f789d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f789d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f789d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f789d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f789d-106">Rufen Sie die [Experten Posteingang](../resources/manage-focused-inbox.md) überschreibt, die ein Benutzer zum Klassifizieren von Nachrichten von bestimmten Absendern immer auf bestimmte Weise eingerichtet hat.</span><span class="sxs-lookup"><span data-stu-id="f789d-106">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="f789d-p102">Jede Außerkraftsetzung entspricht einer SMTP-Adresse eines Absenders. Zu Beginn hat ein Benutzer keine Außerkraftsetzungen.</span><span class="sxs-lookup"><span data-stu-id="f789d-p102">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="f789d-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f789d-109">Permissions</span></span>
<span data-ttu-id="f789d-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f789d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f789d-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f789d-112">Permission type</span></span>      | <span data-ttu-id="f789d-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f789d-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f789d-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f789d-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f789d-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f789d-115">Mail.Read</span></span>    |
|<span data-ttu-id="f789d-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f789d-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f789d-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f789d-117">Mail.Read</span></span>    |
|<span data-ttu-id="f789d-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f789d-118">Application</span></span> | <span data-ttu-id="f789d-119">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="f789d-119">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f789d-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f789d-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="f789d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f789d-121">Request headers</span></span>
| <span data-ttu-id="f789d-122">Name</span><span class="sxs-lookup"><span data-stu-id="f789d-122">Name</span></span>       | <span data-ttu-id="f789d-123">Typ</span><span class="sxs-lookup"><span data-stu-id="f789d-123">Type</span></span> | <span data-ttu-id="f789d-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f789d-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f789d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f789d-125">Authorization</span></span>  | <span data-ttu-id="f789d-126">string</span><span class="sxs-lookup"><span data-stu-id="f789d-126">string</span></span>  | <span data-ttu-id="f789d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f789d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f789d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f789d-129">Request body</span></span>
<span data-ttu-id="f789d-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f789d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f789d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="f789d-131">Response</span></span>

<span data-ttu-id="f789d-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [InferenceClassificationOverride](../resources/inferenceclassificationoverride.md) .</span><span class="sxs-lookup"><span data-stu-id="f789d-132">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f789d-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f789d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f789d-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f789d-134">Request</span></span>
<span data-ttu-id="f789d-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f789d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="f789d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="f789d-136">Response</span></span>
<span data-ttu-id="f789d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f789d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
