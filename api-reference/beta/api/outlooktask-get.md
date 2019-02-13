---
title: Get outlookTask
description: Abrufen der Eigenschaften und Beziehungen einer Outlook-Aufgabe im Postfach des Benutzers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: f140734b6e5fa3e6488b71dbe183a9e3d82fc795
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967291"
---
# <a name="get-outlooktask"></a><span data-ttu-id="04314-103">Get outlookTask</span><span class="sxs-lookup"><span data-stu-id="04314-103">Get outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04314-104">Abrufen der Eigenschaften und Beziehungen einer Outlook-Aufgabe im Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="04314-104">Get the properties and relationships of an Outlook task in the user's mailbox.</span></span>

<span data-ttu-id="04314-105">Standardmäßig wird dieses Vorgangs (und die POST, PATCH und [Abschließen von](../api/outlooktask-complete.md) Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04314-105">By default, this operation (and the POST, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="04314-106">Sie können die `Prefer: outlook.timezone`-Kopfzeile verwenden, um alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darzustellen.</span><span class="sxs-lookup"><span data-stu-id="04314-106">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="04314-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="04314-107">Permissions</span></span>

<span data-ttu-id="04314-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04314-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04314-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04314-110">Permission type</span></span>                        | <span data-ttu-id="04314-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04314-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="04314-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04314-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="04314-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="04314-113">Tasks.Read</span></span>                          |
| <span data-ttu-id="04314-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04314-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04314-115">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="04314-115">Tasks.Read</span></span>                          |
| <span data-ttu-id="04314-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04314-116">Application</span></span>                            | <span data-ttu-id="04314-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="04314-117">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="04314-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04314-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/outlook/tasks/{id}
GET /users/{id|userPrincipalName}/outlook/tasks/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="04314-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="04314-119">Optional query parameters</span></span>

<span data-ttu-id="04314-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="04314-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04314-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04314-121">Request headers</span></span>

| <span data-ttu-id="04314-122">Name</span><span class="sxs-lookup"><span data-stu-id="04314-122">Name</span></span>                     | <span data-ttu-id="04314-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="04314-123">Description</span></span>                                       |
|:-------------------------|:--------------------------------------------------|
| <span data-ttu-id="04314-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="04314-124">Authorization</span></span>            | <span data-ttu-id="04314-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="04314-p103">Bearer {token}. Required.</span></span>                         |
| <span data-ttu-id="04314-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="04314-127">Prefer: outlook.timezone</span></span> | <span data-ttu-id="04314-128">Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="04314-128">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="04314-129">Optional.</span><span class="sxs-lookup"><span data-stu-id="04314-129">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04314-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04314-130">Request body</span></span>

<span data-ttu-id="04314-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="04314-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04314-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="04314-132">Response</span></span>

<span data-ttu-id="04314-133">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [OutlookTask](../resources/outlooktask.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="04314-133">If successful, this method returns a `200 OK` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04314-134">Beispiele</span><span class="sxs-lookup"><span data-stu-id="04314-134">Examples</span></span>

### <a name="example-1-get-an-outlook-task"></a><span data-ttu-id="04314-135">Beispiel 1: Abrufen einer Outlook-Aufgabenelements</span><span class="sxs-lookup"><span data-stu-id="04314-135">Example 1: Get an Outlook task</span></span>

#### <a name="request"></a><span data-ttu-id="04314-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04314-136">Request</span></span>

<span data-ttu-id="04314-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04314-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MTrgAAA=')
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="04314-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="04314-138">Response</span></span>

<span data-ttu-id="04314-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="04314-139">Here is an example of the response.</span></span> <span data-ttu-id="04314-140">Standardmäßig sind die Datums-/Uhrzeiteigenschaften in der Antwort in UTC angegeben.</span><span class="sxs-lookup"><span data-stu-id="04314-140">By default, the date-time properties in the response are in UTC.</span></span>

> <span data-ttu-id="04314-141">**Hinweis:** Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="04314-141">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="04314-142">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04314-142">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MTrgAAA=",
  "createdDateTime": "2016-04-22T06:03:35.9279794Z",
  "lastModifiedDateTime": "2016-04-22T06:03:35.9436052Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMyQ==",
  "categories": [],
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
  "hasAttachments": false,
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

### <a name="example-2-get-outlook-task-with-date-time-properties-in-pacific-standard-time"></a><span data-ttu-id="04314-143">Beispiel 2: Abrufen von Outlook-Aufgabe mit Datum-Uhrzeit-Eigenschaften in Pazifik Normalzeit</span><span class="sxs-lookup"><span data-stu-id="04314-143">Example 2: Get Outlook task with date-time properties in Pacific Standard Time</span></span>

#### <a name="request"></a><span data-ttu-id="04314-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04314-144">Request</span></span>

<span data-ttu-id="04314-145">In diesem Beispiel wird die `Prefer: outlook.timezone` Header, um anzugeben, dass die API Datum-/ Uhrzeit-Eigenschaften in der Pacific Standard Time-Antwort zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="04314-145">This example uses the `Prefer: outlook.timezone` header to specify that the API should return date-time properties in the response in Pacific Standard Time.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_outlooktask"
}-->

```http
GET https://graph.microsoft.com/beta/me/outlook/tasks('AAMkADA1MHgwAAA=')
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="04314-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="04314-146">Response</span></span>

<span data-ttu-id="04314-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="04314-147">Here is an example of the response.</span></span> <span data-ttu-id="04314-148">Die Datum-Uhrzeit-Eigenschaften in der Antwort werden in der angegebenen Pacific Standard Time zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04314-148">The date-time properties in the response are returned in the specified Pacific Standard Time.</span></span>

> <span data-ttu-id="04314-149">**Hinweis:** Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="04314-149">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="04314-150">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04314-150">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkADA1MHgwAAA=",
  "createdDateTime": "2016-04-22T15:19:18.9526004-07:00",
  "lastModifiedDateTime": "2016-04-22T15:19:19.015101-07:00",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XXA==",
  "categories": [],
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
  "hasAttachments": false,
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
