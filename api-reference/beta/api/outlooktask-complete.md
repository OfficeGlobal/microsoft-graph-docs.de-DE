---
title: 'OutlookTask: abgeschlossen'
description: 'Führen Sie eine Outlook-Aufgabe, die die **CompletedDateTime** -Eigenschaft auf das aktuelle Datum festgelegt wird, '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 966f5c2a6d429169cff3bd6746ebb0bace34ad15
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979635"
---
# <a name="outlooktask-complete"></a><span data-ttu-id="2fb3e-103">OutlookTask: abgeschlossen</span><span class="sxs-lookup"><span data-stu-id="2fb3e-103">outlookTask: complete</span></span>

> <span data-ttu-id="2fb3e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fb3e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2fb3e-106">Führen Sie eine Outlook-Aufgabe, die die **CompletedDateTime** -Eigenschaft auf das aktuelle Datum und die **Status** -Eigenschaft festlegt `completed`.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-106">Complete an Outlook task which sets the **completedDateTime** property to the current date, and the **status** property to `completed`.</span></span>

<span data-ttu-id="2fb3e-107">Wenn Sie eine Aufgabe in einer Terminserie in der Antwort durchführen wird die Auflistung der abgeschlossenen Aufgabe in der Datenreihe und die nächste Aufgabe in der Datenreihe enthalten.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-107">If you are completing a task in a recurring series, in the response, the task collection will contain the completed task in the series, and the next task in the series.</span></span>

<span data-ttu-id="2fb3e-108">Die **CompletedDateTime** -Eigenschaft gibt das Datum an, wenn die Aufgabe abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-108">The **completedDateTime** property represents the date when the task is finished.</span></span> <span data-ttu-id="2fb3e-109">Den Zeitbereich des **CompletedDateTime** ist standardmäßig auf Mitternacht UTC festgelegt.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-109">The time portion of **completedDateTime** is set to midnight UTC by default.</span></span>

<span data-ttu-id="2fb3e-110">Standardmäßig wird dieses Vorgangs (und die POST-, Get- und PATCH Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-110">By default, this operation (and the POST, GET, and PATCH task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="2fb3e-111">Sie können mit dem `Prefer: outlook.timezone`-Header alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darstellen.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-111">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fb3e-112">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2fb3e-112">Permissions</span></span>

<span data-ttu-id="2fb3e-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fb3e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fb3e-115">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2fb3e-115">Permission type</span></span>      | <span data-ttu-id="2fb3e-116">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2fb3e-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fb3e-117">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2fb3e-117">Delegated (work or school account)</span></span> | <span data-ttu-id="2fb3e-118">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fb3e-118">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="2fb3e-119">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2fb3e-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fb3e-120">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2fb3e-120">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="2fb3e-121">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2fb3e-121">Application</span></span> | <span data-ttu-id="2fb3e-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2fb3e-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fb3e-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2fb3e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/outlook/tasks/{id}/complete
POST /users/{id|userPrincipalName}/outlook/tasks/{id}/complete
```

## <a name="request-headers"></a><span data-ttu-id="2fb3e-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2fb3e-124">Request headers</span></span>

| <span data-ttu-id="2fb3e-125">Name</span><span class="sxs-lookup"><span data-stu-id="2fb3e-125">Name</span></span>       | <span data-ttu-id="2fb3e-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2fb3e-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2fb3e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fb3e-127">Authorization</span></span>  | <span data-ttu-id="2fb3e-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2fb3e-130">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="2fb3e-130">Prefer: outlook.timezone</span></span> | <span data-ttu-id="2fb3e-131">Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-131">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="2fb3e-132">Optional.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-132">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fb3e-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2fb3e-133">Request body</span></span>

<span data-ttu-id="2fb3e-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2fb3e-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2fb3e-135">Response</span></span>

<span data-ttu-id="2fb3e-136">Wenn der Vorgang erfolgreich war, gibt diese Methode `200 OK` Antwortcode und des [OutlookTask](../resources/outlooktask.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-136">If successful, this method returns `200 OK` response code and the [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fb3e-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2fb3e-137">Example</span></span>

<span data-ttu-id="2fb3e-138">Das folgende Beispiel kennzeichnet die angegebene Aufgabe als erledigt.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-138">The following example marks the specified task as complete.</span></span> <span data-ttu-id="2fb3e-139">Es gibt Pacific Standard Time (PST) in der `Prefer: outlook.timezone` Kopfzeile.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-139">It specifies Pacific Standard Time (PST) in the `Prefer: outlook.timezone` header.</span></span>

### <a name="request"></a><span data-ttu-id="2fb3e-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2fb3e-140">Request</span></span>

<span data-ttu-id="2fb3e-141">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}-->

```http
POST https://graph.microsoft.com/beta/me/tasks('AAMkADA1MT15rfAAA=')/complete
Prefer: outlook.timezone="Pacific Standard Time"
```

### <a name="response"></a><span data-ttu-id="2fb3e-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="2fb3e-142">Response</span></span>

<span data-ttu-id="2fb3e-143">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-143">Here is an example of the response.</span></span> <span data-ttu-id="2fb3e-144">Die **CompletedDateTime** und andere Eigenschaften datumsspezifische in der Antwort werden in PST-Datei angegeben.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-144">The **completedDateTime** and other date-related properties in the response are expressed in PST.</span></span>

> <span data-ttu-id="2fb3e-145">**Hinweis:** Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-145">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2fb3e-146">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2fb3e-146">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "outlookTask: complete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
