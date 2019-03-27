---
title: TaskFolders aufListen
description: Abrufen von Outlook-Aufgabenordnern in einem bestimmten Outlook Task Group.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c639fb0fe8e1ae010c3f5dbfb6b9c85c34009f00
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869463"
---
# <a name="list-taskfolders"></a><span data-ttu-id="85e69-103">TaskFolders aufListen</span><span class="sxs-lookup"><span data-stu-id="85e69-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85e69-104">Abrufen von Outlook-Aufgabenordnern in einem bestimmten [Outlook Task Group](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="85e69-104">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="85e69-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="85e69-105">Permissions</span></span>
<span data-ttu-id="85e69-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85e69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85e69-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85e69-108">Permission type</span></span>      | <span data-ttu-id="85e69-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85e69-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85e69-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85e69-110">Delegated (work or school account)</span></span> | <span data-ttu-id="85e69-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="85e69-111">Tasks.Read</span></span>    |
|<span data-ttu-id="85e69-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85e69-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85e69-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="85e69-113">Tasks.Read</span></span>    |
|<span data-ttu-id="85e69-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85e69-114">Application</span></span> | <span data-ttu-id="85e69-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="85e69-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="85e69-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85e69-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="85e69-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="85e69-117">Optional query parameters</span></span>
<span data-ttu-id="85e69-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="85e69-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85e69-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85e69-119">Request headers</span></span>
| <span data-ttu-id="85e69-120">Name</span><span class="sxs-lookup"><span data-stu-id="85e69-120">Name</span></span>      |<span data-ttu-id="85e69-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85e69-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="85e69-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="85e69-122">Authorization</span></span>  | <span data-ttu-id="85e69-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="85e69-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85e69-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85e69-125">Request body</span></span>
<span data-ttu-id="85e69-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="85e69-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85e69-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="85e69-127">Response</span></span>

<span data-ttu-id="85e69-128">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [Outlook Task Folder](../resources/outlooktaskfolder.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="85e69-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="85e69-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85e69-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85e69-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85e69-130">Request</span></span>
<span data-ttu-id="85e69-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85e69-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups('AAMkADIyAAAhrbe-AAA=')/taskFolders
```
##### <a name="response"></a><span data-ttu-id="85e69-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="85e69-132">Response</span></span>
<span data-ttu-id="85e69-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85e69-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
