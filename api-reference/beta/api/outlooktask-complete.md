---
title: 'OutlookTask: abgeschlossen'
description: 'Führen Sie eine Outlook-Aufgabe, die die **CompletedDateTime** -Eigenschaft auf das aktuelle Datum festgelegt wird, '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: de3d47d59b89f8bbef42b8b17a9099ecf9e80c98
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513557"
---
# <a name="outlooktask-complete"></a><span data-ttu-id="1e247-103">OutlookTask: abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="1e247-103">outlookTask: complete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e247-104">Führen Sie eine Outlook-Aufgabe, die die **CompletedDateTime** -Eigenschaft auf das aktuelle Datum und die **Status** -Eigenschaft festlegt `completed`.</span><span class="sxs-lookup"><span data-stu-id="1e247-104">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="1e247-105">Wenn Sie eine Aufgabe in einer Terminserie in der Antwort durchführen wird die Auflistung der abgeschlossenen Aufgabe in der Datenreihe und die nächste Aufgabe in der Datenreihe enthalten.</span><span class="sxs-lookup"><span data-stu-id="1e247-105">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="1e247-106">Die **CompletedDateTime** -Eigenschaft gibt das Datum an, wenn die Aufgabe abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="1e247-106">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="1e247-107">Den Zeitbereich des **CompletedDateTime** ist standardmäßig auf Mitternacht UTC festgelegt.</span><span class="sxs-lookup"><span data-stu-id="1e247-107">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="1e247-108">Standardmäßig wird dieses Vorgangs (und die POST-, Get- und PATCH Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e247-108">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="1e247-109">Sie können mit dem `Prefer: outlook.timezone`-Header alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darstellen.</span><span class="sxs-lookup"><span data-stu-id="1e247-109">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e247-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1e247-110">Permissions</span></span>

<span data-ttu-id="1e247-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e247-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e247-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1e247-113">Permission type</span></span>      | <span data-ttu-id="1e247-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1e247-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e247-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1e247-115">Delegated (work or school account)</span></span> | <span data-ttu-id="1e247-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e247-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1e247-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1e247-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e247-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e247-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="1e247-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1e247-119">Application</span></span> | <span data-ttu-id="1e247-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1e247-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e247-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e247-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="1e247-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1e247-122">Request headers</span></span>

| <span data-ttu-id="1e247-123">Name</span><span class="sxs-lookup"><span data-stu-id="1e247-123">Name</span></span>       | <span data-ttu-id="1e247-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1e247-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1e247-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e247-125">Authorization</span></span>  | <span data-ttu-id="1e247-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1e247-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1e247-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="1e247-128">Prefer: outlook.timezone</span></span> | <span data-ttu-id="1e247-129">Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="1e247-129">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="1e247-130">Optional.</span><span class="sxs-lookup"><span data-stu-id="1e247-130">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e247-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1e247-131">Request body</span></span>

<span data-ttu-id="1e247-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1e247-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e247-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e247-133">Response</span></span>

<span data-ttu-id="1e247-134">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und des [OutlookTask](../resources/outlooktask.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="1e247-134">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e247-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1e247-135">Example</span></span>

<span data-ttu-id="1e247-136">Das folgende Beispiel kennzeichnet die angegebene Aufgabe als erledigt.</span><span class="sxs-lookup"><span data-stu-id="1e247-136">The following example marks the specified task as complete.</span></span> <span data-ttu-id="1e247-137">Es gibt Pacific Standard Time (PST) in der `Prefer: outlook.timezone` Kopfzeile.</span><span class="sxs-lookup"><span data-stu-id="1e247-137">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="1e247-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1e247-138">Request</span></span>

<span data-ttu-id="1e247-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1e247-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="1e247-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="1e247-140">Response</span></span>

<span data-ttu-id="1e247-141">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1e247-141">Here is an example of the response.</span></span> <span data-ttu-id="1e247-142">Die **CompletedDateTime** und andere Eigenschaften datumsspezifische in der Antwort werden in PST-Datei angegeben.</span><span class="sxs-lookup"><span data-stu-id="1e247-142">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="1e247-p108">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1e247-p108">**Note:** The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "AAMkADA1MT15rfAAA=",
      "createdDateTime": "2016-04-21T22:44:01.2012012-07:00",
      "lastModifiedDateTime": "2016-04-22T19:28:38.5300447-07:00",
      "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIW9XYQ==",
      "categories": [
      ],
      "assignedTo": null,
      "body": {
          "contentType": "text",
          "content": ""
      },
      "completedDateTime": {
          "dateTime": "2016-04-22T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "dueDateTime": {
          "dateTime": "2016-04-25T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "hasAttachments":false,
      "importance": "normal",
      "isReminderOn": false,
      "owner": "Administrator",
      "parentFolderId": "AQMkADA1MTIBEgAAAA==",
      "recurrence": null,
      "reminderDateTime": null,
      "sensitivity": "normal",
      "startDateTime": {
          "dateTime": "2016-04-21T00:00:00.0000000",
          "timeZone": "Pacific Standard Time"
      },
      "status": "completed",
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
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktask-complete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
