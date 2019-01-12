---
title: Gerät löschen
description: Mit dieser API können Sie registrierte Geräte löschen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 49bffc1147735aeefcbdb541804fbff386f2c77f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917573"
---
# <a name="delete-device"></a><span data-ttu-id="c79af-103">Gerät löschen</span><span class="sxs-lookup"><span data-stu-id="c79af-103">Delete device</span></span>

<span data-ttu-id="c79af-104">Mit dieser API können Sie registrierte Geräte löschen.</span><span class="sxs-lookup"><span data-stu-id="c79af-104">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="c79af-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c79af-105">Permissions</span></span>
<span data-ttu-id="c79af-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c79af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c79af-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c79af-108">Permission type</span></span>      | <span data-ttu-id="c79af-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c79af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c79af-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c79af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c79af-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c79af-111">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c79af-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c79af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c79af-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c79af-113">Not supported.</span></span>    |
|<span data-ttu-id="c79af-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c79af-114">Application</span></span> | <span data-ttu-id="c79af-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c79af-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c79af-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c79af-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}
```
> <span data-ttu-id="c79af-117">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="c79af-117">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c79af-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c79af-118">Request headers</span></span>
| <span data-ttu-id="c79af-119">Name</span><span class="sxs-lookup"><span data-stu-id="c79af-119">Name</span></span>       | <span data-ttu-id="c79af-120">Typ</span><span class="sxs-lookup"><span data-stu-id="c79af-120">Type</span></span> | <span data-ttu-id="c79af-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c79af-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c79af-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c79af-122">Authorization</span></span>  | <span data-ttu-id="c79af-123">string</span><span class="sxs-lookup"><span data-stu-id="c79af-123">string</span></span>  | <span data-ttu-id="c79af-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c79af-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c79af-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c79af-126">Request body</span></span>
<span data-ttu-id="c79af-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c79af-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c79af-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="c79af-128">Response</span></span>

<span data-ttu-id="c79af-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c79af-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c79af-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c79af-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c79af-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c79af-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="c79af-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c79af-133">Response</span></span>

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
