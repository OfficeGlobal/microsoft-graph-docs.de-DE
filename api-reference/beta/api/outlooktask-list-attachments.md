---
title: Anlagen auflisten
description: Rufen Sie eine Liste der Attachment-Objekte, die eine Outlook-Aufgabe zugeordnet ist.
ms.openlocfilehash: 11388a2a0bc2df1b0bb680e97326f7d0058c9e07
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062839"
---
# <a name="list-attachments"></a><span data-ttu-id="5693d-103">Anlagen auflisten</span><span class="sxs-lookup"><span data-stu-id="5693d-103">List attachments</span></span>

> <span data-ttu-id="5693d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5693d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5693d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5693d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5693d-106">Rufen Sie eine Liste der [Attachment](../resources/attachment.md) -Objekte, die eine Outlook-Aufgabe zugeordnet ist.</span><span class="sxs-lookup"><span data-stu-id="5693d-106">Get a list of [attachment](../resources/attachment.md) objects attached to an Outlook task.</span></span>
## <a name="permissions"></a><span data-ttu-id="5693d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5693d-107">Permissions</span></span>
<span data-ttu-id="5693d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5693d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5693d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5693d-110">Permission type</span></span>      | <span data-ttu-id="5693d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5693d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5693d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5693d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5693d-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5693d-113">Tasks.Read</span></span>    |
|<span data-ttu-id="5693d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5693d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5693d-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="5693d-115">Tasks.Read</span></span>    |
|<span data-ttu-id="5693d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5693d-116">Application</span></span> | <span data-ttu-id="5693d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5693d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5693d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5693d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}/attachments
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}/attachments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5693d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5693d-119">Optional query parameters</span></span>
<span data-ttu-id="5693d-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5693d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5693d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5693d-121">Request headers</span></span>
| <span data-ttu-id="5693d-122">Name</span><span class="sxs-lookup"><span data-stu-id="5693d-122">Name</span></span>      |<span data-ttu-id="5693d-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5693d-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5693d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5693d-124">Authorization</span></span>  | <span data-ttu-id="5693d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5693d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5693d-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5693d-127">Request body</span></span>
<span data-ttu-id="5693d-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5693d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5693d-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="5693d-129">Response</span></span>

<span data-ttu-id="5693d-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von [Attachment](../resources/attachment.md) -Objekte in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5693d-130">If successful, this method returns a `200 OK` response code and collection of [attachment](../resources/attachment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5693d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5693d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5693d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5693d-132">Request</span></span>
<span data-ttu-id="5693d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5693d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_attachments"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id}/outlook/tasks/{id}/attachments
```
##### <a name="response"></a><span data-ttu-id="5693d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="5693d-134">Response</span></span>
<span data-ttu-id="5693d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5693d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "lastModifiedDateTime": "datetime-value",
      "name": "name-value",
      "contentType": "contentType-value",
      "size": 99,
      "isInline": true,
      "id": "id-value"
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