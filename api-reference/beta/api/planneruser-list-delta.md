---
title: 'Planner: Delta'
description: Ruft die Änderungen an-Objekten, denen der Benutzer abonniert ist.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 772a5d487f48b1552707da45729a84c7fdf7da2f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525724"
---
# <a name="planner-delta"></a><span data-ttu-id="7f4ee-103">Planner: Delta</span><span class="sxs-lookup"><span data-stu-id="7f4ee-103">Planner: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f4ee-104">Ruft die Änderungen für Objekte, denen der Benutzer [angemeldet](../resources/planner-overview.md#track-changes-using-delta-query) ist.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-104">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="7f4ee-105">Mit dieser Methode können die Anwendung zum Nachverfolgen von Änderungen auf Objekte, die der Benutzer über einen Zeitraum von in Planner zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-105">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="7f4ee-106">Der Rückgabewert dieser Methode kann heterogenes Typen von Objekten aus Planner enthalten.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-106">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="7f4ee-107">Weitere Informationen zum Nachverfolgen von Änderungen in Microsoft Graph-Daten finden Sie unter [Verwendung Delta-Abfrage zum Nachverfolgen von Änderungen in Microsoft Graph-Daten](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="7f4ee-107">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="7f4ee-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7f4ee-108">Permissions</span></span>

<span data-ttu-id="7f4ee-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f4ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f4ee-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7f4ee-111">Permission type</span></span>      | <span data-ttu-id="7f4ee-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7f4ee-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f4ee-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7f4ee-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7f4ee-114">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f4ee-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7f4ee-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7f4ee-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f4ee-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f4ee-116">Not supported.</span></span>    |
|<span data-ttu-id="7f4ee-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7f4ee-117">Application</span></span> | <span data-ttu-id="7f4ee-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7f4ee-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f4ee-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f4ee-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/<id>/planner/all/delta
```

<span data-ttu-id="7f4ee-120">Keine zusätzlichen Abfrageparametern (z. B. `$select`, `$expand`, oder `$filter`) werden derzeit Planner Implementierung der Delta-Abfragen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-120">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f4ee-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7f4ee-121">Request headers</span></span>

| <span data-ttu-id="7f4ee-122">Name</span><span class="sxs-lookup"><span data-stu-id="7f4ee-122">Name</span></span>           |<span data-ttu-id="7f4ee-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7f4ee-123">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="7f4ee-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f4ee-124">Authorization</span></span>  | <span data-ttu-id="7f4ee-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f4ee-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7f4ee-127">Request body</span></span>

<span data-ttu-id="7f4ee-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f4ee-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f4ee-129">Response</span></span>

<span data-ttu-id="7f4ee-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eine Auflistung von Änderungen auf Objekte in der Antworttext und einen Link Delta Sync, denen Sie folgen angewendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-130">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="7f4ee-131">Wenn die `deltaLink` , dass der Anrufer verwendet ist falsch formatiert, diesen Endpunkt HTTP 400 zurück.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-131">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="7f4ee-132">Wenn die `deltaLink` , dass der Anrufer verwendet ist veraltet, diesen Endpunkt HTTP 410 zurück.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-132">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="7f4ee-p103">Diese Methode kann einen beliebigen [HTTP-Statuscode](/graph/errors) zurückgeben. Die häufigsten Fehler, die Apps für diese Methode behandeln sollten, sind die Antworten 403 und 404. Weitere Informationen zu diesen Fehlern finden Sie unter [Häufige Planner-Fehlerbedingungen](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="7f4ee-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="7f4ee-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7f4ee-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7f4ee-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7f4ee-137">Request</span></span>

<span data-ttu-id="7f4ee-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-138">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```http
GET https://graph.microsoft.com/beta/me/planner/all/delta
```

##### <a name="response"></a><span data-ttu-id="7f4ee-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="7f4ee-139">Response</span></span>
<span data-ttu-id="7f4ee-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-140">Here is an example of the response.</span></span>

><span data-ttu-id="7f4ee-141">**Hinweis:** Das gezeigte Antwortobjekt wurde möglicherweise zur besseren Lesbarkeit gekürzt.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-141">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="7f4ee-142">Alle geänderten Eigenschaften werden von einem tatsächlichen Aufruf zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7f4ee-142">All the changed properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List changes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
