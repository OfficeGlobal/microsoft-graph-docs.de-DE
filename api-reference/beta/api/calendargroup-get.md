---
title: CalendarGroup abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kalendergruppenobjekts abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: c5eb48f208a9f4a6e8fa0b6c6268722501b16d52
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517659"
---
# <a name="get-calendargroup"></a><span data-ttu-id="658fc-103">CalendarGroup abrufen</span><span class="sxs-lookup"><span data-stu-id="658fc-103">Get calendarGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="658fc-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kalendergruppenobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="658fc-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="658fc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="658fc-105">Permissions</span></span>

<span data-ttu-id="658fc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="658fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="658fc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="658fc-108">Permission type</span></span>                        | <span data-ttu-id="658fc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="658fc-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="658fc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="658fc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="658fc-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="658fc-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="658fc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="658fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="658fc-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="658fc-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="658fc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="658fc-114">Application</span></span>                            | <span data-ttu-id="658fc-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="658fc-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="658fc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="658fc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="658fc-117">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="658fc-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="658fc-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="658fc-118">Optional query parameters</span></span>

<span data-ttu-id="658fc-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="658fc-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="658fc-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="658fc-120">Request headers</span></span>

| <span data-ttu-id="658fc-121">Name</span><span class="sxs-lookup"><span data-stu-id="658fc-121">Name</span></span>          | <span data-ttu-id="658fc-122">Typ</span><span class="sxs-lookup"><span data-stu-id="658fc-122">Type</span></span>   | <span data-ttu-id="658fc-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="658fc-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="658fc-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="658fc-124">Authorization</span></span> | <span data-ttu-id="658fc-125">string</span><span class="sxs-lookup"><span data-stu-id="658fc-125">string</span></span> | <span data-ttu-id="658fc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="658fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="658fc-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="658fc-128">Request body</span></span>

<span data-ttu-id="658fc-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="658fc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="658fc-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="658fc-130">Response</span></span>

<span data-ttu-id="658fc-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [calendarGroup](../resources/calendargroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="658fc-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="658fc-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="658fc-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="658fc-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="658fc-133">Request</span></span>

<span data-ttu-id="658fc-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="658fc-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="658fc-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="658fc-135">Response</span></span>

<span data-ttu-id="658fc-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="658fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/calendargroup-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
