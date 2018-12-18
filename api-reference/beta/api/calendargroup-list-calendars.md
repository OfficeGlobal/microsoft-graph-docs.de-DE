---
title: Kalender auflisten
description: Mit dieser API können Sie eine Liste der zu einer Kalendergruppe gehörenden Kalender abrufen.
author: angelgolfer-ms
ms.openlocfilehash: a6cf89b6c5670659d5864496118d125d3c60a903
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336680"
---
# <a name="list-calendars"></a><span data-ttu-id="4f9f3-103">Kalender auflisten</span><span class="sxs-lookup"><span data-stu-id="4f9f3-103">List calendars</span></span>

> <span data-ttu-id="4f9f3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4f9f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f9f3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4f9f3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4f9f3-106">Mit dieser API können Sie eine Liste der zu einer Kalendergruppe gehörenden Kalender abrufen.</span><span class="sxs-lookup"><span data-stu-id="4f9f3-106">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="4f9f3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4f9f3-107">Permissions</span></span>

<span data-ttu-id="4f9f3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f9f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4f9f3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4f9f3-110">Permission type</span></span>                        | <span data-ttu-id="4f9f3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4f9f3-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4f9f3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4f9f3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4f9f3-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4f9f3-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="4f9f3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4f9f3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4f9f3-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4f9f3-115">Calendars.Read</span></span>                              |
| <span data-ttu-id="4f9f3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4f9f3-116">Application</span></span>                            | <span data-ttu-id="4f9f3-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="4f9f3-117">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="4f9f3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f9f3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="4f9f3-119">Die standardmäßige [CalendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="4f9f3-119">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="4f9f3-120">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="4f9f3-120">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4f9f3-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4f9f3-121">Optional query parameters</span></span>

<span data-ttu-id="4f9f3-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4f9f3-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4f9f3-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4f9f3-123">Request headers</span></span>

| <span data-ttu-id="4f9f3-124">Name</span><span class="sxs-lookup"><span data-stu-id="4f9f3-124">Name</span></span>          | <span data-ttu-id="4f9f3-125">Typ</span><span class="sxs-lookup"><span data-stu-id="4f9f3-125">Type</span></span>   | <span data-ttu-id="4f9f3-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4f9f3-126">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="4f9f3-127">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="4f9f3-127">Authorization</span></span> | <span data-ttu-id="4f9f3-128">string</span><span class="sxs-lookup"><span data-stu-id="4f9f3-128">string</span></span> | <span data-ttu-id="4f9f3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4f9f3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4f9f3-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4f9f3-131">Request body</span></span>

<span data-ttu-id="4f9f3-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4f9f3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4f9f3-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f9f3-133">Response</span></span>

<span data-ttu-id="4f9f3-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Calendar](../resources/calendar.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f9f3-134">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f9f3-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4f9f3-135">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4f9f3-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4f9f3-136">Request</span></span>

<span data-ttu-id="4f9f3-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4f9f3-137">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="4f9f3-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="4f9f3-138">Response</span></span>

<span data-ttu-id="4f9f3-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4f9f3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
