---
title: Ereignisse auflisten
description: Dient zum Abrufen einer Liste von Ereignisobjekten.
ms.openlocfilehash: bb79676e63cf12731a39dceb94e8a1b8b8cf2247
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061534"
---
# <a name="list-events"></a><span data-ttu-id="0504d-103">Ereignisse auflisten</span><span class="sxs-lookup"><span data-stu-id="0504d-103">List events</span></span>

> <span data-ttu-id="0504d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0504d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0504d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0504d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0504d-106">Mit dieser API können Sie eine Liste von Objekten des Typs [event](../resources/event.md) abrufen.</span><span class="sxs-lookup"><span data-stu-id="0504d-106">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0504d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0504d-107">Permissions</span></span>
<span data-ttu-id="0504d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0504d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0504d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0504d-110">Permission type</span></span>      | <span data-ttu-id="0504d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0504d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0504d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0504d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0504d-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0504d-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0504d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0504d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0504d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0504d-115">Not supported.</span></span>    |
|<span data-ttu-id="0504d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0504d-116">Application</span></span> | <span data-ttu-id="0504d-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0504d-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0504d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0504d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0504d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0504d-119">Optional query parameters</span></span>
<span data-ttu-id="0504d-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query-parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0504d-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0504d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0504d-121">Request headers</span></span>
| <span data-ttu-id="0504d-122">Name</span><span class="sxs-lookup"><span data-stu-id="0504d-122">Name</span></span>       | <span data-ttu-id="0504d-123">Typ</span><span class="sxs-lookup"><span data-stu-id="0504d-123">Type</span></span> | <span data-ttu-id="0504d-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0504d-124">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="0504d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0504d-125">Authorization</span></span>  | <span data-ttu-id="0504d-126">string</span><span class="sxs-lookup"><span data-stu-id="0504d-126">string</span></span> | <span data-ttu-id="0504d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0504d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0504d-129">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="0504d-129">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="0504d-130">string</span><span class="sxs-lookup"><span data-stu-id="0504d-130">string</span></span> | <span data-ttu-id="0504d-131">Verwenden Sie dies, um die Zeitzone für die Anfangs- und Endzeiten in der Antwort anzugeben.</span><span class="sxs-lookup"><span data-stu-id="0504d-131">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="0504d-132">Wenn nicht angegeben, werden diese Zeitwerte in UTC zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0504d-132">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="0504d-133">Optional.</span><span class="sxs-lookup"><span data-stu-id="0504d-133">Optional.</span></span> |
| <span data-ttu-id="0504d-134">Besser: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="0504d-134">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="0504d-135">string</span><span class="sxs-lookup"><span data-stu-id="0504d-135">string</span></span> | <span data-ttu-id="0504d-136">Das Format, in der die **body**-Eigenschaft zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="0504d-136">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="0504d-137">Werte können „Text“ oder „html“ sein.</span><span class="sxs-lookup"><span data-stu-id="0504d-137">Values can be "text" or "html".</span></span> <span data-ttu-id="0504d-138">Als Bestätigung wird eine `Preference-Applied`-Kopfzeile zurückgegeben, wenn diese `Prefer`-Kopfzeile angegeben ist.</span><span class="sxs-lookup"><span data-stu-id="0504d-138">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="0504d-139">Wenn die Kopfzeile nicht angegeben ist, wird die **body**-Eigenschaft im HTML-Format zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0504d-139">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="0504d-140">Optional.</span><span class="sxs-lookup"><span data-stu-id="0504d-140">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0504d-141">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0504d-141">Request body</span></span>
<span data-ttu-id="0504d-142">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0504d-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0504d-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="0504d-143">Response</span></span>
<span data-ttu-id="0504d-144">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [event](../resources/event.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0504d-144">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0504d-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0504d-145">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0504d-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0504d-146">Request</span></span>
<span data-ttu-id="0504d-147">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0504d-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/events
```

#### <a name="response"></a><span data-ttu-id="0504d-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="0504d-148">Response</span></span>
<span data-ttu-id="0504d-149">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0504d-149">The following is an example of the response.</span></span>
><span data-ttu-id="0504d-150">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="0504d-150">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0504d-151">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0504d-151">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List group events",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
