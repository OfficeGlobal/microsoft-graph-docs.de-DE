---
title: Anlagen auflisten
description: Mit dieser API können Sie eine Liste der einem Ereignis angefügten Objekte des Typs attachment abrufen.
author: angelgolfer-ms
ms.openlocfilehash: 57545b89adc5cbb3c20ab782de04438b7b5ba9bf
ms.sourcegitcommit: 6b1ba9b3be038cd6247de54a255bad560034fe42
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/08/2019
ms.locfileid: "27771800"
---
# <a name="list-attachments"></a><span data-ttu-id="f754d-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="f754d-103">List attachments</span></span>

> <span data-ttu-id="f754d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f754d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f754d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f754d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f754d-106">Mit dieser API können Sie eine Liste der einem Ereignis angefügten Objekte des Typs [attachment](../resources/attachment.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="f754d-106">Retrieve a list of [attachment](../resources/attachment.md) objects attached to an event.</span></span>

## <a name="permissions"></a><span data-ttu-id="f754d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f754d-107">Permissions</span></span>

<span data-ttu-id="f754d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f754d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f754d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f754d-110">Permission type</span></span>      | <span data-ttu-id="f754d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f754d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f754d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f754d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f754d-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f754d-113">Calendars.Read</span></span>    |
|<span data-ttu-id="f754d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f754d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f754d-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f754d-115">Calendars.Read</span></span>    |
|<span data-ttu-id="f754d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f754d-116">Application</span></span> | <span data-ttu-id="f754d-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f754d-117">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="f754d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f754d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/events/{id}/attachments
GET /users/{id|userPrincipalName}/events/{id}/attachments
```

<!--
GET /groups/{id}/events/{id}/attachments
-->

## <a name="optional-query-parameters"></a><span data-ttu-id="f754d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f754d-119">Optional query parameters</span></span>

<span data-ttu-id="f754d-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f754d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f754d-121">Insbesondere, können Sie mithilfe der `$expand` Abfragen Parameter, um alle für das Ereignis Anlagen Inline mit dem Rest der Ereigniseigenschaften enthalten.</span><span class="sxs-lookup"><span data-stu-id="f754d-121">In particular, you can use the `$expand` query parameter to include all of the event attachments inline with the rest of the event properties.</span></span> <span data-ttu-id="f754d-122">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="f754d-122">For example:</span></span>

```http
GET https://graph.microsoft.com/beta/me/events/{id}?$expand=attachments
```

## <a name="request-headers"></a><span data-ttu-id="f754d-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f754d-123">Request headers</span></span>

| <span data-ttu-id="f754d-124">Name</span><span class="sxs-lookup"><span data-stu-id="f754d-124">Name</span></span>       | <span data-ttu-id="f754d-125">Typ</span><span class="sxs-lookup"><span data-stu-id="f754d-125">Type</span></span> | <span data-ttu-id="f754d-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f754d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f754d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f754d-127">Authorization</span></span>  | <span data-ttu-id="f754d-128">string</span><span class="sxs-lookup"><span data-stu-id="f754d-128">string</span></span>  | <span data-ttu-id="f754d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f754d-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f754d-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f754d-131">Request body</span></span>

<span data-ttu-id="f754d-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f754d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f754d-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f754d-133">Response</span></span>

<span data-ttu-id="f754d-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Attachment](../resources/attachment.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f754d-134">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/attachment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f754d-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f754d-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="f754d-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f754d-136">Request</span></span>

<span data-ttu-id="f754d-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f754d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->

```http
GET https://graph.microsoft.com/beta/me/events/{id}/attachments
```

### <a name="response"></a><span data-ttu-id="f754d-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="f754d-138">Response</span></span>

<span data-ttu-id="f754d-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f754d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 215

{
  "value": [
    {
      "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
      "contentType": "contentType-value",
      "contentLocation": "contentLocation-value",
      "contentBytes": "contentBytes-value",
      "contentId": "null",
      "lastModifiedDateTime": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "isInline": false,
      "isContactPhoto": false,
      "name": "name-value",
      "size": 99
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List attachments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->