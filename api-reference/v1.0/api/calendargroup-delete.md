---
title: CalendarGroup löschen
description: Dient zum Löschen einer anderen Kalendergruppe als der Standardkalendergruppe.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f1dded8885f99646d48ddf309ff12e64d61988e1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978935"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="f94ae-103">CalendarGroup löschen</span><span class="sxs-lookup"><span data-stu-id="f94ae-103">Delete calendarGroup</span></span>

<span data-ttu-id="f94ae-104">Dient zum Löschen einer anderen Kalendergruppe als der Standardkalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="f94ae-104">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="f94ae-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f94ae-105">Permissions</span></span>

<span data-ttu-id="f94ae-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f94ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f94ae-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f94ae-108">Permission type</span></span>                        | <span data-ttu-id="f94ae-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f94ae-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="f94ae-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f94ae-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f94ae-111">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f94ae-111">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="f94ae-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f94ae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f94ae-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f94ae-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="f94ae-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f94ae-114">Application</span></span>                            | <span data-ttu-id="f94ae-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f94ae-115">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="f94ae-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f94ae-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f94ae-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f94ae-117">Request headers</span></span>

| <span data-ttu-id="f94ae-118">Name</span><span class="sxs-lookup"><span data-stu-id="f94ae-118">Name</span></span>          | <span data-ttu-id="f94ae-119">Typ</span><span class="sxs-lookup"><span data-stu-id="f94ae-119">Type</span></span>   | <span data-ttu-id="f94ae-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f94ae-120">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="f94ae-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f94ae-121">Authorization</span></span> | <span data-ttu-id="f94ae-122">string</span><span class="sxs-lookup"><span data-stu-id="f94ae-122">string</span></span> | <span data-ttu-id="f94ae-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f94ae-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f94ae-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f94ae-125">Request body</span></span>

<span data-ttu-id="f94ae-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f94ae-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f94ae-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="f94ae-127">Response</span></span>

<span data-ttu-id="f94ae-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f94ae-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f94ae-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f94ae-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f94ae-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f94ae-131">Request</span></span>

<span data-ttu-id="f94ae-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f94ae-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="f94ae-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="f94ae-133">Response</span></span>

<span data-ttu-id="f94ae-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f94ae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Delete calendarGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
