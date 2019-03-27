---
title: Task Groups aufListen
description: Rufen Sie alle Outlook-Aufgabengruppen im Postfach des Benutzers ab.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: b3ebf2896ff8805280c23680915e54f9a094a7c8
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869358"
---
# <a name="list-taskgroups"></a><span data-ttu-id="7f980-103">Task Groups aufListen</span><span class="sxs-lookup"><span data-stu-id="7f980-103">List taskGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f980-104">Rufen Sie alle Outlook-Aufgabengruppen im Postfach des Benutzers ab.</span><span class="sxs-lookup"><span data-stu-id="7f980-104">Get all the Outlook task groups in the user's mailbox.</span></span>

<span data-ttu-id="7f980-105">Die Antwort enthält immer die Standardaufgabengruppe `My Tasks` und alle anderen Aufgabengruppen, die im Postfach erstellt wurden.</span><span class="sxs-lookup"><span data-stu-id="7f980-105">The response always includes the default task group `My Tasks`, and any other task groups that have been created in the mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="7f980-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7f980-106">Permissions</span></span>
<span data-ttu-id="7f980-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f980-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f980-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f980-109">Permission type</span></span>      | <span data-ttu-id="7f980-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f980-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f980-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f980-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7f980-112">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="7f980-112">Tasks.Read</span></span>    |
|<span data-ttu-id="7f980-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f980-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f980-114">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="7f980-114">Tasks.Read</span></span>    |
|<span data-ttu-id="7f980-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f980-115">Application</span></span> | <span data-ttu-id="7f980-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f980-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f980-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f980-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups
GET /users/{id|userPrincipalName}/outlook/taskGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7f980-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7f980-118">Optional query parameters</span></span>
<span data-ttu-id="7f980-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7f980-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f980-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f980-120">Request headers</span></span>
| <span data-ttu-id="7f980-121">Name</span><span class="sxs-lookup"><span data-stu-id="7f980-121">Name</span></span>      |<span data-ttu-id="7f980-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f980-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f980-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f980-123">Authorization</span></span>  | <span data-ttu-id="7f980-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7f980-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f980-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f980-126">Request body</span></span>
<span data-ttu-id="7f980-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7f980-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f980-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f980-128">Response</span></span>

<span data-ttu-id="7f980-129">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [Outlook Task Group](../resources/outlooktaskgroup.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="7f980-129">If successful, this method returns a `200 OK` response code and collection of [outlookTaskGroup](../resources/outlooktaskgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f980-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f980-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f980-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f980-131">Request</span></span>
<span data-ttu-id="7f980-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f980-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_taskgroups"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups
```
##### <a name="response"></a><span data-ttu-id="7f980-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f980-133">Response</span></span>
<span data-ttu-id="7f980-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f980-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

{
  "value": [
    {
      "id": "AAMkADIyAAADJ5pYAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxLA==",
      "isDefaultGroup": true,
      "name": "My Tasks",
      "groupKey": "0006f0b7-0000-0000-c000-000000000046"
    },
    {
      "id": "AAMkADIyAAAhrbe-AAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAInHxKw==",
      "isDefaultGroup": false,
      "name": "Leisure Tasks",
      "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List TaskGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-list-taskgroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
