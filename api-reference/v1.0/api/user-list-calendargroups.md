---
title: calendarGroups auflisten
description: Dient zum Abrufen der Kalendergruppen des Benutzers.
localization_priority: Normal
ms.openlocfilehash: 932fa9767ecd8ff6957cad825ad4a2864500d41a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808722"
---
# <a name="list-calendargroups"></a><span data-ttu-id="9a528-103">calendarGroups auflisten</span><span class="sxs-lookup"><span data-stu-id="9a528-103">List calendarGroups</span></span>

<span data-ttu-id="9a528-104">Mit dieser API können Sie die Kalendergruppen eines Benutzers abrufen.</span><span class="sxs-lookup"><span data-stu-id="9a528-104">Get the user's calendar groups.</span></span>
## <a name="permissions"></a><span data-ttu-id="9a528-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9a528-105">Permissions</span></span>
<span data-ttu-id="9a528-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a528-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a528-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9a528-108">Permission type</span></span>      | <span data-ttu-id="9a528-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9a528-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a528-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9a528-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9a528-111">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a528-111">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9a528-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9a528-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a528-113">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a528-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="9a528-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9a528-114">Application</span></span> | <span data-ttu-id="9a528-115">Calendars.Read, Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a528-115">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a528-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a528-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/calendarGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9a528-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="9a528-117">Optional query parameters</span></span>
<span data-ttu-id="9a528-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9a528-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9a528-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9a528-119">Request headers</span></span>
| <span data-ttu-id="9a528-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="9a528-120">Header</span></span>       | <span data-ttu-id="9a528-121">Wert</span><span class="sxs-lookup"><span data-stu-id="9a528-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a528-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a528-122">Authorization</span></span>  | <span data-ttu-id="9a528-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9a528-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9a528-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9a528-125">Content-Type</span></span>  | <span data-ttu-id="9a528-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a528-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a528-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9a528-127">Request body</span></span>
<span data-ttu-id="9a528-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9a528-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a528-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a528-129">Response</span></span>

<span data-ttu-id="9a528-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [CalendarGroup](../resources/calendargroup.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a528-130">If successful, this method returns a `200 OK` response code and collection of [CalendarGroup](../resources/calendargroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9a528-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9a528-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9a528-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9a528-132">Request</span></span>
<span data-ttu-id="9a528-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9a528-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_calendargroups"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarGroups
```
##### <a name="response"></a><span data-ttu-id="9a528-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="9a528-134">Response</span></span>
<span data-ttu-id="9a528-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9a528-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
