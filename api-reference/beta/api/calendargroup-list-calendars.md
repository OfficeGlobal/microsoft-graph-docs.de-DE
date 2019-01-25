---
title: Kalender auflisten
description: Mit dieser API können Sie eine Liste der zu einer Kalendergruppe gehörenden Kalender abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5e1ca56fdeb2f1087a6c6902ee387220e6966602
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510064"
---
# <a name="list-calendars"></a><span data-ttu-id="7b710-103">Kalender auflisten</span><span class="sxs-lookup"><span data-stu-id="7b710-103">List calendars</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b710-104">Mit dieser API können Sie eine Liste der zu einer Kalendergruppe gehörenden Kalender abrufen.</span><span class="sxs-lookup"><span data-stu-id="7b710-104">Retrieve a list of calendars belonging to a calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="7b710-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7b710-105">Permissions</span></span>

<span data-ttu-id="7b710-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b710-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b710-108">Permission type</span></span>                        | <span data-ttu-id="7b710-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b710-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="7b710-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b710-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="7b710-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7b710-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="7b710-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b710-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b710-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7b710-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="7b710-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b710-114">Application</span></span>                            | <span data-ttu-id="7b710-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7b710-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="7b710-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b710-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="7b710-117">Die standardmäßige [CalendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="7b710-117">A user's default [calendarGroup](../resources/calendargroup.md).</span></span>

```http
GET /me/calendarGroup/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="7b710-118">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="7b710-118">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7b710-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7b710-119">Optional query parameters</span></span>

<span data-ttu-id="7b710-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b710-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7b710-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b710-121">Request headers</span></span>

| <span data-ttu-id="7b710-122">Name</span><span class="sxs-lookup"><span data-stu-id="7b710-122">Name</span></span>          | <span data-ttu-id="7b710-123">Typ</span><span class="sxs-lookup"><span data-stu-id="7b710-123">Type</span></span>   | <span data-ttu-id="7b710-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b710-124">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="7b710-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b710-125">Authorization</span></span> | <span data-ttu-id="7b710-126">string</span><span class="sxs-lookup"><span data-stu-id="7b710-126">string</span></span> | <span data-ttu-id="7b710-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7b710-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b710-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b710-129">Request body</span></span>

<span data-ttu-id="7b710-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7b710-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b710-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b710-131">Response</span></span>

<span data-ttu-id="7b710-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Calendar](../resources/calendar.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b710-132">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b710-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b710-133">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7b710-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b710-134">Request</span></span>

<span data-ttu-id="7b710-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b710-135">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}/calendars
```

##### <a name="response"></a><span data-ttu-id="7b710-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b710-136">Response</span></span>

<span data-ttu-id="7b710-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7b710-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "List calendars",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendargroup-list-calendars.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
