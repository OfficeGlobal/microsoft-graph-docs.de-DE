---
title: Außerkraftsetzungen auflisten
description: Rufen Sie die Experten Posteingang überschreibt, die ein Benutzer zum Klassifizieren von Nachrichten von bestimmten Absendern immer auf bestimmte Weise eingerichtet hat.
localization_priority: Normal
ms.openlocfilehash: a49d47e39caff5c00981d02551b0eeb564239f73
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511919"
---
# <a name="list-overrides"></a><span data-ttu-id="3a79e-103">Außerkraftsetzungen auflisten</span><span class="sxs-lookup"><span data-stu-id="3a79e-103">List overrides</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a79e-104">Rufen Sie die [Experten Posteingang](../resources/manage-focused-inbox.md) überschreibt, die ein Benutzer zum Klassifizieren von Nachrichten von bestimmten Absendern immer auf bestimmte Weise eingerichtet hat.</span><span class="sxs-lookup"><span data-stu-id="3a79e-104">Get the [Focused Inbox](../resources/manage-focused-inbox.md) overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>

<span data-ttu-id="3a79e-p101">Jede Außerkraftsetzung entspricht einer SMTP-Adresse eines Absenders. Zu Beginn hat ein Benutzer keine Außerkraftsetzungen.</span><span class="sxs-lookup"><span data-stu-id="3a79e-p101">Each override corresponds to an SMTP address of a sender. Initially, a user does not have any overrides.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a79e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3a79e-107">Permissions</span></span>
<span data-ttu-id="3a79e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a79e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a79e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a79e-110">Permission type</span></span>      | <span data-ttu-id="3a79e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a79e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a79e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a79e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3a79e-113">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3a79e-113">Mail.Read</span></span>    |
|<span data-ttu-id="3a79e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a79e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a79e-115">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3a79e-115">Mail.Read</span></span>    |
|<span data-ttu-id="3a79e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a79e-116">Application</span></span> | <span data-ttu-id="3a79e-117">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="3a79e-117">Mail.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a79e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a79e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/inferenceClassification/overrides
GET /users/{id}/inferenceClassification/overrides
```

## <a name="request-headers"></a><span data-ttu-id="3a79e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a79e-119">Request headers</span></span>
| <span data-ttu-id="3a79e-120">Name</span><span class="sxs-lookup"><span data-stu-id="3a79e-120">Name</span></span>       | <span data-ttu-id="3a79e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="3a79e-121">Type</span></span> | <span data-ttu-id="3a79e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a79e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3a79e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a79e-123">Authorization</span></span>  | <span data-ttu-id="3a79e-124">string</span><span class="sxs-lookup"><span data-stu-id="3a79e-124">string</span></span>  | <span data-ttu-id="3a79e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a79e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a79e-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a79e-127">Request body</span></span>
<span data-ttu-id="3a79e-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3a79e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3a79e-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a79e-129">Response</span></span>

<span data-ttu-id="3a79e-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Objekten im Antworttext [InferenceClassificationOverride](../resources/inferenceclassificationoverride.md) .</span><span class="sxs-lookup"><span data-stu-id="3a79e-130">If successful, this method returns a `200 OK` response code and a collection of [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3a79e-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a79e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a79e-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a79e-132">Request</span></span>
<span data-ttu-id="3a79e-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a79e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_overrides"
}-->
```http
GET https://graph.microsoft.com/beta/me/inferenceClassification/overrides
```
##### <a name="response"></a><span data-ttu-id="3a79e-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a79e-134">Response</span></span>
<span data-ttu-id="3a79e-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a79e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List overrides",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/inferenceclassification-list-overrides.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
