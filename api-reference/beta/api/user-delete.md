---
title: Benutzer löschen
description: Mit dieser API können Sie Benutzer löschen.
author: dkershaw10
ms.openlocfilehash: d6f1a09e02fd054767a3e54050b9b0a9cb0042a7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320587"
---
# <a name="delete-a-user"></a><span data-ttu-id="588ba-103">Benutzer löschen</span><span class="sxs-lookup"><span data-stu-id="588ba-103">Delete a user</span></span>

> <span data-ttu-id="588ba-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="588ba-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="588ba-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="588ba-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="588ba-106">Mit dieser API können Sie Benutzer löschen.</span><span class="sxs-lookup"><span data-stu-id="588ba-106">Delete user.</span></span>
## <a name="permissions"></a><span data-ttu-id="588ba-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="588ba-107">Permissions</span></span>
<span data-ttu-id="588ba-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="588ba-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="588ba-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="588ba-110">Permission type</span></span>      | <span data-ttu-id="588ba-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="588ba-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="588ba-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="588ba-112">Delegated (work or school account)</span></span> | <span data-ttu-id="588ba-113">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="588ba-113">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="588ba-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="588ba-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="588ba-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="588ba-115">Not supported.</span></span>    |
|<span data-ttu-id="588ba-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="588ba-116">Application</span></span> | <span data-ttu-id="588ba-117">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="588ba-117">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="588ba-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="588ba-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="588ba-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="588ba-119">Request headers</span></span>
| <span data-ttu-id="588ba-120">Header</span><span class="sxs-lookup"><span data-stu-id="588ba-120">Header</span></span>       | <span data-ttu-id="588ba-121">Wert</span><span class="sxs-lookup"><span data-stu-id="588ba-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="588ba-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="588ba-122">Authorization</span></span>  | <span data-ttu-id="588ba-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="588ba-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="588ba-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="588ba-125">Request body</span></span>
<span data-ttu-id="588ba-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="588ba-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="588ba-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="588ba-127">Response</span></span>

<span data-ttu-id="588ba-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="588ba-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="588ba-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="588ba-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="588ba-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="588ba-131">Request</span></span>
<span data-ttu-id="588ba-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="588ba-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
##### <a name="response"></a><span data-ttu-id="588ba-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="588ba-133">Response</span></span>
<span data-ttu-id="588ba-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="588ba-134">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->