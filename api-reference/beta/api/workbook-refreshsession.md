---
title: Sitzung aktualisieren
description: 'Verwenden Sie diese API, um eine vorhandene Arbeitsmappensitzung zu aktualisieren. '
ms.openlocfilehash: 637ce0a07f2ee09cb8496ed88bb62410660e43c2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065736"
---
# <a name="refresh-session"></a><span data-ttu-id="087b9-103">Sitzung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="087b9-103">Refresh Session</span></span>

<span data-ttu-id="087b9-104">Verwenden Sie diese API, um eine vorhandene Arbeitsmappensitzung zu aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="087b9-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="087b9-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="087b9-105">Permissions</span></span>
<span data-ttu-id="087b9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="087b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="087b9-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="087b9-108">Permission type</span></span>      | <span data-ttu-id="087b9-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="087b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="087b9-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="087b9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="087b9-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="087b9-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="087b9-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="087b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="087b9-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="087b9-113">Not supported.</span></span>    |
|<span data-ttu-id="087b9-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="087b9-114">Application</span></span> | <span data-ttu-id="087b9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="087b9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="087b9-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="087b9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="087b9-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="087b9-117">Request headers</span></span>
| <span data-ttu-id="087b9-118">Name</span><span class="sxs-lookup"><span data-stu-id="087b9-118">Name</span></span>       | <span data-ttu-id="087b9-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="087b9-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="087b9-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="087b9-120">Authorization</span></span>  | <span data-ttu-id="087b9-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="087b9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="087b9-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="087b9-123">workbook-session-id</span></span> | <span data-ttu-id="087b9-124">Arbeitsmappensitzungs-ID für die Aktualisierung</span><span class="sxs-lookup"><span data-stu-id="087b9-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="087b9-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="087b9-125">Request body</span></span>
<span data-ttu-id="087b9-126">Für diese API ist kein Anforderungstext erforderlich.</span><span class="sxs-lookup"><span data-stu-id="087b9-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="087b9-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="087b9-127">Response</span></span>

<span data-ttu-id="087b9-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="087b9-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="087b9-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="087b9-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="087b9-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="087b9-130">Request</span></span>
<span data-ttu-id="087b9-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="087b9-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="087b9-132">Beachten Sie, dass ein Arbeitsmappesitzungs-ID-Header erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="087b9-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="087b9-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="087b9-133">Response</span></span>
<span data-ttu-id="087b9-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="087b9-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```