---
title: Sitzung schließen
description: 'Verwenden Sie diese API, um eine vorhandene Arbeitsmappensitzung zu schließen. '
ms.openlocfilehash: f38529de8af2289421c577dd074a182da5782d5c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27017810"
---
# <a name="close-session"></a><span data-ttu-id="847bc-103">Sitzung schließen</span><span class="sxs-lookup"><span data-stu-id="847bc-103">Close Session</span></span>

<span data-ttu-id="847bc-104">Verwenden Sie diese API, um eine vorhandene Arbeitsmappensitzung zu schließen.</span><span class="sxs-lookup"><span data-stu-id="847bc-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="847bc-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="847bc-105">Permissions</span></span>
<span data-ttu-id="847bc-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="847bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="847bc-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="847bc-108">Permission type</span></span>      | <span data-ttu-id="847bc-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="847bc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="847bc-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="847bc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="847bc-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="847bc-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="847bc-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="847bc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="847bc-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="847bc-113">Not supported.</span></span>    |
|<span data-ttu-id="847bc-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="847bc-114">Application</span></span> | <span data-ttu-id="847bc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="847bc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="847bc-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="847bc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="847bc-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="847bc-117">Request headers</span></span>
| <span data-ttu-id="847bc-118">Name</span><span class="sxs-lookup"><span data-stu-id="847bc-118">Name</span></span>       | <span data-ttu-id="847bc-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="847bc-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="847bc-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="847bc-120">Authorization</span></span>  | <span data-ttu-id="847bc-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="847bc-p102">Bearer {token}. Required.</span></span> | | <span data-ttu-id="847bc-123">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="847bc-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="847bc-p103">Arbeitsmappensitzungs-ID, die bestimmt, ob Änderungen beibehalten werden. Optional.</span><span class="sxs-lookup"><span data-stu-id="847bc-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|
| <span data-ttu-id="847bc-126">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="847bc-126">workbook-session-id</span></span> | <span data-ttu-id="847bc-127">Arbeitsmappensitzungs-ID zum Schließen</span><span class="sxs-lookup"><span data-stu-id="847bc-127">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="847bc-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="847bc-128">Request body</span></span>
<span data-ttu-id="847bc-129">Für diese API ist kein Anforderungstext erforderlich.</span><span class="sxs-lookup"><span data-stu-id="847bc-129">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="847bc-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="847bc-130">Response</span></span>

<span data-ttu-id="847bc-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="847bc-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="847bc-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="847bc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="847bc-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="847bc-133">Request</span></span>
<span data-ttu-id="847bc-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="847bc-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="847bc-135">Beachten Sie, dass ein Arbeitsmappesitzungs-ID-Header erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="847bc-135">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="847bc-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="847bc-136">Response</span></span>
<span data-ttu-id="847bc-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="847bc-137">Here is an example of the response.</span></span> 

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
    "Warning: close_excel_session//api-reference/v1.0/api/workbook-closesession.md:
      Request includes a non-standard header: workbook-session-id"
  ]
}-->