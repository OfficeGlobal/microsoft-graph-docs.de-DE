---
title: Liste taskFolders
description: Rufen Sie Outlook Aufgabenordner in einer bestimmten OutlookTaskGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 66f755a994ea04a862051b6b32ce3ae9e6b39d0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857652"
---
# <a name="list-taskfolders"></a><span data-ttu-id="49d5c-103">Liste taskFolders</span><span class="sxs-lookup"><span data-stu-id="49d5c-103">List taskFolders</span></span>

> <span data-ttu-id="49d5c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="49d5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49d5c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="49d5c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="49d5c-106">Rufen Sie Outlook Aufgabenordner in einer bestimmten [OutlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="49d5c-106">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="49d5c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="49d5c-107">Permissions</span></span>
<span data-ttu-id="49d5c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49d5c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49d5c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="49d5c-110">Permission type</span></span>      | <span data-ttu-id="49d5c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="49d5c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49d5c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="49d5c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="49d5c-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="49d5c-113">Tasks.Read</span></span>    |
|<span data-ttu-id="49d5c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="49d5c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49d5c-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="49d5c-115">Tasks.Read</span></span>    |
|<span data-ttu-id="49d5c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="49d5c-116">Application</span></span> | <span data-ttu-id="49d5c-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="49d5c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49d5c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="49d5c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="49d5c-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="49d5c-119">Optional query parameters</span></span>
<span data-ttu-id="49d5c-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="49d5c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="49d5c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="49d5c-121">Request headers</span></span>
| <span data-ttu-id="49d5c-122">Name</span><span class="sxs-lookup"><span data-stu-id="49d5c-122">Name</span></span>      |<span data-ttu-id="49d5c-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="49d5c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49d5c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="49d5c-124">Authorization</span></span>  | <span data-ttu-id="49d5c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="49d5c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49d5c-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="49d5c-127">Request body</span></span>
<span data-ttu-id="49d5c-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="49d5c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49d5c-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="49d5c-129">Response</span></span>

<span data-ttu-id="49d5c-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [OutlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="49d5c-130">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="49d5c-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="49d5c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49d5c-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="49d5c-132">Request</span></span>
<span data-ttu-id="49d5c-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="49d5c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')/taskFolders
```
##### <a name="response"></a><span data-ttu-id="49d5c-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="49d5c-134">Response</span></span>
<span data-ttu-id="49d5c-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="49d5c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "value": [
    {
      "id": "AAMkADIyAAAhrbPXAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
      "isDefaultFolder": false,
      "name": "Cooking",
      "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List taskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
