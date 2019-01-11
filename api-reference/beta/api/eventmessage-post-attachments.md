---
title: Anlage hinzufügen
description: Verwenden Sie diese API, um eine neue Anlage zu erstellen.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: e56da5a4b6f57506800e07e3f8e2b09ed7ef6f46
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824080"
---
# <a name="add-attachment"></a><span data-ttu-id="ec1e2-103">Anlage hinzufügen</span><span class="sxs-lookup"><span data-stu-id="ec1e2-103">Add attachment</span></span>

> <span data-ttu-id="ec1e2-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec1e2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ec1e2-106">Verwenden Sie diese API, um eine neue Anlage zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-106">Use this API to create a new Attachment.</span></span>

<span data-ttu-id="ec1e2-107">Eine Anlage weist einen der folgenden Typen auf:</span><span class="sxs-lookup"><span data-stu-id="ec1e2-107">An attachment can be one of the following types:</span></span>

* <span data-ttu-id="ec1e2-108">Datei ([fileAttachment](../resources/fileattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="ec1e2-108">A file ([fileAttachment](../resources/fileattachment.md) resource).</span></span>
* <span data-ttu-id="ec1e2-109">Element (Kontakt, Ereignis oder Nachricht, dargestellt durch eine [itemAttachment](../resources/itemattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="ec1e2-109">An item (contact, event or message, represented by an [itemAttachment](../resources/itemattachment.md) resource).</span></span>
* <span data-ttu-id="ec1e2-110">Link zu einer Datei ([referenceAttachment](../resources/referenceattachment.md)-Ressource)</span><span class="sxs-lookup"><span data-stu-id="ec1e2-110">A link to a file ([referenceAttachment](../resources/referenceattachment.md) resource).</span></span>

<span data-ttu-id="ec1e2-111">All diese Typen von Anlagenressourcen werden von der Ressource [attachment](../resources/attachment.md) abgeleitet.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-111">All these types of attachment resources are derived from the [attachment](../resources/attachment.md) resource.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ec1e2-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ec1e2-112">Permissions</span></span>
<span data-ttu-id="ec1e2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec1e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec1e2-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec1e2-115">Permission type</span></span>      | <span data-ttu-id="ec1e2-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec1e2-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec1e2-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec1e2-117">Delegated (work or school account)</span></span> | <span data-ttu-id="ec1e2-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec1e2-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ec1e2-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec1e2-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec1e2-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec1e2-120">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ec1e2-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec1e2-121">Application</span></span> | <span data-ttu-id="ec1e2-122">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ec1e2-122">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec1e2-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec1e2-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/attachments
POST /users/{id|userPrincipalName}/messages/{id}/attachments
```
## <a name="request-headers"></a><span data-ttu-id="ec1e2-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec1e2-124">Request headers</span></span>
| <span data-ttu-id="ec1e2-125">Name</span><span class="sxs-lookup"><span data-stu-id="ec1e2-125">Name</span></span>       | <span data-ttu-id="ec1e2-126">Typ</span><span class="sxs-lookup"><span data-stu-id="ec1e2-126">Type</span></span> | <span data-ttu-id="ec1e2-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec1e2-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ec1e2-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec1e2-128">Authorization</span></span>  | <span data-ttu-id="ec1e2-129">string</span><span class="sxs-lookup"><span data-stu-id="ec1e2-129">string</span></span>  | <span data-ttu-id="ec1e2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ec1e2-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec1e2-132">Content-Type</span></span> | <span data-ttu-id="ec1e2-133">string</span><span class="sxs-lookup"><span data-stu-id="ec1e2-133">string</span></span>  | <span data-ttu-id="ec1e2-p104">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-p104">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec1e2-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec1e2-136">Request body</span></span>
<span data-ttu-id="ec1e2-137">Geben Sie im Anforderungstext eine JSON-Darstellung des [Attachment](../resources/attachment.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-137">In the request body, supply a JSON representation of [Attachment](../resources/attachment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ec1e2-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec1e2-138">Response</span></span>

<span data-ttu-id="ec1e2-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [Attachment](../resources/attachment.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-139">If successful, this method returns `201 Created` response code and [Attachment](../resources/attachment.md) object in the response body.</span></span>

## <a name="example-file-attachment"></a><span data-ttu-id="ec1e2-140">Beispiel (Dateianlage)</span><span class="sxs-lookup"><span data-stu-id="ec1e2-140">Example (file attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="ec1e2-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec1e2-141">Request</span></span>
<span data-ttu-id="ec1e2-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-142">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ec1e2-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec1e2-143">Response</span></span>
<span data-ttu-id="ec1e2-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
} -->
```http
HTTP 201 Created
```


## <a name="example-item-attachment"></a><span data-ttu-id="ec1e2-147">Beispiel (Elementanlage)</span><span class="sxs-lookup"><span data-stu-id="ec1e2-147">Example (item attachment)</span></span>

##### <a name="request"></a><span data-ttu-id="ec1e2-148">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec1e2-148">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="ec1e2-149">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec1e2-149">Response</span></span>
<span data-ttu-id="ec1e2-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec1e2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Attachment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
