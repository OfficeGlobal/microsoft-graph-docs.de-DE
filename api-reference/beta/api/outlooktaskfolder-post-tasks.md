---
title: Erstellen von outlookTask
description: Erstellen Sie eine Outlook-Aufgabe im angegebenen Ordner.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 477ddf32b790da5b5d43560119d7a2529e773ad0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841419"
---
# <a name="create-outlooktask"></a><span data-ttu-id="2b0d6-103">Erstellen von outlookTask</span><span class="sxs-lookup"><span data-stu-id="2b0d6-103">Create outlookTask</span></span>

> <span data-ttu-id="2b0d6-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b0d6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b0d6-106">Erstellen Sie eine Outlook-Aufgabe im angegebenen Ordner.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-106">Create an Outlook task in the specified task folder.</span></span>

<span data-ttu-id="2b0d6-107">Die POST-Methode immer den Zeitbereich des **StartDateTime** und **DueDateTime** im Textkörper Anforderung ignoriert, und dann wird die Zeit in der angegebenen Zeitzone Mitternacht, vorausgesetzt.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-107">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

## <a name="permissions"></a><span data-ttu-id="2b0d6-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2b0d6-108">Permissions</span></span>
<span data-ttu-id="2b0d6-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2b0d6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b0d6-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2b0d6-111">Permission type</span></span>      | <span data-ttu-id="2b0d6-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2b0d6-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b0d6-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2b0d6-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2b0d6-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b0d6-114">Not supported.</span></span>    |
|<span data-ttu-id="2b0d6-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2b0d6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b0d6-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b0d6-116">Not supported.</span></span>    |
|<span data-ttu-id="2b0d6-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2b0d6-117">Application</span></span> | <span data-ttu-id="2b0d6-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2b0d6-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b0d6-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b0d6-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks
```
## <a name="request-headers"></a><span data-ttu-id="2b0d6-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2b0d6-120">Request headers</span></span>
| <span data-ttu-id="2b0d6-121">Name</span><span class="sxs-lookup"><span data-stu-id="2b0d6-121">Name</span></span>       | <span data-ttu-id="2b0d6-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2b0d6-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2b0d6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b0d6-123">Authorization</span></span>  | <span data-ttu-id="2b0d6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2b0d6-126">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="2b0d6-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="2b0d6-127">Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-127">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="2b0d6-128">Optional.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-128">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b0d6-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2b0d6-129">Request body</span></span>
<span data-ttu-id="2b0d6-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTask](../resources/outlooktask.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-130">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2b0d6-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b0d6-131">Response</span></span>

<span data-ttu-id="2b0d6-132">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [OutlookTask](../resources/outlooktask.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-132">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b0d6-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2b0d6-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2b0d6-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2b0d6-134">Request</span></span>
<span data-ttu-id="2b0d6-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlooktaskfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/taskfolders('AAMkADIyAAAhrbPXAAA=')/tasks
Content-type: application/json
Content-length: 376

{
  "subject": "Shop for dinner",
  "startDateTime": {
      "dateTime": "2016-04-23T18:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "dueDateTime":  {
      "dateTime": "2016-04-25T13:00:00",
      "timeZone": "Pacific Standard Time"
  }
}
```
<span data-ttu-id="2b0d6-136">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTask](../resources/outlooktask.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-136">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2b0d6-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="2b0d6-137">Response</span></span>
<span data-ttu-id="2b0d6-138">Die POST-Methode ignoriert den Zeitanteil im Anforderungstext und geht davon aus, dass die Zeit immer Mitternacht in der angegebenen Zeitzone (PST) ist.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-138">The POST method ignores the time portion in the request body and assumes the time to be always midnight in the specified time zone (PST).</span></span> <span data-ttu-id="2b0d6-139">Die POST-Methode konvertiert dann standardmäßig alle datumsbezogenen Eigenschaften in der Antwort in UTC.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-139">Then, by default, the POST method converts and shows all the date-related properties in UTC in the response.</span></span>

<span data-ttu-id="2b0d6-p106">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2b0d6-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 376

{
  "createdDateTime": "2016-04-22T05:44:01.2012012Z",
  "lastModifiedDateTime": "2016-04-22T05:44:02.9980882Z",
  "changeKey": "1/KC9Vmu40G3DwB6Lgs7MAAAIOJMxw==",
  "categories": [ ],
  "assignedTo": "null",
  "body": {
    "contentType": "Text",
    "content": ""
  },
  "completedDateTime": null,
  "dueDateTime": {
    "dateTime": "2016-04-25T07:00:00.0000000",
    "timeZone": "UTC"
  },
  "hasAttachments":false,
  "importance": "Normal",
  "isReminderOn": false,
  "owner": "Administrator",
  "parentFolderId": "AQMkADA1MTkAAAAIBEgAAAA==",
  "recurrence": null,
  "reminderDateTime": null,
  "sensitivity": "Normal",
  "startDateTime": {
    "dateTime": "2016-04-23T07:00:00.0000000",
    "timeZone": "UTC"
  },
  "status": "NotStarted",
  "subject": "Shop for dinner"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
