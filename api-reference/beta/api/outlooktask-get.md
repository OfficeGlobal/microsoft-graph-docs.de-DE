---
title: Abrufen von outlookTask
description: Rufen Sie die Eigenschaften und Beziehungen zwischen Outlook-Aufgaben in das Postfach des Benutzers an.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 47c6a24ccb76eb7752736386cf6ec17330832780
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526319"
---
# <a name="get-outlooktask"></a><span data-ttu-id="65ca9-103">Abrufen von outlookTask</span><span class="sxs-lookup"><span data-stu-id="65ca9-103">Get outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65ca9-104">Rufen Sie die Eigenschaften und Beziehungen zwischen Outlook-Aufgaben in das Postfach des Benutzers an.</span><span class="sxs-lookup"><span data-stu-id="65ca9-104">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="65ca9-105">Standardmäßig wird dieses Vorgangs (und die POST, PATCH und [Abschließen von](../api/outlooktask-complete.md) Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65ca9-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="65ca9-106">Sie können mit dem `Prefer: outlook.timezone`-Header alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darstellen.</span><span class="sxs-lookup"><span data-stu-id="65ca9-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="65ca9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="65ca9-107">Permissions</span></span>

<span data-ttu-id="65ca9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65ca9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65ca9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="65ca9-110">Permission type</span></span>      | <span data-ttu-id="65ca9-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="65ca9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65ca9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="65ca9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="65ca9-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="65ca9-113">Tasks.Read</span></span>    |
|<span data-ttu-id="65ca9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="65ca9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65ca9-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="65ca9-115">Tasks.Read</span></span>    |
|<span data-ttu-id="65ca9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="65ca9-116">Application</span></span> | <span data-ttu-id="65ca9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="65ca9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="65ca9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="65ca9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="65ca9-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="65ca9-119">Optional query parameters</span></span>

<span data-ttu-id="65ca9-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="65ca9-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65ca9-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="65ca9-121">Request headers</span></span>

| <span data-ttu-id="65ca9-122">Name</span><span class="sxs-lookup"><span data-stu-id="65ca9-122">Name</span></span>      |<span data-ttu-id="65ca9-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="65ca9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="65ca9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="65ca9-124">Authorization</span></span>  | <span data-ttu-id="65ca9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="65ca9-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="65ca9-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="65ca9-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="65ca9-128">Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="65ca9-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="65ca9-129">Optional.</span><span class="sxs-lookup"><span data-stu-id="65ca9-129">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65ca9-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="65ca9-130">Request body</span></span>

<span data-ttu-id="65ca9-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="65ca9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65ca9-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="65ca9-132">Response</span></span>

<span data-ttu-id="65ca9-133">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [OutlookTask](../resources/outlooktask.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="65ca9-133">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="65ca9-134">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="65ca9-134">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="65ca9-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65ca9-135">Request</span></span>

<span data-ttu-id="65ca9-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="65ca9-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTrgAAA=')
```

### <a name="response"></a><span data-ttu-id="65ca9-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="65ca9-137">Response</span></span>

<span data-ttu-id="65ca9-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="65ca9-138">Here is an example of the response.</span></span> <span data-ttu-id="65ca9-139">Standardmäßig sind die Datums-/Uhrzeiteigenschaften in der Antwort in UTC angegeben.</span><span class="sxs-lookup"><span data-stu-id="65ca9-139">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="65ca9-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65ca9-p106">**Note:** The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 376

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
```

## <a name="example-2"></a><span data-ttu-id="65ca9-142">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="65ca9-142">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="65ca9-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="65ca9-143">Request</span></span>

<span data-ttu-id="65ca9-144">In diesem Beispiel wird die `Prefer: outlook.timezone` Header zum Anzeigen von Datum / Uhrzeit-Eigenschaften in der Pacific Standard Time-Antwort angeben.</span><span class="sxs-lookup"><span data-stu-id="65ca9-144">This example uses the `Prefer: outlook.timezone` header to specify displaying date-time properties in the response in Pacific Standard Time.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MHgwAAA=')
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="65ca9-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="65ca9-145">Response</span></span>

<span data-ttu-id="65ca9-146">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="65ca9-146">Here is an example of the response.</span></span> <span data-ttu-id="65ca9-147">Die Datum-Uhrzeit-Eigenschaften in der Antwort werden in der angegebenen Pacific Standard Time angezeigt.</span><span class="sxs-lookup"><span data-stu-id="65ca9-147">The date-time properties in the response are displayed in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="65ca9-p108">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="65ca9-p108">**Note:** The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 576

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [ ],
  "assignedTo": "Dana Swope",
  "body": {
    "contentType": "text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-05-04T021:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "hasAttachments":false,
  "importance": "normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "normal",
  "startDateTime": {
    "dateTime": "2016-05-02T21:00:00.0000000",
    "timeZone": "Pacific Standard Time"
  },
  "status": "notStarted",
  "subject": "Shop for children's weekend"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
