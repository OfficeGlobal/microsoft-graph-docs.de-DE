---
title: Anlage hinzufügen
description: Verwenden Sie diese API, um eine neue Anlage zu erstellen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 504b3daccc5e1313ee56d23a87b2d25eb62abae9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522665"
---
# <a name="add-attachment"></a><span data-ttu-id="02644-103">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="02644-103">Add attachment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02644-104">Verwenden Sie diese API, um eine neue Anlage zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="02644-104">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="02644-105">Eine Anlage weist einen der folgenden Typen auf:</span><span class="sxs-lookup"><span data-stu-id="02644-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="02644-106">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="02644-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="02644-107">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="02644-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="02644-108">Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="02644-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="02644-109">All diese Typen von Anlagenressourcen werden von der Ressource [attachment](../resources/attachment.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="02644-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="02644-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="02644-110">Permissions</span></span>
<span data-ttu-id="02644-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02644-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02644-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="02644-113">Permission type</span></span>      | <span data-ttu-id="02644-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="02644-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02644-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="02644-115">Delegated (work or school account)</span></span> | <span data-ttu-id="02644-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02644-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="02644-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="02644-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02644-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02644-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="02644-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="02644-119">Application</span></span> | <span data-ttu-id="02644-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="02644-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="02644-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="02644-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="02644-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="02644-122">Request headers</span></span>
| <span data-ttu-id="02644-123">Name</span><span class="sxs-lookup"><span data-stu-id="02644-123">Name</span></span>       | <span data-ttu-id="02644-124">Typ</span><span class="sxs-lookup"><span data-stu-id="02644-124">Type</span></span> | <span data-ttu-id="02644-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="02644-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="02644-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="02644-126">Authorization</span></span>  | <span data-ttu-id="02644-127">string</span><span class="sxs-lookup"><span data-stu-id="02644-127">string</span></span>  | <span data-ttu-id="02644-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="02644-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="02644-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="02644-130">Content-Type</span></span> | <span data-ttu-id="02644-131">string</span><span class="sxs-lookup"><span data-stu-id="02644-131">string</span></span>  | <span data-ttu-id="02644-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="02644-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02644-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="02644-134">Request body</span></span>
<span data-ttu-id="02644-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="02644-135">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="02644-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="02644-136">Response</span></span>

<span data-ttu-id="02644-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [Attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02644-137">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="02644-138">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="02644-138">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="02644-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02644-139">Request</span></span>
<span data-ttu-id="02644-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="02644-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "contentBytes-value"
}
```

##### <a name="response"></a><span data-ttu-id="02644-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="02644-141">Response</span></span>
<span data-ttu-id="02644-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02644-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="02644-145">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="02644-145">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="02644-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="02644-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="02644-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="02644-147">Response</span></span>
<span data-ttu-id="02644-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="02644-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/eventmessage-post-attachments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
