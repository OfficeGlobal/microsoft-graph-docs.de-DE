---
title: Sitzung aktualisieren
description: 'Verwenden Sie diese API, um eine vorhandene Arbeitsmappensitzung zu aktualisieren. '
ms.openlocfilehash: d3504646f4fcacfd71e18c3fc6a83e4835397703
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016645"
---
# <a name="refresh-session"></a><span data-ttu-id="56d95-103">Sitzung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="56d95-103">Refresh Session</span></span>

<span data-ttu-id="56d95-104">Verwenden Sie diese API, um eine vorhandene Arbeitsmappensitzung zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="56d95-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="56d95-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="56d95-105">Permissions</span></span>
<span data-ttu-id="56d95-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56d95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56d95-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56d95-108">Permission type</span></span>      | <span data-ttu-id="56d95-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56d95-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56d95-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56d95-110">Delegated (work or school account)</span></span> | <span data-ttu-id="56d95-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56d95-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="56d95-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56d95-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56d95-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56d95-113">Not supported.</span></span>    |
|<span data-ttu-id="56d95-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56d95-114">Application</span></span> | <span data-ttu-id="56d95-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56d95-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56d95-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56d95-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="56d95-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56d95-117">Request headers</span></span>
| <span data-ttu-id="56d95-118">Name</span><span class="sxs-lookup"><span data-stu-id="56d95-118">Name</span></span>       | <span data-ttu-id="56d95-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56d95-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="56d95-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="56d95-120">Authorization</span></span>  | <span data-ttu-id="56d95-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="56d95-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="56d95-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="56d95-123">workbook-session-id</span></span> | <span data-ttu-id="56d95-124">Arbeitsmappensitzungs-ID für die Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="56d95-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="56d95-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56d95-125">Request body</span></span>
<span data-ttu-id="56d95-126">Für diese API ist kein Anforderungstext erforderlich.</span><span class="sxs-lookup"><span data-stu-id="56d95-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="56d95-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="56d95-127">Response</span></span>

<span data-ttu-id="56d95-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56d95-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="56d95-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56d95-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56d95-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56d95-130">Request</span></span>
<span data-ttu-id="56d95-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56d95-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="56d95-132">Beachten Sie, dass ein Arbeitsmappesitzungs-ID-Header erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="56d95-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="56d95-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="56d95-133">Response</span></span>
<span data-ttu-id="56d95-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="56d95-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: refresh_excel_session//api-reference/v1.0/api/workbook-refreshsession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->
