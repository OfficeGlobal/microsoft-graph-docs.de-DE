---
title: Löschen von messageRule
description: Löschen des angegebenen MessageRule-Objekts.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: cfb0f1840ca4a4de0a82b90a4525a8f26b35536d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985564"
---
# <a name="delete-messagerule"></a><span data-ttu-id="d837c-103">Löschen von messageRule</span><span class="sxs-lookup"><span data-stu-id="d837c-103">Delete messageRule</span></span>

> <span data-ttu-id="d837c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d837c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d837c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d837c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d837c-106">Löschen des angegebenen [MessageRule](../resources/messagerule.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="d837c-106">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d837c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d837c-107">Permissions</span></span>
<span data-ttu-id="d837c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d837c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d837c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d837c-110">Permission type</span></span>      | <span data-ttu-id="d837c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d837c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d837c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d837c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d837c-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d837c-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="d837c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d837c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d837c-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d837c-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="d837c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d837c-116">Application</span></span> | <span data-ttu-id="d837c-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d837c-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="d837c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d837c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d837c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d837c-119">Request headers</span></span>
| <span data-ttu-id="d837c-120">Name</span><span class="sxs-lookup"><span data-stu-id="d837c-120">Name</span></span>       | <span data-ttu-id="d837c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d837c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d837c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d837c-122">Authorization</span></span>  | <span data-ttu-id="d837c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d837c-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="d837c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d837c-125">Request body</span></span>
<span data-ttu-id="d837c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d837c-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="d837c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d837c-127">Response</span></span>
<span data-ttu-id="d837c-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d837c-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d837c-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d837c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d837c-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d837c-131">Request</span></span>
<span data-ttu-id="d837c-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d837c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
##### <a name="response"></a><span data-ttu-id="d837c-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d837c-133">Response</span></span>
<span data-ttu-id="d837c-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d837c-134">Here is an example of the response.</span></span> 
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
