---
title: CalendarGroup abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kalendergruppenobjekts abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 399dcccbb264b8bd19e72b5e887236269581256a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824878"
---
# <a name="get-calendargroup"></a><span data-ttu-id="f6bed-103">CalendarGroup abrufen</span><span class="sxs-lookup"><span data-stu-id="f6bed-103">Get calendarGroup</span></span>

> <span data-ttu-id="f6bed-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f6bed-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f6bed-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f6bed-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f6bed-106">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kalendergruppenobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="f6bed-106">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6bed-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f6bed-107">Permissions</span></span>

<span data-ttu-id="f6bed-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6bed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f6bed-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f6bed-110">Permission type</span></span>                        | <span data-ttu-id="f6bed-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f6bed-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f6bed-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f6bed-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="f6bed-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f6bed-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="f6bed-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f6bed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6bed-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f6bed-115">Calendars.Read</span></span>                              |
| <span data-ttu-id="f6bed-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f6bed-116">Application</span></span>                            | <span data-ttu-id="f6bed-117">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="f6bed-117">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="f6bed-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6bed-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="f6bed-119">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f6bed-119">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6bed-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f6bed-120">Optional query parameters</span></span>

<span data-ttu-id="f6bed-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f6bed-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6bed-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f6bed-122">Request headers</span></span>

| <span data-ttu-id="f6bed-123">Name</span><span class="sxs-lookup"><span data-stu-id="f6bed-123">Name</span></span>          | <span data-ttu-id="f6bed-124">Typ</span><span class="sxs-lookup"><span data-stu-id="f6bed-124">Type</span></span>   | <span data-ttu-id="f6bed-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f6bed-125">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="f6bed-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6bed-126">Authorization</span></span> | <span data-ttu-id="f6bed-127">string</span><span class="sxs-lookup"><span data-stu-id="f6bed-127">string</span></span> | <span data-ttu-id="f6bed-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f6bed-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6bed-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f6bed-130">Request body</span></span>

<span data-ttu-id="f6bed-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f6bed-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6bed-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6bed-132">Response</span></span>

<span data-ttu-id="f6bed-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [calendarGroup](../resources/calendargroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6bed-133">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6bed-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f6bed-134">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f6bed-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f6bed-135">Request</span></span>

<span data-ttu-id="f6bed-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f6bed-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="f6bed-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="f6bed-137">Response</span></span>

<span data-ttu-id="f6bed-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f6bed-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "Get calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
