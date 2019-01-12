---
title: Gerät löschen
description: Mit dieser API können Sie registrierte Geräte löschen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6088f7667346e472531b065b5c13eb2953529aea
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921339"
---
# <a name="delete-device"></a><span data-ttu-id="c3be9-103">Gerät löschen</span><span class="sxs-lookup"><span data-stu-id="c3be9-103">Delete device</span></span>

> <span data-ttu-id="c3be9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c3be9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3be9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c3be9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c3be9-106">Mit dieser API können Sie registrierte Geräte löschen.</span><span class="sxs-lookup"><span data-stu-id="c3be9-106">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3be9-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c3be9-107">Permissions</span></span>
<span data-ttu-id="c3be9-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3be9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c3be9-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c3be9-110">Permission type</span></span>      | <span data-ttu-id="c3be9-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c3be9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3be9-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c3be9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c3be9-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c3be9-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="c3be9-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c3be9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3be9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3be9-115">Not supported.</span></span>    |
|<span data-ttu-id="c3be9-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c3be9-116">Application</span></span> | <span data-ttu-id="c3be9-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c3be9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c3be9-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3be9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="c3be9-119">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="c3be9-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c3be9-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c3be9-120">Request headers</span></span>
| <span data-ttu-id="c3be9-121">Name</span><span class="sxs-lookup"><span data-stu-id="c3be9-121">Name</span></span>       | <span data-ttu-id="c3be9-122">Typ</span><span class="sxs-lookup"><span data-stu-id="c3be9-122">Type</span></span> | <span data-ttu-id="c3be9-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c3be9-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c3be9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3be9-124">Authorization</span></span>  | <span data-ttu-id="c3be9-125">string</span><span class="sxs-lookup"><span data-stu-id="c3be9-125">string</span></span>  | <span data-ttu-id="c3be9-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c3be9-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3be9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c3be9-128">Request body</span></span>
<span data-ttu-id="c3be9-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c3be9-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3be9-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3be9-130">Response</span></span>

<span data-ttu-id="c3be9-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c3be9-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3be9-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c3be9-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c3be9-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c3be9-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="c3be9-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c3be9-135">Response</span></span>

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
