---
title: calendarGroups auflisten
description: Dient zum Abrufen der Kalendergruppen des Benutzers.
ms.openlocfilehash: 5afdac039ad4e03eb61776c5a3eed92fee2bd577
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016460"
---
# <a name="list-calendargroups"></a><span data-ttu-id="715ba-103">calendarGroups auflisten</span><span class="sxs-lookup"><span data-stu-id="715ba-103">List calendarGroups</span></span>

<span data-ttu-id="715ba-104">Mit dieser API können Sie die Kalendergruppen eines Benutzers abrufen.</span><span class="sxs-lookup"><span data-stu-id="715ba-104">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="715ba-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="715ba-105">Permissions</span></span>
<span data-ttu-id="715ba-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="715ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="715ba-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="715ba-108">Permission type</span></span>      | <span data-ttu-id="715ba-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="715ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="715ba-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="715ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="715ba-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="715ba-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="715ba-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="715ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="715ba-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="715ba-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="715ba-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="715ba-114">Application</span></span> | <span data-ttu-id="715ba-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="715ba-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="715ba-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="715ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="715ba-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="715ba-117">Optional query parameters</span></span>
<span data-ttu-id="715ba-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="715ba-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="715ba-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="715ba-119">Request headers</span></span>
| <span data-ttu-id="715ba-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="715ba-120">Header</span></span>       | <span data-ttu-id="715ba-121">Wert</span><span class="sxs-lookup"><span data-stu-id="715ba-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="715ba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="715ba-122">Authorization</span></span>  | <span data-ttu-id="715ba-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="715ba-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="715ba-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="715ba-125">Content-Type</span></span>  | <span data-ttu-id="715ba-126">application/json</span><span class="sxs-lookup"><span data-stu-id="715ba-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="715ba-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="715ba-127">Request body</span></span>
<span data-ttu-id="715ba-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="715ba-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="715ba-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="715ba-129">Response</span></span>

<span data-ttu-id="715ba-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [CalendarGroup](../resources/calendargroup.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="715ba-130">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="715ba-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="715ba-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="715ba-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="715ba-132">Request</span></span>
<span data-ttu-id="715ba-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="715ba-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups
```
##### <a name="response"></a><span data-ttu-id="715ba-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="715ba-134">Response</span></span>
<span data-ttu-id="715ba-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="715ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 155

{
  "value": [
    {
      "name": "name-value",
      "classId": "classId-value",
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
  "description": "List calendarGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
