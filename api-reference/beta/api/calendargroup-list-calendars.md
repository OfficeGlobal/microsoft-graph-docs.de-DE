---
title: Kalender auflisten
description: Mit dieser API können Sie eine Liste der zu einer Kalendergruppe gehörenden Kalender abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 9ffa22a25fcc5c42ca9a61ea09a5cc68d2f3351b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814203"
---
# <a name="list-calendars"></a><span data-ttu-id="40146-103">Kalender auflisten</span><span class="sxs-lookup"><span data-stu-id="40146-103">List calendars</span></span>

> <span data-ttu-id="40146-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="40146-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="40146-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="40146-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="40146-106">Mit dieser API können Sie eine Liste der zu einer Kalendergruppe gehörenden Kalender abrufen.</span><span class="sxs-lookup"><span data-stu-id="40146-106">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="40146-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="40146-107">Permissions</span></span>

<span data-ttu-id="40146-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40146-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="40146-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="40146-110">Permission type</span></span>                        | <span data-ttu-id="40146-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="40146-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="40146-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="40146-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="40146-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="40146-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="40146-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="40146-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="40146-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="40146-115">Calendars.Read</span></span>                              |
| <span data-ttu-id="40146-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="40146-116">Application</span></span>                            | <span data-ttu-id="40146-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="40146-117">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="40146-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="40146-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="40146-119">Die standardmäßige [CalendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="40146-119">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="40146-120">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="40146-120">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40146-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="40146-121">Optional query parameters</span></span>

<span data-ttu-id="40146-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="40146-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="40146-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="40146-123">Request headers</span></span>

| <span data-ttu-id="40146-124">Name</span><span class="sxs-lookup"><span data-stu-id="40146-124">Name</span></span>          | <span data-ttu-id="40146-125">Typ</span><span class="sxs-lookup"><span data-stu-id="40146-125">Type</span></span>   | <span data-ttu-id="40146-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="40146-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="40146-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="40146-127">Authorization</span></span> | <span data-ttu-id="40146-128">string</span><span class="sxs-lookup"><span data-stu-id="40146-128">string</span></span> | <span data-ttu-id="40146-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="40146-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40146-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="40146-131">Request body</span></span>

<span data-ttu-id="40146-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="40146-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40146-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="40146-133">Response</span></span>

<span data-ttu-id="40146-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Calendar](../resources/calendar.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40146-134">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40146-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="40146-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="40146-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="40146-136">Request</span></span>

<span data-ttu-id="40146-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="40146-137">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="40146-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="40146-138">Response</span></span>

<span data-ttu-id="40146-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="40146-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
