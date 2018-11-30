---
title: CalendarGroup abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kalendergruppenobjekts abrufen.
ms.openlocfilehash: ffaf4fa4fbc96649bb93a430e77be758e8768ceb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018522"
---
# <a name="get-calendargroup"></a><span data-ttu-id="85f2a-103">CalendarGroup abrufen</span><span class="sxs-lookup"><span data-stu-id="85f2a-103">Get calendarGroup</span></span>

<span data-ttu-id="85f2a-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kalendergruppenobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="85f2a-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="85f2a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="85f2a-105">Permissions</span></span>

<span data-ttu-id="85f2a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85f2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85f2a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="85f2a-108">Permission type</span></span>                        | <span data-ttu-id="85f2a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="85f2a-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="85f2a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="85f2a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="85f2a-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="85f2a-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="85f2a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="85f2a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85f2a-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="85f2a-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="85f2a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="85f2a-114">Application</span></span>                            | <span data-ttu-id="85f2a-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="85f2a-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="85f2a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="85f2a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="85f2a-117">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="85f2a-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="85f2a-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="85f2a-118">Optional query parameters</span></span>

<span data-ttu-id="85f2a-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="85f2a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85f2a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="85f2a-120">Request headers</span></span>

| <span data-ttu-id="85f2a-121">Name</span><span class="sxs-lookup"><span data-stu-id="85f2a-121">Name</span></span>          | <span data-ttu-id="85f2a-122">Typ</span><span class="sxs-lookup"><span data-stu-id="85f2a-122">Type</span></span>   | <span data-ttu-id="85f2a-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="85f2a-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="85f2a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="85f2a-124">Authorization</span></span> | <span data-ttu-id="85f2a-125">string</span><span class="sxs-lookup"><span data-stu-id="85f2a-125">string</span></span> | <span data-ttu-id="85f2a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="85f2a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85f2a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="85f2a-128">Request body</span></span>

<span data-ttu-id="85f2a-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="85f2a-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85f2a-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="85f2a-130">Response</span></span>

<span data-ttu-id="85f2a-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [calendarGroup](../resources/calendargroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85f2a-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85f2a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="85f2a-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="85f2a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="85f2a-133">Request</span></span>

<span data-ttu-id="85f2a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="85f2a-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="85f2a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="85f2a-135">Response</span></span>

<span data-ttu-id="85f2a-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="85f2a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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