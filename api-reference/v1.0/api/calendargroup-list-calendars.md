---
title: Kalender auflisten
description: Mit dieser API können Sie eine Liste der zu einer Kalendergruppe gehörenden Kalender abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5852e43e32b58a714e44dcbcad2a77e3f1999bf9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27922935"
---
# <a name="list-calendars"></a><span data-ttu-id="96adf-103">Kalender auflisten</span><span class="sxs-lookup"><span data-stu-id="96adf-103">List calendars</span></span>

<span data-ttu-id="96adf-104">Mit dieser API können Sie eine Liste der zu einer Kalendergruppe gehörenden Kalender abrufen.</span><span class="sxs-lookup"><span data-stu-id="96adf-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="96adf-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="96adf-105">Permissions</span></span>

<span data-ttu-id="96adf-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96adf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96adf-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96adf-108">Permission type</span></span>                        | <span data-ttu-id="96adf-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96adf-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="96adf-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96adf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="96adf-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="96adf-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="96adf-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96adf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96adf-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="96adf-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="96adf-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96adf-114">Application</span></span>                            | <span data-ttu-id="96adf-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="96adf-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="96adf-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96adf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="96adf-117">Die standardmäßige [CalendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="96adf-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="96adf-118">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="96adf-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96adf-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="96adf-119">Optional query parameters</span></span>

<span data-ttu-id="96adf-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="96adf-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="96adf-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96adf-121">Request headers</span></span>

| <span data-ttu-id="96adf-122">Name</span><span class="sxs-lookup"><span data-stu-id="96adf-122">Name</span></span>          | <span data-ttu-id="96adf-123">Typ</span><span class="sxs-lookup"><span data-stu-id="96adf-123">Type</span></span>   | <span data-ttu-id="96adf-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96adf-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="96adf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="96adf-125">Authorization</span></span> | <span data-ttu-id="96adf-126">string</span><span class="sxs-lookup"><span data-stu-id="96adf-126">string</span></span> | <span data-ttu-id="96adf-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="96adf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96adf-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96adf-129">Request body</span></span>

<span data-ttu-id="96adf-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="96adf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96adf-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="96adf-131">Response</span></span>

<span data-ttu-id="96adf-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Calendar](../resources/calendar.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96adf-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96adf-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96adf-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="96adf-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96adf-134">Request</span></span>

<span data-ttu-id="96adf-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96adf-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="96adf-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="96adf-136">Response</span></span>

<span data-ttu-id="96adf-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96adf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 147

{
  "value": [
    {
      "name": "name-value",
      "color": {
      },
      "changeKey": "changeKey-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
