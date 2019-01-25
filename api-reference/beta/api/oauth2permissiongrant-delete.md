---
title: OAuth2PermissionGrant löschen
description: Löschen einer oAuth2PermissionGrant.
localization_priority: Normal
ms.openlocfilehash: 5c115ada8e39412fbe64259da02b1eadef3f263b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523358"
---
# <a name="delete-oauth2permissiongrant"></a><span data-ttu-id="5b921-103">OAuth2PermissionGrant löschen</span><span class="sxs-lookup"><span data-stu-id="5b921-103">Delete oAuth2PermissionGrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b921-104">Löschen einer oAuth2PermissionGrant.</span><span class="sxs-lookup"><span data-stu-id="5b921-104">Delete an oAuth2PermissionGrant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b921-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5b921-105">Permissions</span></span>
<span data-ttu-id="5b921-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b921-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5b921-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b921-108">Permission type</span></span>      | <span data-ttu-id="5b921-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b921-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b921-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b921-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5b921-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5b921-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5b921-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b921-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b921-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b921-113">Not supported.</span></span>    |
|<span data-ttu-id="5b921-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b921-114">Application</span></span> | <span data-ttu-id="5b921-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b921-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b921-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b921-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /oAuth2Permissiongrants/{id}
DELETE /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
DELETE /drive/root/createdByUser/oAuth2Permissiongrants/{id}

```
## <a name="request-headers"></a><span data-ttu-id="5b921-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b921-117">Request headers</span></span>
| <span data-ttu-id="5b921-118">Name</span><span class="sxs-lookup"><span data-stu-id="5b921-118">Name</span></span>       | <span data-ttu-id="5b921-119">Typ</span><span class="sxs-lookup"><span data-stu-id="5b921-119">Type</span></span> | <span data-ttu-id="5b921-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5b921-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5b921-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b921-121">Authorization</span></span>  | <span data-ttu-id="5b921-122">string</span><span class="sxs-lookup"><span data-stu-id="5b921-122">string</span></span>  | <span data-ttu-id="5b921-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5b921-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b921-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b921-125">Request body</span></span>
<span data-ttu-id="5b921-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5b921-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b921-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b921-127">Response</span></span>

<span data-ttu-id="5b921-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b921-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b921-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b921-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5b921-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b921-131">Request</span></span>
<span data-ttu-id="5b921-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b921-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_oAuth2Permissiongrant"
}-->
```http
DELETE https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="5b921-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b921-133">Response</span></span>
<span data-ttu-id="5b921-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b921-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
