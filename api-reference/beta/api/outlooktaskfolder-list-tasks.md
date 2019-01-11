---
title: Aufgaben auflisten
description: Rufen Sie die Outlook-Aufgaben im angegebenen Ordner.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: ee6b4c2454ba6bfad0c0f4e6acd826917f02ca93
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863077"
---
# <a name="list-tasks"></a><span data-ttu-id="7f692-103">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="7f692-103">List tasks</span></span>

> <span data-ttu-id="7f692-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7f692-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f692-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7f692-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f692-106">Rufen Sie die Outlook-Aufgaben im angegebenen Ordner.</span><span class="sxs-lookup"><span data-stu-id="7f692-106">Get all the Outlook tasks in the specified folder.</span></span>

<span data-ttu-id="7f692-107">Standardmäßig wird dieses Vorgangs (und die POST, PATCH und [Abschließen von](../api/outlooktask-complete.md) Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f692-107">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>  <span data-ttu-id="7f692-108">Sie können eine `Prefer: outlook.timezone` Anforderungsheader alle datumsspezifische Eigenschaften in der Antwort in einer anderen als UTC Zeitzone dargestellt werden.</span><span class="sxs-lookup"><span data-stu-id="7f692-108">You can use a `Prefer: outlook.timezone` request header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="7f692-109">Finden Sie ein [Beispiel](outlooktask-get.md#example-2) für eine einzelne Aufgabe abrufen.</span><span class="sxs-lookup"><span data-stu-id="7f692-109">See an [example](outlooktask-get.md#example-2) for getting a single task.</span></span> <span data-ttu-id="7f692-110">Sie können die Kopfzeile auf ähnliche Weise, um mehrere Aufgaben erhalten anwenden.</span><span class="sxs-lookup"><span data-stu-id="7f692-110">You can apply the header similarly to get multiple tasks.</span></span>

<span data-ttu-id="7f692-111">Wenn mehr als ein "Task Group" vorhanden ist, und rufen alle Aufgaben in eine bestimmte Aufgabengruppe zuerst [Alle Aufgabenordner in dieser Aufgabengruppe erhalten möchten](outlooktaskgroup-list-taskfolders.md), und klicken Sie dann die Aufgaben in jeder dieser Aufgabenordner werden soll.</span><span class="sxs-lookup"><span data-stu-id="7f692-111">If there is more than one task group, and you want to get all the tasks in a specific task group, first [get all the task folders in that task group](outlooktaskgroup-list-taskfolders.md), and then get the tasks in each of these task folders.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7f692-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7f692-112">Permissions</span></span>
<span data-ttu-id="7f692-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f692-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f692-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f692-115">Permission type</span></span>      | <span data-ttu-id="7f692-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f692-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f692-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f692-117">Delegated (work or school account)</span></span> | <span data-ttu-id="7f692-118">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="7f692-118">Tasks.Read</span></span>    |
|<span data-ttu-id="7f692-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f692-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f692-120">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="7f692-120">Tasks.Read</span></span>    |
|<span data-ttu-id="7f692-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f692-121">Application</span></span> | <span data-ttu-id="7f692-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f692-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f692-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f692-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7f692-124">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7f692-124">Optional query parameters</span></span>
<span data-ttu-id="7f692-125">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7f692-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f692-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f692-126">Request headers</span></span>
| <span data-ttu-id="7f692-127">Name</span><span class="sxs-lookup"><span data-stu-id="7f692-127">Name</span></span>      |<span data-ttu-id="7f692-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f692-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7f692-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f692-129">Authorization</span></span>  | <span data-ttu-id="7f692-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7f692-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7f692-132">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="7f692-132">Prefer: outlook.timezone</span></span> | <span data-ttu-id="7f692-133">Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="7f692-133">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="7f692-134">Optional.</span><span class="sxs-lookup"><span data-stu-id="7f692-134">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f692-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f692-135">Request body</span></span>
<span data-ttu-id="7f692-136">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7f692-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f692-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f692-137">Response</span></span>

<span data-ttu-id="7f692-138">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [OutlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="7f692-138">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7f692-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f692-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f692-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f692-140">Request</span></span>
<span data-ttu-id="7f692-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f692-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=/tasks
```
##### <a name="response"></a><span data-ttu-id="7f692-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f692-142">Response</span></span>
<span data-ttu-id="7f692-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f692-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
