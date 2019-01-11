---
title: 'group: removeFavorite'
description: Entfernt die Gruppe aus der Liste der Favoritengruppen des aktuellen Benutzers. Wird nur für Office 365-Gruppen unterstützt.
localization_priority: Normal
ms.openlocfilehash: 7299c89bc95ce267adf0149cbf3ff3f76c3a52ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887262"
---
# <a name="group-removefavorite"></a><span data-ttu-id="ed7d8-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="ed7d8-104">group: removeFavorite</span></span>

> <span data-ttu-id="ed7d8-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ed7d8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed7d8-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed7d8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ed7d8-p103">Entfernt die Gruppe aus der Liste der Favoritengruppen des aktuellen Benutzers. Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ed7d8-p103">Remove the group from the list of the current user's favorite groups. Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed7d8-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ed7d8-109">Permissions</span></span>
<span data-ttu-id="ed7d8-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed7d8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed7d8-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed7d8-112">Permission type</span></span>      | <span data-ttu-id="ed7d8-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed7d8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed7d8-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed7d8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ed7d8-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed7d8-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ed7d8-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed7d8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed7d8-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed7d8-117">Not supported.</span></span>    |
|<span data-ttu-id="ed7d8-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed7d8-118">Application</span></span> | <span data-ttu-id="ed7d8-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed7d8-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed7d8-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed7d8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```

## <a name="request-headers"></a><span data-ttu-id="ed7d8-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed7d8-121">Request headers</span></span>
| <span data-ttu-id="ed7d8-122">Header</span><span class="sxs-lookup"><span data-stu-id="ed7d8-122">Header</span></span>       | <span data-ttu-id="ed7d8-123">Wert</span><span class="sxs-lookup"><span data-stu-id="ed7d8-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ed7d8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed7d8-124">Authorization</span></span>  | <span data-ttu-id="ed7d8-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ed7d8-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ed7d8-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="ed7d8-127">Prefer</span></span> | <span data-ttu-id="ed7d8-128">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="ed7d8-128">return=minimal.</span></span> <span data-ttu-id="ed7d8-129">Wenn die Antwortkopfzeile „minimal“ in der Anforderungskopfzeile enthalten ist, gibt eine erfolgreiche Antwort den `204 No Content`-Code zurück. </span><span class="sxs-lookup"><span data-stu-id="ed7d8-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="ed7d8-130">Optional.</span><span class="sxs-lookup"><span data-stu-id="ed7d8-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="ed7d8-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed7d8-131">Request body</span></span>
<span data-ttu-id="ed7d8-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ed7d8-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed7d8-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed7d8-133">Response</span></span>
<span data-ttu-id="ed7d8-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed7d8-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed7d8-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed7d8-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ed7d8-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed7d8-137">Request</span></span>
<span data-ttu-id="ed7d8-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ed7d8-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/removeFavorite
```

#### <a name="response"></a><span data-ttu-id="ed7d8-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed7d8-139">Response</span></span>
<span data-ttu-id="ed7d8-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ed7d8-140">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: removeFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
