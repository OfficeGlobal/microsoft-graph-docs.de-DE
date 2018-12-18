---
title: Gerät löschen
description: Mit dieser API können Sie registrierte Geräte löschen.
author: tfitzmac
ms.openlocfilehash: e171656e0d4ab32f140c1b53f5ea42e8424cb2e9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311522"
---
# <a name="delete-device"></a><span data-ttu-id="eff72-103">Gerät löschen</span><span class="sxs-lookup"><span data-stu-id="eff72-103">Delete device</span></span>

> <span data-ttu-id="eff72-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eff72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eff72-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eff72-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eff72-106">Mit dieser API können Sie registrierte Geräte löschen.</span><span class="sxs-lookup"><span data-stu-id="eff72-106">Delete a registered device.</span></span>

## <a name="permissions"></a><span data-ttu-id="eff72-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eff72-107">Permissions</span></span>
<span data-ttu-id="eff72-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eff72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eff72-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eff72-110">Permission type</span></span>      | <span data-ttu-id="eff72-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eff72-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eff72-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eff72-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eff72-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eff72-113">Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="eff72-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eff72-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eff72-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eff72-115">Not supported.</span></span>    |
|<span data-ttu-id="eff72-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eff72-116">Application</span></span> | <span data-ttu-id="eff72-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eff72-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eff72-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eff72-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /devices/{id}

```

> <span data-ttu-id="eff72-119">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="eff72-119">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eff72-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eff72-120">Request headers</span></span>
| <span data-ttu-id="eff72-121">Name</span><span class="sxs-lookup"><span data-stu-id="eff72-121">Name</span></span>       | <span data-ttu-id="eff72-122">Typ</span><span class="sxs-lookup"><span data-stu-id="eff72-122">Type</span></span> | <span data-ttu-id="eff72-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eff72-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eff72-124">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="eff72-124">Authorization</span></span>  | <span data-ttu-id="eff72-125">string</span><span class="sxs-lookup"><span data-stu-id="eff72-125">string</span></span>  | <span data-ttu-id="eff72-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eff72-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eff72-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eff72-128">Request body</span></span>
<span data-ttu-id="eff72-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="eff72-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eff72-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="eff72-130">Response</span></span>

<span data-ttu-id="eff72-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eff72-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eff72-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eff72-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eff72-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eff72-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_device"
}-->
```http
DELETE https://graph.microsoft.com/beta/devices/{id}
```
##### <a name="response"></a><span data-ttu-id="eff72-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="eff72-135">Response</span></span>

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