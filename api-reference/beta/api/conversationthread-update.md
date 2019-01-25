---
title: conversationThread aktualisieren
description: Mit dieser API können Sie Threads sperren oder entsperren und so steuern, ob weiterhin in ihnen gepostet werden darf.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 2127b85b048a3c62baeabfae34eaa3806979cee8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516070"
---
# <a name="update-conversationthread"></a><span data-ttu-id="1ee93-103">conversationThread aktualisieren</span><span class="sxs-lookup"><span data-stu-id="1ee93-103">Update conversationthread</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ee93-104">Mit dieser API können Sie Threads sperren oder entsperren und so steuern, ob weiterhin in ihnen gepostet werden darf.</span><span class="sxs-lookup"><span data-stu-id="1ee93-104">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="1ee93-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1ee93-105">Permissions</span></span>
<span data-ttu-id="1ee93-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ee93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ee93-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1ee93-108">Permission type</span></span>      | <span data-ttu-id="1ee93-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1ee93-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ee93-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1ee93-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1ee93-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee93-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1ee93-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1ee93-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ee93-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1ee93-113">Not supported.</span></span>    |
|<span data-ttu-id="1ee93-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1ee93-114">Application</span></span> | <span data-ttu-id="1ee93-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ee93-115">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ee93-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ee93-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1ee93-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1ee93-117">Request headers</span></span>
| <span data-ttu-id="1ee93-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1ee93-118">Header</span></span>       | <span data-ttu-id="1ee93-119">Wert</span><span class="sxs-lookup"><span data-stu-id="1ee93-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1ee93-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ee93-120">Authorization</span></span>  | <span data-ttu-id="1ee93-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1ee93-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1ee93-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ee93-123">Content-Type</span></span>  | <span data-ttu-id="1ee93-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="1ee93-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1ee93-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1ee93-126">Request body</span></span>
<span data-ttu-id="1ee93-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="1ee93-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="1ee93-130">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1ee93-130">Property</span></span>     | <span data-ttu-id="1ee93-131">Typ</span><span class="sxs-lookup"><span data-stu-id="1ee93-131">Type</span></span>   |<span data-ttu-id="1ee93-132">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1ee93-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ee93-133">isLocked</span><span class="sxs-lookup"><span data-stu-id="1ee93-133">isLocked</span></span>|<span data-ttu-id="1ee93-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ee93-134">Boolean</span></span>|<span data-ttu-id="1ee93-p105">Zeigt an, ob der Thread gesperrt ist. Mit `true` werden Beiträge verhindert.</span><span class="sxs-lookup"><span data-stu-id="1ee93-p105">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="1ee93-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ee93-137">Response</span></span>

<span data-ttu-id="1ee93-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ee93-138">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ee93-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1ee93-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ee93-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1ee93-140">Request</span></span>
<span data-ttu-id="1ee93-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1ee93-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_conversationthread"
}-->
```http
PATCH https://graph.microsoft.com/beta/groups/{id}/threads/{id}
Content-type: application/json
Content-length: 419

{
  "@odata.type":"#Microsoft.OutlookServices.ConversationThread",
  "isLocked": true
}
```
##### <a name="response"></a><span data-ttu-id="1ee93-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="1ee93-142">Response</span></span>
<span data-ttu-id="1ee93-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1ee93-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 419

{
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "topic": "topic-value",
  "hasAttachments": true,
  "lastDeliveredDateTime": "2016-10-19T10:37:00Z",
  "uniqueSenders": [
    "uniqueSenders-value"
  ],
  "ccRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ],
  "isLocked": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationthread-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
