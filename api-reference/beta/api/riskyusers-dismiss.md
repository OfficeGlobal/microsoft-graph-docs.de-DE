---
title: RiskyUsers schließen
description: Schließen Sie das Risiko eines riskyUsers-Objekts ab.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.date: 03/20/2019
ms.openlocfilehash: 8e7a64e5762808691c4997c83b112a17c9667d47
ms.sourcegitcommit: fd9f62fd9a6d311f98afe2e31afca8b818c402c2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2019
ms.locfileid: "31013131"
---
# <a name="dismiss-riskyusers"></a><span data-ttu-id="ef5fc-103">RiskyUsers schließen</span><span class="sxs-lookup"><span data-stu-id="ef5fc-103">Dismiss riskyUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

><span data-ttu-id="ef5fc-104">**Hinweis:** Die Verwendung der riskyUsers-API erfordert eine Azure AD Premium P2-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="ef5fc-104">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

<span data-ttu-id="ef5fc-105">Schließen Sie das Risiko eines **riskyUsers** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="ef5fc-105">Dismiss the risk of a **riskyUsers** object.</span></span> <span data-ttu-id="ef5fc-106">Mit dieser Aktion wird die Risikostufe des Zielbenutzers auf None festgelegt.</span><span class="sxs-lookup"><span data-stu-id="ef5fc-106">This action will set the targeted user's risk level to none.</span></span>
## <a name="permissions"></a><span data-ttu-id="ef5fc-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ef5fc-107">Permissions</span></span>
<span data-ttu-id="ef5fc-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef5fc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef5fc-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ef5fc-110">Permission type</span></span>      | <span data-ttu-id="ef5fc-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ef5fc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ef5fc-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ef5fc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ef5fc-113">IdentityRiskyUser. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="ef5fc-113">IdentityRiskyUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="ef5fc-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ef5fc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef5fc-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ef5fc-115">Not supported.</span></span>    |
|<span data-ttu-id="ef5fc-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ef5fc-116">Application</span></span> | <span data-ttu-id="ef5fc-117">IdentityRiskyUser. ReadWrite. all</span><span class="sxs-lookup"><span data-stu-id="ef5fc-117">IdentityRiskyUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef5fc-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef5fc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /riskyUsers/dismiss
```


## <a name="request-headers"></a><span data-ttu-id="ef5fc-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ef5fc-119">Request headers</span></span>
| <span data-ttu-id="ef5fc-120">Name</span><span class="sxs-lookup"><span data-stu-id="ef5fc-120">Name</span></span>      |<span data-ttu-id="ef5fc-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ef5fc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ef5fc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef5fc-122">Authorization</span></span>  | <span data-ttu-id="ef5fc-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ef5fc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ef5fc-125">Arbeitsmappensitzungs-ID</span><span class="sxs-lookup"><span data-stu-id="ef5fc-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="ef5fc-126">Sitzungs-ID der Arbeitsmappe, die bestimmt, ob Änderungen beibehalten werden.</span><span class="sxs-lookup"><span data-stu-id="ef5fc-126">Workbook session ID that determines whether changes are persisted.</span></span> <span data-ttu-id="ef5fc-127">Optional.</span><span class="sxs-lookup"><span data-stu-id="ef5fc-127">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef5fc-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ef5fc-128">Request body</span></span>
<span data-ttu-id="ef5fc-129">Geben Sie die Benutzer-IDs an, die im Anforderungstext geschlossen werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ef5fc-129">Specify the userIds to dismiss in the request body.</span></span>

## <a name="response"></a><span data-ttu-id="ef5fc-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef5fc-130">Response</span></span>

<span data-ttu-id="ef5fc-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 NoContent` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ef5fc-131">If successful, this method returns a `204 NoContent` response code.</span></span>
## <a name="example"></a><span data-ttu-id="ef5fc-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ef5fc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ef5fc-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ef5fc-133">Request</span></span>
<span data-ttu-id="ef5fc-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ef5fc-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "dismiss_riskyuser"
}-->
```http
POST https://graph.microsoft.com/beta/riskyUsers/dismiss

Request Body
{
  "userIds": [
    "04487ee0-f4f6-4e7f-8999-facc5a30e232",
    "13387ee0-f4f6-4e7f-8999-facc5120e345"
  ]
}
```
##### <a name="response"></a><span data-ttu-id="ef5fc-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="ef5fc-135">Response</span></span>
<span data-ttu-id="ef5fc-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ef5fc-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUsers"
} -->
```http
HTTP/1.1 204 NoContent
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Dismiss riskyUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
