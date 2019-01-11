---
title: Kalender auflisten
description: 'Mit dieser API können Sie alle Kalender eines Benutzers (Navigationseigenschaft `/calendars`), alle Kalender aus der Standardkalendergruppe oder alle Kalender aus einer bestimmten Kalendergruppe abrufen. '
localization_priority: Normal
ms.openlocfilehash: c59ee99c900aa39221530473c9323dfcaab721b5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886514"
---
# <a name="list-calendars"></a><span data-ttu-id="f8efa-103">Kalender auflisten</span><span class="sxs-lookup"><span data-stu-id="f8efa-103">List calendars</span></span>

> <span data-ttu-id="f8efa-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f8efa-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8efa-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f8efa-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f8efa-106">Mit dieser API können Sie alle Kalender eines Benutzers (Navigationseigenschaft `/calendars`), alle Kalender aus der Standardkalendergruppe oder alle Kalender aus einer bestimmten Kalendergruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="f8efa-106">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="f8efa-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f8efa-107">Permissions</span></span>
<span data-ttu-id="f8efa-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8efa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8efa-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f8efa-110">Permission type</span></span>      | <span data-ttu-id="f8efa-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f8efa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f8efa-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f8efa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f8efa-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8efa-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f8efa-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f8efa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f8efa-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8efa-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="f8efa-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f8efa-116">Application</span></span> | <span data-ttu-id="f8efa-117">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f8efa-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f8efa-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8efa-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="f8efa-119">Des Benutzers Kalender.</span><span class="sxs-lookup"><span data-stu-id="f8efa-119">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="f8efa-120">Der Kalender des Benutzers in der standardmäßigen [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="f8efa-120">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="f8efa-121">Der Kalender des Benutzers in einer bestimmten [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="f8efa-121">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f8efa-122">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f8efa-122">Optional query parameters</span></span>
<span data-ttu-id="f8efa-123">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="f8efa-123">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f8efa-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f8efa-124">Request headers</span></span>
| <span data-ttu-id="f8efa-125">Header</span><span class="sxs-lookup"><span data-stu-id="f8efa-125">Header</span></span>       | <span data-ttu-id="f8efa-126">Wert</span><span class="sxs-lookup"><span data-stu-id="f8efa-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f8efa-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8efa-127">Authorization</span></span>  | <span data-ttu-id="f8efa-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f8efa-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f8efa-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f8efa-130">Content-Type</span></span>   | <span data-ttu-id="f8efa-131">application/json</span><span class="sxs-lookup"><span data-stu-id="f8efa-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f8efa-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f8efa-132">Request body</span></span>
<span data-ttu-id="f8efa-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f8efa-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f8efa-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8efa-134">Response</span></span>

<span data-ttu-id="f8efa-135">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Calendar](../resources/calendar.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8efa-135">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f8efa-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f8efa-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f8efa-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f8efa-137">Request</span></span>
<span data-ttu-id="f8efa-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f8efa-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendars
```
##### <a name="response"></a><span data-ttu-id="f8efa-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="f8efa-139">Response</span></span>
<span data-ttu-id="f8efa-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8efa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#me/calendars",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/beta/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
            "id": "AAMkAGI2TGuLAAA=",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
            "isDefaultCalendar": true,
            "canShare":true,
            "canViewPrivateItems":true,
            "hexColor": "",
            "isShared":false,
            "isSharedWithMe":false,
            "canEdit":true,
            "owner":{
                "name":"Samantha Booth",
                "address":"samanthab@adatum.onmicrosoft.com"
            }
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
