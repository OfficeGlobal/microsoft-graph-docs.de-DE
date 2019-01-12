---
title: Abrufen von outlookTaskFolder
description: Rufen Sie die Eigenschaften und Beziehungen zwischen den angegebenen Outlook-Aufgabenordner.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 7e8f8e9c1fa16b5e0a00b0f779d652d2c6e1aa93
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929221"
---
# <a name="get-outlooktaskfolder"></a><span data-ttu-id="69629-103">Abrufen von outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="69629-103">Get outlookTaskFolder</span></span>

> <span data-ttu-id="69629-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="69629-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69629-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="69629-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="69629-106">Rufen Sie die Eigenschaften und Beziehungen zwischen den angegebenen Outlook-Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="69629-106">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="69629-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="69629-107">Permissions</span></span>
<span data-ttu-id="69629-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="69629-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69629-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="69629-110">Permission type</span></span>      | <span data-ttu-id="69629-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="69629-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69629-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="69629-112">Delegated (work or school account)</span></span> | <span data-ttu-id="69629-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="69629-113">Tasks.Read</span></span>    |
|<span data-ttu-id="69629-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="69629-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69629-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="69629-115">Tasks.Read</span></span>    |
|<span data-ttu-id="69629-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="69629-116">Application</span></span> | <span data-ttu-id="69629-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="69629-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="69629-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="69629-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="69629-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="69629-119">Optional query parameters</span></span>
<span data-ttu-id="69629-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="69629-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="69629-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="69629-121">Request headers</span></span>
| <span data-ttu-id="69629-122">Name</span><span class="sxs-lookup"><span data-stu-id="69629-122">Name</span></span>      |<span data-ttu-id="69629-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="69629-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="69629-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="69629-124">Authorization</span></span>  | <span data-ttu-id="69629-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="69629-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69629-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="69629-127">Request body</span></span>
<span data-ttu-id="69629-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="69629-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69629-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="69629-129">Response</span></span>

<span data-ttu-id="69629-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [OutlookTaskFolder](../resources/outlooktaskfolder.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="69629-130">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="69629-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="69629-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="69629-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="69629-132">Request</span></span>
<span data-ttu-id="69629-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="69629-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAAABrJAAA=')
```
##### <a name="response"></a><span data-ttu-id="69629-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="69629-134">Response</span></span>
<span data-ttu-id="69629-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="69629-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAAABrJAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
  "isDefaultFolder": false,
  "name": "Monthly tasks",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
