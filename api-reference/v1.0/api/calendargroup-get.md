---
title: CalendarGroup abrufen
description: Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kalendergruppenobjekts abrufen.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: c29290064ec877f3e8dafd7173292fefb4c2e958
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848384"
---
# <a name="get-calendargroup"></a><span data-ttu-id="3779b-103">CalendarGroup abrufen</span><span class="sxs-lookup"><span data-stu-id="3779b-103">Get calendarGroup</span></span>

<span data-ttu-id="3779b-104">Mit dieser API können Sie die Eigenschaften und Beziehungen eines Kalendergruppenobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="3779b-104">Retrieve the properties and relationships of a calendar group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3779b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3779b-105">Permissions</span></span>

<span data-ttu-id="3779b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3779b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3779b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3779b-108">Permission type</span></span>                        | <span data-ttu-id="3779b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3779b-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3779b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3779b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3779b-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3779b-111">Calendars.Read</span></span>                              |
| <span data-ttu-id="3779b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3779b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3779b-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3779b-113">Calendars.Read</span></span>                              |
| <span data-ttu-id="3779b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3779b-114">Application</span></span>                            | <span data-ttu-id="3779b-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="3779b-115">Calendars.Read</span></span>                              |

## <a name="http-request"></a><span data-ttu-id="3779b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3779b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="3779b-117">Eine [calendarGroup](../resources/calendargroup.md) eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="3779b-117">Any [calendarGroup](../resources/calendargroup.md) of a user.</span></span>

```http
GET /me/calendarGroups/{id}
GET /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3779b-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3779b-118">Optional query parameters</span></span>

<span data-ttu-id="3779b-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3779b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3779b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3779b-120">Request headers</span></span>

| <span data-ttu-id="3779b-121">Name</span><span class="sxs-lookup"><span data-stu-id="3779b-121">Name</span></span>          | <span data-ttu-id="3779b-122">Typ</span><span class="sxs-lookup"><span data-stu-id="3779b-122">Type</span></span>   | <span data-ttu-id="3779b-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3779b-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="3779b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3779b-124">Authorization</span></span> | <span data-ttu-id="3779b-125">string</span><span class="sxs-lookup"><span data-stu-id="3779b-125">string</span></span> | <span data-ttu-id="3779b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3779b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3779b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3779b-128">Request body</span></span>

<span data-ttu-id="3779b-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3779b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3779b-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="3779b-130">Response</span></span>

<span data-ttu-id="3779b-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [calendarGroup](../resources/calendargroup.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3779b-131">If successful, this method returns a `200 OK` response code and [calendarGroup](../resources/calendargroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3779b-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3779b-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3779b-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3779b-133">Request</span></span>

<span data-ttu-id="3779b-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3779b-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_calendargroup"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="3779b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3779b-135">Response</span></span>

<span data-ttu-id="3779b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3779b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
