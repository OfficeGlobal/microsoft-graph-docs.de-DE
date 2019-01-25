---
title: Erstellen von outlookTask
description: Erstellen Sie eine Outlook-Aufgabe in der Standardgruppe Aufgabe (`My Tasks`) und Aufgabe Standardordner (`Tasks`) in das Postfach des Benutzers.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 935732e14f7e467e3094d4a5a2f82d2922020569
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520991"
---
# <a name="create-outlooktask"></a><span data-ttu-id="5f571-103">Erstellen von outlookTask</span><span class="sxs-lookup"><span data-stu-id="5f571-103">Create outlookTask</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f571-104">Erstellen Sie eine Outlook-Aufgabe in der Standardgruppe Aufgabe (`My Tasks`) und Aufgabe Standardordner (`Tasks`) in das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="5f571-104">Create an Outlook task in the default task group (`My Tasks`) and default task folder (`Tasks`) in the user's mailbox.</span></span>

<span data-ttu-id="5f571-105">Die POST-Methode immer den Zeitbereich des **StartDateTime** und **DueDateTime** im Textkörper Anforderung ignoriert, und dann wird die Zeit in der angegebenen Zeitzone Mitternacht, vorausgesetzt.</span><span class="sxs-lookup"><span data-stu-id="5f571-105">The POST method always ignores the time portion of **startDateTime** and **dueDateTime** in the request body, and assumes the time to be always midnight in the specified time zone.</span></span>

<span data-ttu-id="5f571-106">Standardmäßig wird dieses Vorgangs (und die GET, PATCH und [Abschließen von](../api/outlooktask-complete.md) Aufgabe Vorgänge) datumsspezifische Eigenschaften in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f571-106">By default, this operation (and the GET, PATCH, and [complete](../api/outlooktask-complete.md) task operations) returns date-related properties in UTC.</span></span> <span data-ttu-id="5f571-107">Sie können mit dem `Prefer: outlook.timezone`-Header alle datumsbezogenen Eigenschaften in der Antwort in einer anderen Zeitzone als UTC darstellen.</span><span class="sxs-lookup"><span data-stu-id="5f571-107">You can use the `Prefer: outlook.timezone` header to have all the date-related properties in the response represented in a time zone different than UTC.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f571-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5f571-108">Permissions</span></span>
<span data-ttu-id="5f571-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5f571-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f571-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5f571-111">Permission type</span></span>      | <span data-ttu-id="5f571-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5f571-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f571-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5f571-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5f571-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f571-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="5f571-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5f571-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f571-116">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5f571-116">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="5f571-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5f571-117">Application</span></span> | <span data-ttu-id="5f571-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5f571-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f571-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f571-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/tasks
```
## <a name="request-headers"></a><span data-ttu-id="5f571-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5f571-120">Request headers</span></span>
| <span data-ttu-id="5f571-121">Name</span><span class="sxs-lookup"><span data-stu-id="5f571-121">Name</span></span>       | <span data-ttu-id="5f571-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5f571-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="5f571-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f571-123">Authorization</span></span>  | <span data-ttu-id="5f571-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5f571-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5f571-126">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="5f571-126">Prefer: outlook.timezone</span></span> | <span data-ttu-id="5f571-127">Gibt die Zeitzone für Zeiteigenschaften in der Antwort, die in UTC wäre, wenn diese Kopfzeile nicht angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="5f571-127">Specifies the time zone for time properties in the response, which would be in UTC if this header is not specified.</span></span> <span data-ttu-id="5f571-128">Optional.</span><span class="sxs-lookup"><span data-stu-id="5f571-128">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f571-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5f571-129">Request body</span></span>
<span data-ttu-id="5f571-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTask](../resources/outlooktask.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f571-130">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5f571-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f571-131">Response</span></span>

<span data-ttu-id="5f571-132">Wenn der Vorgang erfolgreich war, gibt diese Methode `201 Created` Antwortobjekt Code und [OutlookTask](../resources/outlooktask.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="5f571-132">If successful, this method returns `201 Created` response code and [outlookTask](../resources/outlooktask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f571-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5f571-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5f571-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5f571-134">Request</span></span>
<span data-ttu-id="5f571-135">Das folgende Beispiel zeigt die Verwendung von der `Prefer: outlook.timezone` Kopfzeile.</span><span class="sxs-lookup"><span data-stu-id="5f571-135">The following example shows the use of the `Prefer: outlook.timezone` header.</span></span> <span data-ttu-id="5f571-136">Es wird eine Aufgabe erstellt, **StartDateTime** und **DueDateTime** in Standard EST (Eastern Time) ausdrückt und umfasst eine `Prefer` Kopfzeile der Pacific Standard Time (PST).</span><span class="sxs-lookup"><span data-stu-id="5f571-136">It creates a task, expresses **startDateTime** and **dueDateTime** in Eastern Standard Time (EST), and includes a `Prefer` header of Pacific Standard Time (PST).</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/tasks
Prefer: outlook.timezone="Pacific Standard Time"
Content-type: application/json
Content-length: 276

{
  "assignedTo": "Dana Swope",
  "subject": "Shop for children's weekend",
  "startDateTime": {
      "dateTime": "2016-05-03T09:00:00",
      "timeZone": "Eastern Standard Time"
  },
  "dueDateTime":  {
      "dateTime": "2016-05-05T16:00:00",
      "timeZone": "Eastern Standard Time"
  }
}
```
<span data-ttu-id="5f571-137">Geben Sie im Textkörper Anforderung eine JSON-Darstellung des [OutlookTask](../resources/outlooktask.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="5f571-137">In the request body, supply a JSON representation of [outlookTask](../resources/outlooktask.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="5f571-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="5f571-138">Response</span></span>
<span data-ttu-id="5f571-139">Die POST-Methode ignoriert den Zeitbereich des **StartDateTime** und **DueDateTime** im Textkörper Anforderung und geht davon aus der Zeit Mitternacht in der angegebenen Zeitzone (EST) zu.</span><span class="sxs-lookup"><span data-stu-id="5f571-139">The POST method ignores the time portion of **startDateTime** and **dueDateTime** in the request body and assumes the time to be always midnight in the specified time zone (EST).</span></span>

<span data-ttu-id="5f571-140">Da der `Prefer`-Header PST angibt, drückt die POST-Methode alle datumsbezogenen Eigenschaften in der Antwort in PST aus.</span><span class="sxs-lookup"><span data-stu-id="5f571-140">Since the `Prefer` header specifies PST, the POST method expresses all the date-related properties in the response in PST.</span></span> <span data-ttu-id="5f571-141">Insbesondere für die Eigenschaften **StartDateTime** und **DueDateTime** konvertiert die POST-Methode Mitternacht in EST in PST und gibt sie in der Antwort in PST zurück.</span><span class="sxs-lookup"><span data-stu-id="5f571-141">In particular, for the **startDateTime** and **dueDateTime** properties, the POST method converts midnight in EST to PST and returns them in PST in the response.</span></span>

<span data-ttu-id="5f571-p107">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5f571-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
} -->
```http
HTTP/1.1 201 Created
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
    "contentType": "Text",
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
  "sensitivity": "Normal",
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
  "description": "Create outlookTask",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookuser-post-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
