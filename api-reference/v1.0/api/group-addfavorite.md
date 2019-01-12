---
title: 'group: addFavorite'
description: Fügt die Gruppe zu der Liste der Favoritengruppen des aktuellen Benutzers hinzu. Wird nur für Office 365-Gruppen unterstützt.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5878c3b0ac324592204310c80458744e4e54c446
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916390"
---
# <a name="group-addfavorite"></a><span data-ttu-id="46b4e-104">group: addFavorite</span><span class="sxs-lookup"><span data-stu-id="46b4e-104">group: addFavorite</span></span>
<span data-ttu-id="46b4e-p102">Fügt die Gruppe zu der Liste der Favoritengruppen des aktuellen Benutzers hinzu. Wird nur für Office 365-Gruppen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46b4e-p102">Add the group to the list of the current user's favorite groups. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="46b4e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="46b4e-107">Permissions</span></span>
<span data-ttu-id="46b4e-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46b4e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46b4e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="46b4e-110">Permission type</span></span>      | <span data-ttu-id="46b4e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="46b4e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46b4e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="46b4e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="46b4e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46b4e-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="46b4e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="46b4e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46b4e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46b4e-115">Not supported.</span></span>    |
|<span data-ttu-id="46b4e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="46b4e-116">Application</span></span> | <span data-ttu-id="46b4e-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="46b4e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46b4e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="46b4e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/addFavorite
```

## <a name="request-headers"></a><span data-ttu-id="46b4e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="46b4e-119">Request headers</span></span>
| <span data-ttu-id="46b4e-120">Header</span><span class="sxs-lookup"><span data-stu-id="46b4e-120">Header</span></span>       | <span data-ttu-id="46b4e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="46b4e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="46b4e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="46b4e-122">Authorization</span></span>  | <span data-ttu-id="46b4e-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="46b4e-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="46b4e-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="46b4e-125">Prefer</span></span> | <span data-ttu-id="46b4e-126">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="46b4e-126">return=minimal.</span></span> <span data-ttu-id="46b4e-127">Wenn die Antwortkopfzeile „minimal“ in der Anforderungskopfzeile enthalten ist, gibt eine erfolgreiche Antwort den `204 No Content`-Code zurück. </span><span class="sxs-lookup"><span data-stu-id="46b4e-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="46b4e-128">Optional.</span><span class="sxs-lookup"><span data-stu-id="46b4e-128">Optional.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="46b4e-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="46b4e-129">Request body</span></span>
<span data-ttu-id="46b4e-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="46b4e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46b4e-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="46b4e-131">Response</span></span>
<span data-ttu-id="46b4e-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="46b4e-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46b4e-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="46b4e-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="46b4e-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="46b4e-135">Request</span></span>
<span data-ttu-id="46b4e-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="46b4e-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_addfavorite"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/addFavorite
```

#### <a name="response"></a><span data-ttu-id="46b4e-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="46b4e-137">Response</span></span>
<span data-ttu-id="46b4e-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="46b4e-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: addFavorite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
