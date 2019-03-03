---
title: 'SecurityAction: cancelSecurityAction'
description: Abbrechen eines Sicherheits Vorgangs.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 1b37563ffde274944dc877482602c36d2bf3a4bd
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366952"
---
# <a name="securityaction-cancelsecurityaction"></a><span data-ttu-id="601db-103">SecurityAction: cancelSecurityAction</span><span class="sxs-lookup"><span data-stu-id="601db-103">securityAction: cancelSecurityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="601db-104">Abbrechen eines Sicherheits Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="601db-104">Cancel a security operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="601db-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="601db-105">Permissions</span></span>

<span data-ttu-id="601db-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="601db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="601db-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="601db-108">Permission type</span></span>                        | <span data-ttu-id="601db-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="601db-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="601db-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="601db-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="601db-111">SecurityActions. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="601db-111">SecurityActions.ReadWrite.All</span></span> |
| <span data-ttu-id="601db-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="601db-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="601db-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="601db-113">Not supported.</span></span> |
| <span data-ttu-id="601db-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="601db-114">Application</span></span>                            | <span data-ttu-id="601db-115">SecurityActions. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="601db-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="601db-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="601db-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions/{id}/cancelSecurityAction
```

## <a name="request-headers"></a><span data-ttu-id="601db-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="601db-117">Request headers</span></span>

| <span data-ttu-id="601db-118">Name</span><span class="sxs-lookup"><span data-stu-id="601db-118">Name</span></span>          | <span data-ttu-id="601db-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="601db-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="601db-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="601db-120">Authorization</span></span> | <span data-ttu-id="601db-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="601db-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="601db-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="601db-122">Request body</span></span>

<span data-ttu-id="601db-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="601db-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="601db-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="601db-124">Response</span></span>

<span data-ttu-id="601db-p102">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200, OK` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="601db-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="601db-127">Beispiele</span><span class="sxs-lookup"><span data-stu-id="601db-127">Examples</span></span>

<span data-ttu-id="601db-128">Das folgende Beispiel illustriert, wie Sie diese API aufrufen können.</span><span class="sxs-lookup"><span data-stu-id="601db-128">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="601db-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="601db-129">Request</span></span>

<span data-ttu-id="601db-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="601db-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "securityaction_cancelsecurityaction"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction
```

### <a name="response"></a><span data-ttu-id="601db-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="601db-131">Response</span></span>

<span data-ttu-id="601db-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="601db-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityAction: cancelSecurityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
