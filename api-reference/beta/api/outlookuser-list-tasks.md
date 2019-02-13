---
title: Aufgaben auflisten
description: Rufen Sie die Outlook-Aufgaben in das Postfach des Benutzers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f854d5649c311531e65909c3d6b33f356cd5bac2
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967354"
---
# <a name="list-tasks"></a><span data-ttu-id="cf6e8-103">Aufgaben auflisten</span><span class="sxs-lookup"><span data-stu-id="cf6e8-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf6e8-104">Rufen Sie die Outlook-Aufgaben in das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-104">Get all the Outlook tasks in the user's mailbox.</span></span>

<span data-ttu-id="cf6e8-105">Standardmäßig wird dieses Vorgangs (und die POST, PATCH und [Abschließen von](../api/outlooktask-complete.md) Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span>
<span data-ttu-id="cf6e8-106">Sie können die `Prefer: outlook.timezone`-Kopfzeile verwenden, um alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darzustellen.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span> <span data-ttu-id="cf6e8-107">Finden Sie ein [Beispiel](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) für eine einzelne Aufgabe abrufen.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-107">See an [example](outlooktask-get.md#example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time) for getting a single task.</span></span> <span data-ttu-id="cf6e8-108">Sie können die Kopfzeile auf ähnliche Weise, um mehrere Aufgaben erhalten anwenden.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-108">You can apply the header similarly to get multiple tasks.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf6e8-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cf6e8-109">Permissions</span></span>
<span data-ttu-id="cf6e8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf6e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf6e8-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cf6e8-112">Permission type</span></span>      | <span data-ttu-id="cf6e8-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cf6e8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf6e8-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cf6e8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cf6e8-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="cf6e8-115">Tasks.Read</span></span>    |
|<span data-ttu-id="cf6e8-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cf6e8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf6e8-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="cf6e8-117">Tasks.Read</span></span>    |
|<span data-ttu-id="cf6e8-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cf6e8-118">Application</span></span> | <span data-ttu-id="cf6e8-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cf6e8-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cf6e8-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf6e8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cf6e8-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="cf6e8-121">Optional query parameters</span></span>
<span data-ttu-id="cf6e8-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf6e8-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cf6e8-123">Request headers</span></span>
| <span data-ttu-id="cf6e8-124">Name</span><span class="sxs-lookup"><span data-stu-id="cf6e8-124">Name</span></span>      |<span data-ttu-id="cf6e8-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cf6e8-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cf6e8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf6e8-126">Authorization</span></span>  | <span data-ttu-id="cf6e8-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cf6e8-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="cf6e8-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="cf6e8-130">Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="cf6e8-131">Optional.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf6e8-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cf6e8-132">Request body</span></span>
<span data-ttu-id="cf6e8-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf6e8-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf6e8-134">Response</span></span>

<span data-ttu-id="cf6e8-135">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [OutlookTask](../resources/outlooktask.md) .</span><span class="sxs-lookup"><span data-stu-id="cf6e8-135">If successful, this method returns a `200 OK` response code and collection of [outlookTask](../resources/outlooktask.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="cf6e8-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cf6e8-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cf6e8-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cf6e8-137">Request</span></span>
<span data-ttu-id="cf6e8-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/tasks
```
##### <a name="response"></a><span data-ttu-id="cf6e8-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="cf6e8-139">Response</span></span>
<span data-ttu-id="cf6e8-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-140">Here is an example of the response.</span></span> <span data-ttu-id="cf6e8-141">Standardmäßig sind die Datums-/Uhrzeiteigenschaften in der Antwort in UTC angegeben.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-141">By default, the date-time properties in the response are in UTC.</span></span>

<span data-ttu-id="cf6e8-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cf6e8-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List Tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-list-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
