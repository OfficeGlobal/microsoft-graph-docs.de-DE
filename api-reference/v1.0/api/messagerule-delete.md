---
title: Löschen von messageRule
description: Löschen des angegebenen MessageRule-Objekts.
author: angelgolfer-ms
ms.openlocfilehash: 5fe208b72ddc28ca3d2ee5d2b0f1c48113e49c64
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343463"
---
# <a name="delete-messagerule"></a><span data-ttu-id="8ba98-103">Löschen von messageRule</span><span class="sxs-lookup"><span data-stu-id="8ba98-103">Delete messageRule</span></span>


<span data-ttu-id="8ba98-104">Löschen des angegebenen [MessageRule](../resources/messagerule.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="8ba98-104">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ba98-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8ba98-105">Permissions</span></span>
<span data-ttu-id="8ba98-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ba98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ba98-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ba98-108">Permission type</span></span>      | <span data-ttu-id="8ba98-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ba98-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ba98-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ba98-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ba98-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ba98-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="8ba98-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ba98-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ba98-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ba98-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="8ba98-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ba98-114">Application</span></span> | <span data-ttu-id="8ba98-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8ba98-115">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ba98-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ba98-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messageRules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messageRules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8ba98-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ba98-117">Request headers</span></span>
| <span data-ttu-id="8ba98-118">Name</span><span class="sxs-lookup"><span data-stu-id="8ba98-118">Name</span></span>       | <span data-ttu-id="8ba98-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ba98-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8ba98-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ba98-120">Authorization</span></span>  | <span data-ttu-id="8ba98-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8ba98-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="8ba98-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ba98-123">Request body</span></span>
<span data-ttu-id="8ba98-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8ba98-124">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="8ba98-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ba98-125">Response</span></span>
<span data-ttu-id="8ba98-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ba98-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ba98-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ba98-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ba98-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ba98-129">Request</span></span>
<span data-ttu-id="8ba98-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ba98-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["inbox", "AQAAAJ5dZp8="],
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messageRules/AQAAAJ5dZp8=

```
##### <a name="response"></a><span data-ttu-id="8ba98-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ba98-131">Response</span></span>
<span data-ttu-id="8ba98-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8ba98-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "isEmpty": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->