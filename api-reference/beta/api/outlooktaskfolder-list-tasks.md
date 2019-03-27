---
title: Aufgaben auflisten
description: Rufen Sie alle Outlook-Aufgaben im angegebenen Ordner ab.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a1769c83dc84e70ed051f5d1d284d00de7c71ae4
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869470"
---
# <a name="list-tasks"></a><span data-ttu-id="97578-103">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="97578-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97578-104">Rufen Sie alle Outlook-Aufgaben im angegebenen Ordner ab.</span><span class="sxs-lookup"><span data-stu-id="97578-104">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="97578-105">Standardmäßig gibt dieser Vorgang (und die Vorgänge POST, PATCH und [Vollständiger](../api/outlooktask-complete.md) Vorgang) datumsbezogene Eigenschaften in UTC zurück.</span><span class="sxs-lookup"><span data-stu-id="97578-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="97578-106">Sie können einen `Prefer: outlook.timezone` Anforderungsheader verwenden, um alle datumsbezogenen Eigenschaften in der Antwort zu haben, die in einer anderen Zeitzone als UTC dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="97578-106">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="97578-107">Sehen Sie sich ein [Beispiel](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) für eine einzelne Aufgabe an.</span><span class="sxs-lookup"><span data-stu-id="97578-107">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="97578-108">Sie können die Kopfzeile entsprechend anwenden, um mehrere Vorgänge abzurufen.</span><span class="sxs-lookup"><span data-stu-id="97578-108">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="97578-109">Wenn es mehr als eine Aufgabengruppe gibt und Sie alle Vorgänge in einer bestimmten Aufgabengruppe abrufen möchten, rufen Sie zunächst [alle Aufgabenordner in dieser Aufgabengruppe](outlooktaskgroup-list-taskfolders.md)ab, und rufen Sie dann die Aufgaben in jedem dieser Aufgabenordner ab.</span><span class="sxs-lookup"><span data-stu-id="97578-109">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="97578-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="97578-110">Permissions</span></span>
<span data-ttu-id="97578-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="97578-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97578-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="97578-113">Permission type</span></span>      | <span data-ttu-id="97578-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="97578-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97578-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="97578-115">Delegated (work or school account)</span></span> | <span data-ttu-id="97578-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="97578-116">Tasks.Read</span></span>    |
|<span data-ttu-id="97578-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="97578-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97578-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="97578-118">Tasks.Read</span></span>    |
|<span data-ttu-id="97578-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="97578-119">Application</span></span> | <span data-ttu-id="97578-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="97578-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97578-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="97578-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}/tasks
GET /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="97578-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="97578-122">Optional query parameters</span></span>
<span data-ttu-id="97578-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="97578-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97578-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="97578-124">Request headers</span></span>
| <span data-ttu-id="97578-125">Name</span><span class="sxs-lookup"><span data-stu-id="97578-125">Name</span></span>      |<span data-ttu-id="97578-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="97578-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="97578-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="97578-127">Authorization</span></span>  | <span data-ttu-id="97578-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="97578-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="97578-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="97578-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="97578-131">Gibt die Zeitzone für Zeit Eigenschaften in der Antwort an, die in UTC wäre, wenn diese Kopfzeile nicht angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="97578-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="97578-132">Optional.</span><span class="sxs-lookup"><span data-stu-id="97578-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="97578-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="97578-133">Request body</span></span>
<span data-ttu-id="97578-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="97578-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97578-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="97578-135">Response</span></span>

<span data-ttu-id="97578-136">Bei erfolgreicher Ausführung gibt die Methode den `200 OK` Antwortcode und eine Sammlung von [Outlook Task](../resources/outlooktask.md) -Objekten im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="97578-136">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97578-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="97578-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97578-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="97578-138">Request</span></span>
<span data-ttu-id="97578-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="97578-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
##### <a name="response"></a><span data-ttu-id="97578-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="97578-140">Response</span></span>
<span data-ttu-id="97578-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="97578-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 465

{
  "value": [
   {
      "id": "AAMkADA1MTrfAAA=",
      "createdDateTime": "2016-04-22T05:44:01.2012012Z",
      "lastModifiedDateTime": "2016-04-22T05:44:02.9980882Z",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMxw==",
      "categories": [ ],
      "assignedTo": null,
      "body": {
        "contentType": "text",
        "content": ""
      },
      "completedDateTime": null,
      "dueDateTime": {
        "dateTime": "2016-04-25T07:00:00.0000000",
        "timeZone": "UTC"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
        "dateTime": "2016-04-23T07:00:00.0000000",
        "timeZone": "UTC"
      },
      "status": "notStarted",
      "subject": "Shop for dinner"
    },
    {
      "id": "AAMkADA1MTrgAAA=",
      "createdDateTime": "2016-04-22T06:03:35.9279794Z",
      "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
      "categories": [ ],
      "assignedTo": null,
      "body": {
        "contentType": "text",
        "content": ""
      },
      "completedDateTime": null,
      "dueDateTime": {
        "dateTime": "2016-04-27T04:00:00.0000000",
        "timeZone": "UTC"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
        "dateTime": "2016-04-26T04:00:00.0000000",
        "timeZone": "UTC"
      },
      "status": "notStarted",
      "subject": "Shop for dinner"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-list-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
