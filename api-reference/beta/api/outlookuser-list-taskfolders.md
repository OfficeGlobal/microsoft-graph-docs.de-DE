---
title: Liste taskFolders
description: Rufen Sie alle Outlook Aufgabenordner im Postfach des Benutzers.
ms.openlocfilehash: 5c5636af9abe46b67d29fa03ae39d3020173849a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060359"
---
# <a name="list-taskfolders"></a><span data-ttu-id="1e905-103">Liste taskFolders</span><span class="sxs-lookup"><span data-stu-id="1e905-103">List taskFolders</span></span>

> <span data-ttu-id="1e905-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1e905-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1e905-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1e905-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1e905-106">Rufen Sie alle Outlook Aufgabenordner im Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="1e905-106">Get all the Outlook task folders in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e905-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1e905-107">Permissions</span></span>
<span data-ttu-id="1e905-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e905-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e905-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e905-110">Permission type</span></span>      | <span data-ttu-id="1e905-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e905-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e905-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e905-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1e905-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="1e905-113">Tasks.Read</span></span>    |
|<span data-ttu-id="1e905-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e905-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e905-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="1e905-115">Tasks.Read</span></span>    |
|<span data-ttu-id="1e905-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e905-116">Application</span></span> | <span data-ttu-id="1e905-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e905-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e905-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e905-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1e905-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1e905-119">Optional query parameters</span></span>
<span data-ttu-id="1e905-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1e905-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e905-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e905-121">Request headers</span></span>
| <span data-ttu-id="1e905-122">Name</span><span class="sxs-lookup"><span data-stu-id="1e905-122">Name</span></span>      |<span data-ttu-id="1e905-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e905-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1e905-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e905-124">Authorization</span></span>  | <span data-ttu-id="1e905-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1e905-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e905-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e905-127">Request body</span></span>
<span data-ttu-id="1e905-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1e905-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e905-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e905-129">Response</span></span>

<span data-ttu-id="1e905-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [OutlookTaskFolder](../resources/outlooktaskfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="1e905-130">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1e905-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e905-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1e905-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e905-132">Request</span></span>
<span data-ttu-id="1e905-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1e905-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders
```
##### <a name="response"></a><span data-ttu-id="1e905-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e905-134">Response</span></span>
<span data-ttu-id="1e905-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e905-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "AAMkADIyAAAAABrJAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
      "isDefaultFolder": false,
      "name": "Monthly tasks",
      "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAAAAESAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAAPA==",
      "isDefaultFolder": true,
      "name": "Tasks",
      "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List TaskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->