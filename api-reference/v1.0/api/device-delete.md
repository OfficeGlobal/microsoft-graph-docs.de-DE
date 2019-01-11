---
title: Gerät löschen
description: Mit dieser API können Sie registrierte Geräte löschen.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eec8a198c783a0c04ba1e20d73095701c471b5cb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845668"
---
# <a name="delete-device"></a><span data-ttu-id="e2902-103">Gerät löschen</span><span class="sxs-lookup"><span data-stu-id="e2902-103">Delete device</span></span>

<span data-ttu-id="e2902-104">Mit dieser API können Sie registrierte Geräte löschen.</span><span class="sxs-lookup"><span data-stu-id="e2902-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2902-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e2902-105">Permissions</span></span>
<span data-ttu-id="e2902-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2902-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e2902-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e2902-108">Permission type</span></span>      | <span data-ttu-id="e2902-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e2902-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2902-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e2902-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2902-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2902-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="e2902-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e2902-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2902-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2902-113">Not supported.</span></span>    |
|<span data-ttu-id="e2902-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e2902-114">Application</span></span> | <span data-ttu-id="e2902-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2902-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2902-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2902-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="e2902-117">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="e2902-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2902-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e2902-118">Request headers</span></span>
| <span data-ttu-id="e2902-119">Name</span><span class="sxs-lookup"><span data-stu-id="e2902-119">Name</span></span>       | <span data-ttu-id="e2902-120">Typ</span><span class="sxs-lookup"><span data-stu-id="e2902-120">Type</span></span> | <span data-ttu-id="e2902-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e2902-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2902-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2902-122">Authorization</span></span>  | <span data-ttu-id="e2902-123">string</span><span class="sxs-lookup"><span data-stu-id="e2902-123">string</span></span>  | <span data-ttu-id="e2902-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e2902-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2902-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e2902-126">Request body</span></span>
<span data-ttu-id="e2902-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e2902-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2902-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2902-128">Response</span></span>

<span data-ttu-id="e2902-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2902-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2902-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2902-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2902-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2902-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="e2902-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2902-133">Response</span></span>

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
  "description": "Delete device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
