---
title: Ereignisse auflisten
description: Dient zum Abrufen einer Liste von Ereignisobjekten.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: c02318a8c7a8c7a8ffc7562d4a807fa06fae47a6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525381"
---
# <a name="list-events"></a><span data-ttu-id="9ad56-103">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="9ad56-103">List events</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ad56-104">Mit dieser API können Sie eine Liste von Objekten des Typs [event](../resources/event.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="9ad56-104">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ad56-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9ad56-105">Permissions</span></span>
<span data-ttu-id="9ad56-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ad56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ad56-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9ad56-108">Permission type</span></span>      | <span data-ttu-id="9ad56-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9ad56-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ad56-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9ad56-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9ad56-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ad56-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9ad56-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9ad56-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ad56-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ad56-113">Not supported.</span></span>    |
|<span data-ttu-id="9ad56-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9ad56-114">Application</span></span> | <span data-ttu-id="9ad56-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9ad56-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ad56-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ad56-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ad56-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9ad56-117">Optional query parameters</span></span>
<span data-ttu-id="9ad56-118">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9ad56-118">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ad56-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9ad56-119">Request headers</span></span>
| <span data-ttu-id="9ad56-120">Name</span><span class="sxs-lookup"><span data-stu-id="9ad56-120">Name</span></span>       | <span data-ttu-id="9ad56-121">Typ</span><span class="sxs-lookup"><span data-stu-id="9ad56-121">Type</span></span> | <span data-ttu-id="9ad56-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ad56-122">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="9ad56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ad56-123">Authorization</span></span>  | <span data-ttu-id="9ad56-124">String</span><span class="sxs-lookup"><span data-stu-id="9ad56-124">string</span></span> | <span data-ttu-id="9ad56-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9ad56-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9ad56-127">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="9ad56-127">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="9ad56-128">string</span><span class="sxs-lookup"><span data-stu-id="9ad56-128">string</span></span> | <span data-ttu-id="9ad56-129">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="9ad56-129">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="9ad56-130">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ad56-130">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="9ad56-131">Optional.</span><span class="sxs-lookup"><span data-stu-id="9ad56-131">Optional.</span></span> |
| <span data-ttu-id="9ad56-132">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="9ad56-132">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="9ad56-133">string</span><span class="sxs-lookup"><span data-stu-id="9ad56-133">string</span></span> | <span data-ttu-id="9ad56-134">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="9ad56-134">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="9ad56-135">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="9ad56-135">Values can be "text" or "html".</span></span> <span data-ttu-id="9ad56-136">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="9ad56-136">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="9ad56-137">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ad56-137">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="9ad56-138">Optional.</span><span class="sxs-lookup"><span data-stu-id="9ad56-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ad56-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9ad56-139">Request body</span></span>
<span data-ttu-id="9ad56-140">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9ad56-140">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ad56-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ad56-141">Response</span></span>
<span data-ttu-id="9ad56-142">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9ad56-142">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ad56-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9ad56-143">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9ad56-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9ad56-144">Request</span></span>
<span data-ttu-id="9ad56-145">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9ad56-145">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```

#### <a name="response"></a><span data-ttu-id="9ad56-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="9ad56-146">Response</span></span>
<span data-ttu-id="9ad56-147">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9ad56-147">The following is an example of the response.</span></span>
><span data-ttu-id="9ad56-148">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="9ad56-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9ad56-149">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="9ad56-149">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-list-events.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
