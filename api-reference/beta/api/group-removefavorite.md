---
title: 'group: removeFavorite'
description: Entfernt die Gruppe aus der Liste der Favoritengruppen des aktuellen Benutzers. Wird nur für Office 365-Gruppen unterstützt.
ms.openlocfilehash: 718559a3cd5f429bd0409c8644fab7a0d194e03d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059989"
---
# <a name="group-removefavorite"></a><span data-ttu-id="6b9be-104">group: removeFavorite</span><span class="sxs-lookup"><span data-stu-id="6b9be-104">group: removeFavorite</span></span>

> <span data-ttu-id="6b9be-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6b9be-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b9be-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b9be-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b9be-p103">Entfernt die Gruppe aus der Liste der Favoritengruppen des aktuellen Benutzers. Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6b9be-p103">Remove the group from the list of the current user's favorite groups. Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b9be-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6b9be-109">Permissions</span></span>
<span data-ttu-id="6b9be-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b9be-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b9be-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6b9be-112">Permission type</span></span>      | <span data-ttu-id="6b9be-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6b9be-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b9be-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6b9be-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6b9be-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b9be-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b9be-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6b9be-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b9be-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b9be-117">Not supported.</span></span>    |
|<span data-ttu-id="6b9be-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6b9be-118">Application</span></span> | <span data-ttu-id="6b9be-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6b9be-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b9be-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b9be-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/removeFavorite
```

## <a name="request-headers"></a><span data-ttu-id="6b9be-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6b9be-121">Request headers</span></span>
| <span data-ttu-id="6b9be-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6b9be-122">Header</span></span>       | <span data-ttu-id="6b9be-123">Wert</span><span class="sxs-lookup"><span data-stu-id="6b9be-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6b9be-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b9be-124">Authorization</span></span>  | <span data-ttu-id="6b9be-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6b9be-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6b9be-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="6b9be-127">Prefer</span></span> | <span data-ttu-id="6b9be-128">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="6b9be-128">return=minimal.</span></span> <span data-ttu-id="6b9be-129">Wenn die Antwortkopfzeile „minimal“ in der Anforderungskopfzeile enthalten ist, gibt eine erfolgreiche Antwort den `204 No Content`-Code zurück. </span><span class="sxs-lookup"><span data-stu-id="6b9be-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="6b9be-130">Optional.</span><span class="sxs-lookup"><span data-stu-id="6b9be-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="6b9be-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6b9be-131">Request body</span></span>
<span data-ttu-id="6b9be-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="6b9be-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b9be-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b9be-133">Response</span></span>
<span data-ttu-id="6b9be-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6b9be-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b9be-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6b9be-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6b9be-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6b9be-137">Request</span></span>
<span data-ttu-id="6b9be-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6b9be-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_removefavorite"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/removeFavorite
```

#### <a name="response"></a><span data-ttu-id="6b9be-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="6b9be-139">Response</span></span>
<span data-ttu-id="6b9be-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6b9be-140">The following is an example of the response.</span></span>
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