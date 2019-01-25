---
title: Aufgaben auflisten
description: Rufen Sie die Outlook-Aufgaben im angegebenen Ordner.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 892409d6622ffd7b6e0243f7bcdb8807f2ee1305
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509343"
---
# <a name="list-tasks"></a><span data-ttu-id="463b9-103">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="463b9-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="463b9-104">Rufen Sie die Outlook-Aufgaben im angegebenen Ordner.</span><span class="sxs-lookup"><span data-stu-id="463b9-104">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="463b9-105">Standardmäßig wird dieses Vorgangs (und die POST, PATCH und [Abschließen von](../api/outlooktask-complete.md) Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="463b9-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="463b9-106">Sie können eine `Prefer: outlook.timezone` Anforderungsheader alle datumsspezifische Eigenschaften in der Antwort in einer anderen als UTC Zeitzone dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="463b9-106">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="463b9-107">Finden Sie ein [Beispiel](outlooktask-get.md#example-2) für eine einzelne Aufgabe abrufen.</span><span class="sxs-lookup"><span data-stu-id="463b9-107">See an [example](outlooktask-get.md#example-2) for getting a single task.</span></span> <span data-ttu-id="463b9-108">Sie können die Kopfzeile auf ähnliche Weise, um mehrere Aufgaben erhalten anwenden.</span><span class="sxs-lookup"><span data-stu-id="463b9-108">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="463b9-109">Wenn es mehr als eine Aufgabengruppe gibt und Sie alle Aufgaben in einer bestimmten Aufgabengruppe abrufen möchten, rufen Sie zunächst [alle Aufgabenordner in dieser Aufgabengruppe](outlooktaskgroup-list-taskfolders.md) ab und danach die Aufgaben in jedem dieser Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="463b9-109">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span> 

## <a name="permissions"></a><span data-ttu-id="463b9-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="463b9-110">Permissions</span></span>
<span data-ttu-id="463b9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="463b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="463b9-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="463b9-113">Permission type</span></span>      | <span data-ttu-id="463b9-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="463b9-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="463b9-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="463b9-115">Delegated (work or school account)</span></span> | <span data-ttu-id="463b9-116">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="463b9-116">Tasks.Read</span></span>    |
|<span data-ttu-id="463b9-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="463b9-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="463b9-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="463b9-118">Tasks.Read</span></span>    |
|<span data-ttu-id="463b9-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="463b9-119">Application</span></span> | <span data-ttu-id="463b9-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="463b9-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="463b9-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="463b9-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="463b9-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="463b9-122">Optional query parameters</span></span>
<span data-ttu-id="463b9-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="463b9-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="463b9-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="463b9-124">Request headers</span></span>
| <span data-ttu-id="463b9-125">Name</span><span class="sxs-lookup"><span data-stu-id="463b9-125">Name</span></span>      |<span data-ttu-id="463b9-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="463b9-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="463b9-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="463b9-127">Authorization</span></span>  | <span data-ttu-id="463b9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="463b9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="463b9-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="463b9-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="463b9-131">Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="463b9-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="463b9-132">Optional.</span><span class="sxs-lookup"><span data-stu-id="463b9-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="463b9-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="463b9-133">Request body</span></span>
<span data-ttu-id="463b9-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="463b9-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="463b9-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="463b9-135">Response</span></span>

<span data-ttu-id="463b9-136">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [OutlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="463b9-136">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="463b9-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="463b9-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="463b9-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="463b9-138">Request</span></span>
<span data-ttu-id="463b9-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="463b9-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
##### <a name="response"></a><span data-ttu-id="463b9-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="463b9-140">Response</span></span>
<span data-ttu-id="463b9-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="463b9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
