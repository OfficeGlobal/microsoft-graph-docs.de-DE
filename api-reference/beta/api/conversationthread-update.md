---
title: conversationThread aktualisieren
description: Mit dieser API können Sie Threads sperren oder entsperren und so steuern, ob weiterhin in ihnen gepostet werden darf.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 99ed0a7c635fc02bd0b0c6ea485e18a5875d8fe2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985081"
---
# <a name="update-conversationthread"></a><span data-ttu-id="6110b-103">conversationThread aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6110b-103">Update conversationthread</span></span>

> <span data-ttu-id="6110b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6110b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6110b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6110b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6110b-106">Mit dieser API können Sie Threads sperren oder entsperren und so steuern, ob weiterhin in ihnen gepostet werden darf.</span><span class="sxs-lookup"><span data-stu-id="6110b-106">Lock or unlock a thread, to allow or avoid further posting to the thread.</span></span>
## <a name="permissions"></a><span data-ttu-id="6110b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6110b-107">Permissions</span></span>
<span data-ttu-id="6110b-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6110b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6110b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6110b-110">Permission type</span></span>      | <span data-ttu-id="6110b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6110b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6110b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6110b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6110b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6110b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6110b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6110b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6110b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6110b-115">Not supported.</span></span>    |
|<span data-ttu-id="6110b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6110b-116">Application</span></span> | <span data-ttu-id="6110b-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6110b-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6110b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6110b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /groups/{id}/threads/{id}
PATCH /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="6110b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6110b-119">Request headers</span></span>
| <span data-ttu-id="6110b-120">Header</span><span class="sxs-lookup"><span data-stu-id="6110b-120">Header</span></span>       | <span data-ttu-id="6110b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="6110b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6110b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6110b-122">Authorization</span></span>  | <span data-ttu-id="6110b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6110b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6110b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6110b-125">Content-Type</span></span>  | <span data-ttu-id="6110b-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="6110b-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6110b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6110b-128">Request body</span></span>
<span data-ttu-id="6110b-p105">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="6110b-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6110b-132">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6110b-132">Property</span></span>     | <span data-ttu-id="6110b-133">Typ</span><span class="sxs-lookup"><span data-stu-id="6110b-133">Type</span></span>   |<span data-ttu-id="6110b-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6110b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6110b-135">isLocked</span><span class="sxs-lookup"><span data-stu-id="6110b-135">isLocked</span></span>|<span data-ttu-id="6110b-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="6110b-136">Boolean</span></span>|<span data-ttu-id="6110b-p106">Zeigt an, ob der Thread gesperrt ist. Mit `true` werden Beiträge verhindert.</span><span class="sxs-lookup"><span data-stu-id="6110b-p106">Indicates if the thread is locked. Set to `true` to disallow posting.</span></span>|

## <a name="response"></a><span data-ttu-id="6110b-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6110b-139">Response</span></span>

<span data-ttu-id="6110b-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das aktualisierte [conversationThread](../resources/conversationthread.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6110b-140">If successful, this method returns a `200 OK` response code and updated [conversationThread](../resources/conversationthread.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6110b-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6110b-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6110b-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6110b-142">Request</span></span>
<span data-ttu-id="6110b-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6110b-143">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6110b-144">Antwort</span><span class="sxs-lookup"><span data-stu-id="6110b-144">Response</span></span>
<span data-ttu-id="6110b-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6110b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update conversationthread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
