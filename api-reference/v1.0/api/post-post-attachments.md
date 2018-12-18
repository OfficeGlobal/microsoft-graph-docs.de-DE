---
title: Anlage hinzufügen
description: Verwenden Sie diese API, um eine Anlage auf einen Beitrag hinzuzufügen. Seit dort
author: dkershaw10
ms.openlocfilehash: 15db2de825bf8f0b8fdc68094672f4f4fc7a9ae5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346487"
---
# <a name="add-attachment"></a><span data-ttu-id="25a65-104">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="25a65-104">Add attachment</span></span>

<span data-ttu-id="25a65-p102">Verwenden Sie diese API zum Hinzufügen einer [Anlage](../resources/attachment.md) zu einem Beitrag. Da es derzeit eine Beschränkung von 4 MB für die Gesamtgröße jeder REST-Anforderung gibt, wird hierdurch die Größe der Anlage, die Sie hinzufügen können, auf unter 4 MB beschränkt.</span><span class="sxs-lookup"><span data-stu-id="25a65-p102">Use this API to add an [attachment](../resources/attachment.md) to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB.</span></span>

<span data-ttu-id="25a65-107">Eine Anlage weist einen der folgenden Typen auf:</span><span class="sxs-lookup"><span data-stu-id="25a65-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="25a65-108">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="25a65-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="25a65-109">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="25a65-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="25a65-110">Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="25a65-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="25a65-111">All diese Typen von Anlagenressourcen werden von der Ressource [attachment](../resources/attachment.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="25a65-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="25a65-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="25a65-112">Permissions</span></span>
<span data-ttu-id="25a65-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25a65-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25a65-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="25a65-115">Permission type</span></span>      | <span data-ttu-id="25a65-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="25a65-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25a65-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="25a65-117">Delegated (work or school account)</span></span> | <span data-ttu-id="25a65-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25a65-118">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="25a65-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="25a65-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25a65-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="25a65-120">Not supported.</span></span>    |
|<span data-ttu-id="25a65-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="25a65-121">Application</span></span> | <span data-ttu-id="25a65-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25a65-122">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="25a65-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="25a65-123">HTTP request</span></span>
<span data-ttu-id="25a65-124"><!-- { "blockType": "ignored" } -->Anlagen für einen [Posten](../resources/post.md) in einem [Thread](../resources/conversationthread.md) , die zu einer [Unterhaltung](../resources/conversation.md) einer Gruppe gehören.</span><span class="sxs-lookup"><span data-stu-id="25a65-124"><!-- { "blockType": "ignored" } --> Attachments for a [post](../resources/post.md) in a [thread](../resources/conversationthread.md) belonging to a [conversation](../resources/conversation.md) of a group.</span></span>
```http
POST /groups/{id}/threads/{id}/posts/{id}/attachments
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="25a65-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="25a65-125">Request headers</span></span>
| <span data-ttu-id="25a65-126">Header</span><span class="sxs-lookup"><span data-stu-id="25a65-126">Header</span></span>       | <span data-ttu-id="25a65-127">Wert</span><span class="sxs-lookup"><span data-stu-id="25a65-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="25a65-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="25a65-128">Authorization</span></span>  | <span data-ttu-id="25a65-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="25a65-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="25a65-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="25a65-131">Request body</span></span>
<span data-ttu-id="25a65-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="25a65-132">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="25a65-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="25a65-133">Response</span></span>

<span data-ttu-id="25a65-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [Attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25a65-134">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="25a65-135">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="25a65-135">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="25a65-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="25a65-136">Request</span></span>
<span data-ttu-id="25a65-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="25a65-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="25a65-138">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="25a65-138">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="25a65-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="25a65-139">Response</span></span>
<span data-ttu-id="25a65-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25a65-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```

## <a name="example-item-attachment"></a><span data-ttu-id="25a65-143">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="25a65-143">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="25a65-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="25a65-144">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_post"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "name": "name-value",
  "item": { }
}
```

##### <a name="response"></a><span data-ttu-id="25a65-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="25a65-145">Response</span></span>
<span data-ttu-id="25a65-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="25a65-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 162

{
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "contentType": "contentType-value",
  "size": 99,
  "isInline": true,
  "id": "id-value"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
