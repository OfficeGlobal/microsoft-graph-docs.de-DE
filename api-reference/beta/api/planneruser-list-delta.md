---
title: 'Planner: Delta'
description: Ruft die Änderungen an-Objekten, denen der Benutzer abonniert ist.
ms.openlocfilehash: 7c866946f0c9a873b99ee4efd6d9e2c7ce646be3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063492"
---
# <a name="planner-delta"></a><span data-ttu-id="a6400-103">Planner: Delta</span><span class="sxs-lookup"><span data-stu-id="a6400-103">Planner: delta</span></span>

> <span data-ttu-id="a6400-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a6400-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6400-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6400-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6400-106">Ruft die Änderungen für Objekte, denen der Benutzer [angemeldet](../resources/planner-overview.md#track-changes-using-delta-query) ist.</span><span class="sxs-lookup"><span data-stu-id="a6400-106">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="a6400-107">Mit dieser Methode können die Anwendung zum Nachverfolgen von Änderungen auf Objekte, die der Benutzer über einen Zeitraum von in Planner zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="a6400-107">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="a6400-108">Der Rückgabewert dieser Methode kann heterogenes Typen von Objekten aus Planner enthalten.</span><span class="sxs-lookup"><span data-stu-id="a6400-108">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="a6400-109">Weitere Informationen zum Nachverfolgen von Änderungen in Microsoft Graph-Daten finden Sie unter [Verwendung Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="a6400-109">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="a6400-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a6400-110">Permissions</span></span>

<span data-ttu-id="a6400-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6400-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6400-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a6400-113">Permission type</span></span>      | <span data-ttu-id="a6400-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a6400-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6400-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a6400-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a6400-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6400-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6400-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a6400-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6400-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6400-118">Not supported.</span></span>    |
|<span data-ttu-id="a6400-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a6400-119">Application</span></span> | <span data-ttu-id="a6400-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a6400-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6400-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6400-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/<id>/planner/all/delta
```

<span data-ttu-id="a6400-122">Keine zusätzlichen Abfrageparametern (z. B. `$select`, `$expand`, oder `$filter`) werden derzeit Planner Implementierung der Delta-Abfragen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a6400-122">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6400-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a6400-123">Request headers</span></span>

| <span data-ttu-id="a6400-124">Name</span><span class="sxs-lookup"><span data-stu-id="a6400-124">Name</span></span>           |<span data-ttu-id="a6400-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a6400-125">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="a6400-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6400-126">Authorization</span></span>  | <span data-ttu-id="a6400-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a6400-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6400-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a6400-129">Request body</span></span>

<span data-ttu-id="a6400-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a6400-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6400-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6400-131">Response</span></span>

<span data-ttu-id="a6400-132">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Änderungen auf Objekte in der Antworttext und einen Link Delta Sync, denen Sie folgen angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="a6400-132">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="a6400-133">Wenn die `deltaLink` , dass der Anrufer verwendet ist falsch formatiert, diesen Endpunkt HTTP 400 zurück.</span><span class="sxs-lookup"><span data-stu-id="a6400-133">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="a6400-134">Wenn die `deltaLink` , dass der Anrufer verwendet ist veraltet, diesen Endpunkt HTTP 410 zurück.</span><span class="sxs-lookup"><span data-stu-id="a6400-134">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="a6400-p104">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="a6400-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="a6400-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a6400-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a6400-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6400-139">Request</span></span>

<span data-ttu-id="a6400-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a6400-140">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```http
GET https://graph.microsoft.com/beta/me/planner/all/delta
```

##### <a name="response"></a><span data-ttu-id="a6400-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6400-141">Response</span></span>
<span data-ttu-id="a6400-142">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a6400-142">Here is an example of the response.</span></span>

><span data-ttu-id="a6400-143">**Hinweis:** Das Antwortobjekt dargestellt möglicherweise zur besseren Lesbarkeit wurde verkürzt werden.</span><span class="sxs-lookup"><span data-stu-id="a6400-143">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="a6400-144">Alle geänderten Eigenschaften werden von einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6400-144">All the changed properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_delta",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.entity)",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
cache-control: private
client-request-id: 3acb384b-e2d1-4a46-a347-e03bc6428cac
request-id: 3acb384b-e2d1-4a46-a347-e03bc6428cac
preference-applied: odata.track-changes, odata.track-changes

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.plannerDelta)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/me/planner/all/delta?$deltatoken=jVztGMFnm7qLEQ69FaXzWF5sPEJZU2YxZa32QEvnZTZ4q4C10ThM5uL7bEPm9ysqrxOY0QQIb4Uqmc9DH3rn7pczamvtCipDVJ4FivXh398.J9pSVKpytlutvx03-iBmO4ZM_3qPztOq2T9VIjHoRR0",
    "value": [
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBASCc=\"",
            "percentComplete": 100,
            "completedDateTime": "2018-03-13T21:31:25.778Z",
            "completedBy": {
                "user": {
                    "id": "8414b634-316f-41ba-b6a6-646a2949e3a5"
                }
            },
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        },
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBATCc=\"",
            "percentComplete": 0,
            "completedDateTime": null,
            "completedBy": null,
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        },
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAUCc=\"",
            "title": "Title change",
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List changes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
