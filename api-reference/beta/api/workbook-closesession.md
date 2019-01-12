---
title: Sitzung schließen
description: 'Verwenden Sie diese API, um eine vorhandene Arbeitsmappensitzung zu schließen. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ff089565cc885cc5d70fbea238335b546b41f2ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930663"
---
# <a name="close-session"></a><span data-ttu-id="9754e-103">Sitzung schließen</span><span class="sxs-lookup"><span data-stu-id="9754e-103">Close Session</span></span>

<span data-ttu-id="9754e-104">Verwenden Sie diese API, um eine vorhandene Arbeitsmappensitzung zu schließen.</span><span class="sxs-lookup"><span data-stu-id="9754e-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9754e-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9754e-105">Permissions</span></span>
<span data-ttu-id="9754e-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9754e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9754e-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9754e-108">Permission type</span></span>      | <span data-ttu-id="9754e-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9754e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9754e-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9754e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9754e-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9754e-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="9754e-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9754e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9754e-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9754e-113">Not supported.</span></span>    |
|<span data-ttu-id="9754e-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9754e-114">Application</span></span> | <span data-ttu-id="9754e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9754e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9754e-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9754e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="9754e-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9754e-117">Request headers</span></span>
| <span data-ttu-id="9754e-118">Name</span><span class="sxs-lookup"><span data-stu-id="9754e-118">Name</span></span>       | <span data-ttu-id="9754e-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9754e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9754e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9754e-120">Authorization</span></span>  | <span data-ttu-id="9754e-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9754e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9754e-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="9754e-123">workbook-session-id</span></span> | <span data-ttu-id="9754e-124">Arbeitsmappensitzungs-ID zum Schließen</span><span class="sxs-lookup"><span data-stu-id="9754e-124">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="9754e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9754e-125">Request body</span></span>
<span data-ttu-id="9754e-126">Für diese API ist kein Anforderungstext erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9754e-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="9754e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="9754e-127">Response</span></span>

<span data-ttu-id="9754e-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9754e-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9754e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9754e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9754e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9754e-130">Request</span></span>
<span data-ttu-id="9754e-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="9754e-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="9754e-132">Beachten Sie, dass ein Arbeitsmappesitzungs-ID-Header erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="9754e-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="9754e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="9754e-133">Response</span></span>
<span data-ttu-id="9754e-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="9754e-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
