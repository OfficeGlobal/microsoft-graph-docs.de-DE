---
title: CalendarGroup löschen
description: Dient zum Löschen einer anderen Kalendergruppe als der Standardkalendergruppe.
author: angelgolfer-ms
ms.openlocfilehash: edcb75cfe6d395e505a9d100e85bf4e03bde67a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336743"
---
# <a name="delete-calendargroup"></a><span data-ttu-id="602b3-103">CalendarGroup löschen</span><span class="sxs-lookup"><span data-stu-id="602b3-103">Delete calendarGroup</span></span>

> <span data-ttu-id="602b3-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="602b3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="602b3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="602b3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="602b3-106">Dient zum Löschen einer anderen Kalendergruppe als der Standardkalendergruppe.</span><span class="sxs-lookup"><span data-stu-id="602b3-106">Delete a calendar group other than the default calendar group.</span></span>

## <a name="permissions"></a><span data-ttu-id="602b3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="602b3-107">Permissions</span></span>

<span data-ttu-id="602b3-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="602b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="602b3-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="602b3-110">Permission type</span></span>                        | <span data-ttu-id="602b3-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="602b3-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="602b3-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="602b3-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="602b3-113">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="602b3-113">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="602b3-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="602b3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="602b3-115">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="602b3-115">Calendars.ReadWrite</span></span>                         |
| <span data-ttu-id="602b3-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="602b3-116">Application</span></span>                            | <span data-ttu-id="602b3-117">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="602b3-117">Calendars.ReadWrite</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="602b3-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="602b3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/calendarGroups/{id}
DELETE /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a><span data-ttu-id="602b3-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="602b3-119">Request headers</span></span>

| <span data-ttu-id="602b3-120">Name</span><span class="sxs-lookup"><span data-stu-id="602b3-120">Name</span></span>          | <span data-ttu-id="602b3-121">Typ</span><span class="sxs-lookup"><span data-stu-id="602b3-121">Type</span></span>   | <span data-ttu-id="602b3-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="602b3-122">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="602b3-123">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="602b3-123">Authorization</span></span> | <span data-ttu-id="602b3-124">string</span><span class="sxs-lookup"><span data-stu-id="602b3-124">string</span></span> | <span data-ttu-id="602b3-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="602b3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="602b3-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="602b3-127">Request body</span></span>

<span data-ttu-id="602b3-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="602b3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="602b3-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="602b3-129">Response</span></span>

<span data-ttu-id="602b3-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="602b3-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="602b3-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="602b3-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="602b3-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="602b3-133">Request</span></span>

<span data-ttu-id="602b3-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="602b3-134">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_calendargroup"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/calendarGroups/{id}
```

##### <a name="response"></a><span data-ttu-id="602b3-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="602b3-135">Response</span></span>

<span data-ttu-id="602b3-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="602b3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
