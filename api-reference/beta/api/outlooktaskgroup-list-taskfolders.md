---
title: Liste taskFolders
description: Rufen Sie Outlook Aufgabenordner in einer bestimmten OutlookTaskGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 16a3463a7cdc4a3bc4efd401c7ca1a8932c82b7c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508286"
---
# <a name="list-taskfolders"></a><span data-ttu-id="c3ac5-103">Liste taskFolders</span><span class="sxs-lookup"><span data-stu-id="c3ac5-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3ac5-104">Rufen Sie Outlook Aufgabenordner in einer bestimmten [OutlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="c3ac5-104">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c3ac5-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c3ac5-105">Permissions</span></span>
<span data-ttu-id="c3ac5-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3ac5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3ac5-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c3ac5-108">Permission type</span></span>      | <span data-ttu-id="c3ac5-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c3ac5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3ac5-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c3ac5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3ac5-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c3ac5-111">Tasks.Read</span></span>    |
|<span data-ttu-id="c3ac5-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c3ac5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3ac5-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="c3ac5-113">Tasks.Read</span></span>    |
|<span data-ttu-id="c3ac5-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c3ac5-114">Application</span></span> | <span data-ttu-id="c3ac5-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3ac5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3ac5-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3ac5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c3ac5-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c3ac5-117">Optional query parameters</span></span>
<span data-ttu-id="c3ac5-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3ac5-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c3ac5-119">Request headers</span></span>
| <span data-ttu-id="c3ac5-120">Name</span><span class="sxs-lookup"><span data-stu-id="c3ac5-120">Name</span></span>      |<span data-ttu-id="c3ac5-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3ac5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c3ac5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3ac5-122">Authorization</span></span>  | <span data-ttu-id="c3ac5-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3ac5-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c3ac5-125">Request body</span></span>
<span data-ttu-id="c3ac5-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3ac5-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3ac5-127">Response</span></span>

<span data-ttu-id="c3ac5-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [OutlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="c3ac5-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c3ac5-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c3ac5-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3ac5-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3ac5-130">Request</span></span>
<span data-ttu-id="c3ac5-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')/taskFolders
```
##### <a name="response"></a><span data-ttu-id="c3ac5-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3ac5-132">Response</span></span>
<span data-ttu-id="c3ac5-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c3ac5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List taskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskgroup-list-taskfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
