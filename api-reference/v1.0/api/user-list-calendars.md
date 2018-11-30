---
title: Kalender auflisten
description: 'Mit dieser API können Sie alle Kalender eines Benutzers (Navigationseigenschaft `/calendars`), alle Kalender aus der Standardkalendergruppe oder alle Kalender aus einer bestimmten Kalendergruppe abrufen. '
ms.openlocfilehash: ca0a494510e8236f21b0700092af3dac926df558
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018089"
---
# <a name="list-calendars"></a><span data-ttu-id="bab0d-103">Kalender auflisten</span><span class="sxs-lookup"><span data-stu-id="bab0d-103">List calendars</span></span>

<span data-ttu-id="bab0d-104">Mit dieser API können Sie alle Kalender eines Benutzers (Navigationseigenschaft `/calendars`), alle Kalender aus der Standardkalendergruppe oder alle Kalender aus einer bestimmten Kalendergruppe abrufen.</span><span class="sxs-lookup"><span data-stu-id="bab0d-104">Get all the user's calendars (`/calendars` navigation property), get the calendars from the default calendar group or from a specific calendar group.</span></span> 
## <a name="permissions"></a><span data-ttu-id="bab0d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bab0d-105">Permissions</span></span>
<span data-ttu-id="bab0d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bab0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bab0d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bab0d-108">Permission type</span></span>      | <span data-ttu-id="bab0d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bab0d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bab0d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bab0d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bab0d-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bab0d-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bab0d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bab0d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bab0d-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bab0d-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="bab0d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bab0d-114">Application</span></span> | <span data-ttu-id="bab0d-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bab0d-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bab0d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bab0d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="bab0d-117">Des Benutzers Kalender.</span><span class="sxs-lookup"><span data-stu-id="bab0d-117">All the user's calendars.</span></span>
```http
GET /me/calendars
GET /users/{id | userPrincipalName}/calendars
```

<span data-ttu-id="bab0d-118">Der Kalender des Benutzers in der standardmäßigen [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="bab0d-118">The user's calendars in the default [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendargroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroup/calendars
```

<span data-ttu-id="bab0d-119">Der Kalender des Benutzers in einer bestimmten [calendarGroup](../resources/calendargroup.md).</span><span class="sxs-lookup"><span data-stu-id="bab0d-119">The user's calendars in a specific [calendarGroup](../resources/calendargroup.md).</span></span>
```http
GET /me/calendarGroups/{calendar_group_id}/calendars
GET /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bab0d-120">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bab0d-120">Optional query parameters</span></span>
<span data-ttu-id="bab0d-121">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bab0d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bab0d-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bab0d-122">Request headers</span></span>
| <span data-ttu-id="bab0d-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bab0d-123">Header</span></span>       | <span data-ttu-id="bab0d-124">Wert</span><span class="sxs-lookup"><span data-stu-id="bab0d-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bab0d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bab0d-125">Authorization</span></span>  | <span data-ttu-id="bab0d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bab0d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bab0d-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bab0d-128">Content-Type</span></span>   | <span data-ttu-id="bab0d-129">application/json</span><span class="sxs-lookup"><span data-stu-id="bab0d-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bab0d-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bab0d-130">Request body</span></span>
<span data-ttu-id="bab0d-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bab0d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bab0d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="bab0d-132">Response</span></span>

<span data-ttu-id="bab0d-133">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Calendar](../resources/calendar.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bab0d-133">If successful, this method returns a `200 OK` response code and collection of [Calendar](../resources/calendar.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bab0d-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bab0d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bab0d-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bab0d-135">Request</span></span>
<span data-ttu-id="bab0d-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bab0d-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendars"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendars
```
##### <a name="response"></a><span data-ttu-id="bab0d-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="bab0d-137">Response</span></span>
<span data-ttu-id="bab0d-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bab0d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#me/calendars",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/calendars('AAMkAGI2TGuLAAA=')",
            "id": "AAMkAGI2TGuLAAA=",
            "name": "Calendar",
            "color": "auto",
            "changeKey": "nfZyf7VcrEKLNoU37KWlkQAAA0x0+w==",
            "canShare":true,
            "canViewPrivateItems":true,
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