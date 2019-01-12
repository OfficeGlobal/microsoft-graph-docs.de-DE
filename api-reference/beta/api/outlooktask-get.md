---
title: Abrufen von outlookTask
description: Rufen Sie die Eigenschaften und Beziehungen zwischen Outlook-Aufgaben in das Postfach des Benutzers an.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 680d27e647fdc5dd8162133c21c54276c532e939
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969135"
---
# <a name="get-outlooktask"></a><span data-ttu-id="19395-103">Abrufen von outlookTask</span><span class="sxs-lookup"><span data-stu-id="19395-103">Get outlookTask</span></span>

> <span data-ttu-id="19395-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="19395-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19395-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="19395-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19395-106">Rufen Sie die Eigenschaften und Beziehungen zwischen Outlook-Aufgaben in das Postfach des Benutzers an.</span><span class="sxs-lookup"><span data-stu-id="19395-106">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="19395-107">Standardmäßig wird dieses Vorgangs (und die POST, PATCH und [Abschließen von](../api/outlooktask-complete.md) Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19395-107">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="19395-108">Sie können mit dem `Prefer: outlook.timezone`-Header alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darstellen.</span><span class="sxs-lookup"><span data-stu-id="19395-108">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="19395-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="19395-109">Permissions</span></span>

<span data-ttu-id="19395-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="19395-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19395-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="19395-112">Permission type</span></span>      | <span data-ttu-id="19395-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="19395-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19395-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="19395-114">Delegated (work or school account)</span></span> | <span data-ttu-id="19395-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="19395-115">Tasks.Read</span></span>    |
|<span data-ttu-id="19395-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="19395-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19395-117">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="19395-117">Tasks.Read</span></span>    |
|<span data-ttu-id="19395-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="19395-118">Application</span></span> | <span data-ttu-id="19395-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="19395-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19395-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="19395-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="19395-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="19395-121">Optional query parameters</span></span>

<span data-ttu-id="19395-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="19395-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19395-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="19395-123">Request headers</span></span>

| <span data-ttu-id="19395-124">Name</span><span class="sxs-lookup"><span data-stu-id="19395-124">Name</span></span>      |<span data-ttu-id="19395-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="19395-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19395-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="19395-126">Authorization</span></span>  | <span data-ttu-id="19395-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="19395-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19395-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="19395-129">Prefer: outlook.timezone</span></span> | <span data-ttu-id="19395-130">Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="19395-130">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="19395-131">Optional.</span><span class="sxs-lookup"><span data-stu-id="19395-131">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="19395-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="19395-132">Request body</span></span>

<span data-ttu-id="19395-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="19395-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19395-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="19395-134">Response</span></span>

<span data-ttu-id="19395-135">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [OutlookTask](../resources/outlooktask.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="19395-135">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="19395-136">Beispiel 1</span><span class="sxs-lookup"><span data-stu-id="19395-136">Example 1</span></span>

### <a name="request"></a><span data-ttu-id="19395-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19395-137">Request</span></span>

<span data-ttu-id="19395-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="19395-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTrgAAA=')
```

### <a name="response"></a><span data-ttu-id="19395-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="19395-139">Response</span></span>

<span data-ttu-id="19395-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="19395-140">Here is an example of the response.</span></span> <span data-ttu-id="19395-141">Standardmäßig sind die Datums-/Uhrzeiteigenschaften in der Antwort in UTC angegeben.</span><span class="sxs-lookup"><span data-stu-id="19395-141">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="19395-142">**Hinweis:** Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="19395-142">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="19395-143">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19395-143">All of the properties will be returned from an actual call.</span></span>
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

## <a name="example-2"></a><span data-ttu-id="19395-144">Beispiel 2</span><span class="sxs-lookup"><span data-stu-id="19395-144">Example 2</span></span>

### <a name="request"></a><span data-ttu-id="19395-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="19395-145">Request</span></span>

<span data-ttu-id="19395-146">In diesem Beispiel wird die `Prefer: outlook.timezone` Header zum Anzeigen von Datum / Uhrzeit-Eigenschaften in der Pacific Standard Time-Antwort angeben.</span><span class="sxs-lookup"><span data-stu-id="19395-146">This example uses the `Prefer: outlook.timezone` header to specify displaying date-time properties in the response in Pacific Standard Time.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MHgwAAA=')
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="19395-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="19395-147">Response</span></span>

<span data-ttu-id="19395-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="19395-148">Here is an example of the response.</span></span> <span data-ttu-id="19395-149">Die Datum-Uhrzeit-Eigenschaften in der Antwort werden in der angegebenen Pacific Standard Time angezeigt.</span><span class="sxs-lookup"><span data-stu-id="19395-149">The date-time properties in the response are displayed in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="19395-150">**Hinweis:** Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="19395-150">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="19395-151">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="19395-151">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
