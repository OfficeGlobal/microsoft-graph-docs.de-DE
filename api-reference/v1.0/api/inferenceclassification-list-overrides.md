---
title: Außerkraftsetzungen auflisten
description: Dient zum Abrufen der Außerkraftsetzungen, die ein Benutzer eingerichtet hat, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren.
ms.openlocfilehash: 7953c776b60f4e63aec03245817bfcf6630bbdf8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016312"
---
# <a name="list-overrides"></a><span data-ttu-id="bb561-103">Außerkraftsetzungen auflisten</span><span class="sxs-lookup"><span data-stu-id="bb561-103">List overrides</span></span>

<span data-ttu-id="bb561-104">Dient zum Abrufen der Außerkraftsetzungen, die ein Benutzer eingerichtet hat, um Nachrichten von bestimmten Absendern immer auf eine bestimmte Art und Weise zu klassifizieren.</span><span class="sxs-lookup"><span data-stu-id="bb561-104">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="bb561-p101">Jede Außerkraftsetzung entspricht einer SMTP-Adresse eines Absenders. Zu Beginn hat ein Benutzer keine Außerkraftsetzungen.</span><span class="sxs-lookup"><span data-stu-id="bb561-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="bb561-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bb561-107">Permissions</span></span>
<span data-ttu-id="bb561-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb561-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb561-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bb561-110">Permission type</span></span>      | <span data-ttu-id="bb561-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bb561-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb561-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bb561-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bb561-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bb561-113">Mail.Read</span></span>    |
|<span data-ttu-id="bb561-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bb561-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb561-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bb561-115">Mail.Read</span></span>    |
|<span data-ttu-id="bb561-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bb561-116">Application</span></span> | <span data-ttu-id="bb561-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="bb561-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb561-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb561-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="bb561-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bb561-119">Request headers</span></span>
| <span data-ttu-id="bb561-120">Name</span><span class="sxs-lookup"><span data-stu-id="bb561-120">Name</span></span>       | <span data-ttu-id="bb561-121">Typ</span><span class="sxs-lookup"><span data-stu-id="bb561-121">Type</span></span> | <span data-ttu-id="bb561-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bb561-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bb561-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb561-123">Authorization</span></span>  | <span data-ttu-id="bb561-124">string</span><span class="sxs-lookup"><span data-stu-id="bb561-124">string</span></span>  | <span data-ttu-id="bb561-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bb561-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb561-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bb561-127">Request body</span></span>
<span data-ttu-id="bb561-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bb561-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb561-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb561-129">Response</span></span>

<span data-ttu-id="bb561-p104">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekten im Antworttext zurückgegeben. Wenn der Benutzer keine Außerkraftsetzungen eingerichtet hat, wird eine leere Sammlung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb561-p104">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body. An empty collection is returned if the user doesn't have any overrides set up.</span></span>
## <a name="example"></a><span data-ttu-id="bb561-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bb561-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb561-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb561-133">Request</span></span>
<span data-ttu-id="bb561-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bb561-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="bb561-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb561-135">Response</span></span>
<span data-ttu-id="bb561-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb561-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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