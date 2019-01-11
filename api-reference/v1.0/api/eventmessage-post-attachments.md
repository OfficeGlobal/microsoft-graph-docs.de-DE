---
title: Anlage hinzufügen
description: Verwenden Sie diese API, um eine neue Anlage zu erstellen.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 59e1271e6b27b68e813cb0386c8041a2608a82e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806468"
---
# <a name="add-attachment"></a><span data-ttu-id="aaefe-103">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="aaefe-103">Add attachment</span></span>

<span data-ttu-id="aaefe-104">Verwenden Sie diese API, um eine neue Anlage zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="aaefe-104">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="aaefe-105">Eine Anlage weist einen der folgenden Typen auf:</span><span class="sxs-lookup"><span data-stu-id="aaefe-105">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="aaefe-106">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="aaefe-106">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="aaefe-107">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="aaefe-107">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="aaefe-108">Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="aaefe-108">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="aaefe-109">All diese Typen von Anlagenressourcen werden von der Ressource [attachment](../resources/attachment.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="aaefe-109">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="aaefe-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="aaefe-110">Permissions</span></span>
<span data-ttu-id="aaefe-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaefe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaefe-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="aaefe-113">Permission type</span></span>      | <span data-ttu-id="aaefe-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="aaefe-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaefe-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="aaefe-115">Delegated (work or school account)</span></span> | <span data-ttu-id="aaefe-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaefe-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aaefe-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="aaefe-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaefe-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaefe-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aaefe-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="aaefe-119">Application</span></span> | <span data-ttu-id="aaefe-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aaefe-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaefe-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="aaefe-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id | userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="aaefe-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="aaefe-122">Request headers</span></span>
| <span data-ttu-id="aaefe-123">Name</span><span class="sxs-lookup"><span data-stu-id="aaefe-123">Name</span></span>       | <span data-ttu-id="aaefe-124">Typ</span><span class="sxs-lookup"><span data-stu-id="aaefe-124">Type</span></span> | <span data-ttu-id="aaefe-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="aaefe-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aaefe-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaefe-126">Authorization</span></span>  | <span data-ttu-id="aaefe-127">string</span><span class="sxs-lookup"><span data-stu-id="aaefe-127">string</span></span>  | <span data-ttu-id="aaefe-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aaefe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="aaefe-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aaefe-130">Content-Type</span></span> | <span data-ttu-id="aaefe-131">string</span><span class="sxs-lookup"><span data-stu-id="aaefe-131">string</span></span>  | <span data-ttu-id="aaefe-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="aaefe-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aaefe-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="aaefe-134">Request body</span></span>
<span data-ttu-id="aaefe-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="aaefe-135">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aaefe-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="aaefe-136">Response</span></span>

<span data-ttu-id="aaefe-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [Attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aaefe-137">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="aaefe-138">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="aaefe-138">Example (File attachment)</span></span>
##### <a name="request"></a><span data-ttu-id="aaefe-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aaefe-139">Request</span></span>
<span data-ttu-id="aaefe-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="aaefe-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_file_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/attachments
Content-type: application/json
Content-length: 142

{
  "@odata.type": "microsoft.graph.fileAttachment",
  "name": "name-value",
  "contentType": "contentType-value",
  "isInline": false,
  "contentLocation": "contentLocation-value",
  "contentBytes": "base64-contentBytes-value"
}
```

<span data-ttu-id="aaefe-141">Geben Sie im Anforderungstext eine JSON-Darstellung des [attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="aaefe-141">In the request body, supply a JSON representation of [attachment](../resources/attachment.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="aaefe-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="aaefe-142">Response</span></span>
<span data-ttu-id="aaefe-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aaefe-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
```

## <a name="example-item-attachment"></a><span data-ttu-id="aaefe-146">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="aaefe-146">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="aaefe-147">Anforderung</span><span class="sxs-lookup"><span data-stu-id="aaefe-147">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "create_item_attachment_from_eventmessage"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/events/{id}/attachments
Content-type: application/json
Content-length: 100

{
  "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
  "name": "name-value",
  "item": "message or event entity"
}
```

##### <a name="response"></a><span data-ttu-id="aaefe-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="aaefe-148">Response</span></span>
<span data-ttu-id="aaefe-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="aaefe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP/1.1 201 Created
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
