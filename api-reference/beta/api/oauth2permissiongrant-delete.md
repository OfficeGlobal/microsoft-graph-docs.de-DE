---
title: OAuth2PermissionGrant löschen
description: Löschen einer oAuth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: 8eed0c8d2179af6fe199137cfeb7e386a97f733c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813818"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="a009a-103">OAuth2PermissionGrant löschen</span><span class="sxs-lookup"><span data-stu-id="a009a-103">Delete oAuth2PermissionGrant</span></span>

> <span data-ttu-id="a009a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a009a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a009a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a009a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a009a-106">Löschen einer oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="a009a-106">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="a009a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a009a-107">Permissions</span></span>
<span data-ttu-id="a009a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a009a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a009a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a009a-110">Permission type</span></span>      | <span data-ttu-id="a009a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a009a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a009a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a009a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a009a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a009a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a009a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a009a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a009a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a009a-115">Not supported.</span></span>    |
|<span data-ttu-id="a009a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a009a-116">Application</span></span> | <span data-ttu-id="a009a-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a009a-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a009a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a009a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="a009a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a009a-119">Request headers</span></span>
| <span data-ttu-id="a009a-120">Name</span><span class="sxs-lookup"><span data-stu-id="a009a-120">Name</span></span>       | <span data-ttu-id="a009a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="a009a-121">Type</span></span> | <span data-ttu-id="a009a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a009a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a009a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a009a-123">Authorization</span></span>  | <span data-ttu-id="a009a-124">string</span><span class="sxs-lookup"><span data-stu-id="a009a-124">string</span></span>  | <span data-ttu-id="a009a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a009a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a009a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a009a-127">Request body</span></span>
<span data-ttu-id="a009a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a009a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a009a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="a009a-129">Response</span></span>

<span data-ttu-id="a009a-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a009a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a009a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a009a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a009a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a009a-133">Request</span></span>
<span data-ttu-id="a009a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a009a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="a009a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="a009a-135">Response</span></span>
<span data-ttu-id="a009a-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a009a-136">Here is an example of the response.</span></span> 
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
  "description": "Delete oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
