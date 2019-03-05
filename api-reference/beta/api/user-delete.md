---
title: Löschen eines Benutzers – Microsoft Graph-API
description: Beschreibt die Delete-Methode der Benutzerressource (Entity) der Microsoft Graph-API (REST).
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f7f8ed5b11930865d88ed7f01530c052c3e63738
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253792"
---
# <a name="delete-a-user"></a><span data-ttu-id="b4d1d-103">Benutzer löschen</span><span class="sxs-lookup"><span data-stu-id="b4d1d-103">Delete a user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4d1d-104">Mit dieser API können Sie Benutzer löschen.</span><span class="sxs-lookup"><span data-stu-id="b4d1d-104">Delete user.</span></span>  

<span data-ttu-id="b4d1d-105">Nach dem Löschen werden Benutzer Ressourcen in einen temporären Container verschoben und können innerhalb von 30 Tagen wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="b4d1d-105">When deleted, user resources are moved to a temporary container and can be restored within 30 days.</span></span>  <span data-ttu-id="b4d1d-106">Nach diesem Zeitpunkt werden Sie dauerhaft gelöscht.</span><span class="sxs-lookup"><span data-stu-id="b4d1d-106">After that time, they are permanently deleted.</span></span>  <span data-ttu-id="b4d1d-107">Weitere Informationen finden Sie unter [deletedItems](../resources/directory.md).</span><span class="sxs-lookup"><span data-stu-id="b4d1d-107">To learn more, see [deletedItems](../resources/directory.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4d1d-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b4d1d-108">Permissions</span></span>

<span data-ttu-id="b4d1d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4d1d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4d1d-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b4d1d-111">Permission type</span></span>      | <span data-ttu-id="b4d1d-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b4d1d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4d1d-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b4d1d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b4d1d-114">User.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b4d1d-114">User.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b4d1d-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b4d1d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4d1d-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b4d1d-116">Not supported.</span></span>    |
|<span data-ttu-id="b4d1d-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b4d1d-117">Application</span></span> | <span data-ttu-id="b4d1d-118">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4d1d-118">User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4d1d-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4d1d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}
```

## <a name="request-headers"></a><span data-ttu-id="b4d1d-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b4d1d-120">Request headers</span></span>

| <span data-ttu-id="b4d1d-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b4d1d-121">Header</span></span>       | <span data-ttu-id="b4d1d-122">Wert</span><span class="sxs-lookup"><span data-stu-id="b4d1d-122">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b4d1d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4d1d-123">Authorization</span></span>  | <span data-ttu-id="b4d1d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b4d1d-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4d1d-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b4d1d-126">Request body</span></span>

<span data-ttu-id="b4d1d-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b4d1d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4d1d-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4d1d-128">Response</span></span>

<span data-ttu-id="b4d1d-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b4d1d-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4d1d-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b4d1d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4d1d-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b4d1d-132">Request</span></span>

<span data-ttu-id="b4d1d-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b4d1d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/ba9a3254-9f18-4209-aeb3-9e42a35b5be4 
```
### <a name="response"></a><span data-ttu-id="b4d1d-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b4d1d-134">Response</span></span>

<span data-ttu-id="b4d1d-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b4d1d-135">Here is an example of the response.</span></span> 
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
  "description": "Delete user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
