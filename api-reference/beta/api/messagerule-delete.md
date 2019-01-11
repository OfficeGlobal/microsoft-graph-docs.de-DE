---
title: Löschen von messageRule
description: Löschen des angegebenen MessageRule-Objekts.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 85f48f1f293b898cf911488961dade4a1e9962cc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807294"
---
# <a name="delete-messagerule"></a><span data-ttu-id="c6687-103">Löschen von messageRule</span><span class="sxs-lookup"><span data-stu-id="c6687-103">Delete messageRule</span></span>

> <span data-ttu-id="c6687-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c6687-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6687-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c6687-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6687-106">Löschen des angegebenen [MessageRule](../resources/messagerule.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="c6687-106">Delete the specified [messageRule](../resources/messagerule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6687-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c6687-107">Permissions</span></span>
<span data-ttu-id="c6687-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6687-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6687-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c6687-110">Permission type</span></span>      | <span data-ttu-id="c6687-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c6687-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6687-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c6687-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c6687-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6687-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c6687-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c6687-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6687-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6687-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="c6687-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c6687-116">Application</span></span> | <span data-ttu-id="c6687-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6687-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6687-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6687-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/inbox/messagerules/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c6687-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c6687-119">Request headers</span></span>
| <span data-ttu-id="c6687-120">Name</span><span class="sxs-lookup"><span data-stu-id="c6687-120">Name</span></span>       | <span data-ttu-id="c6687-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c6687-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c6687-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6687-122">Authorization</span></span>  | <span data-ttu-id="c6687-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c6687-p103">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c6687-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c6687-125">Request body</span></span>
<span data-ttu-id="c6687-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c6687-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="c6687-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6687-127">Response</span></span>
<span data-ttu-id="c6687-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c6687-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6687-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c6687-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6687-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c6687-131">Request</span></span>
<span data-ttu-id="c6687-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c6687-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_messagerule"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailfolders/inbox/messagerules('AQAAAJ5dZp8=')

```
##### <a name="response"></a><span data-ttu-id="c6687-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c6687-133">Response</span></span>
<span data-ttu-id="c6687-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c6687-134">Here is an example of the response.</span></span> 
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
