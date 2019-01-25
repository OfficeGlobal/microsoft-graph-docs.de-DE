---
title: Löschen Sie eine Einstellung für die directory
description: Eine Einstellung für die Verzeichnis zu löschen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c66335ec863460c9b2167e25a7e78850846e105c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515825"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="b823a-103">Löschen Sie eine Einstellung für die directory</span><span class="sxs-lookup"><span data-stu-id="b823a-103">Delete a directory setting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b823a-104">Eine Einstellung für die Verzeichnis zu löschen.</span><span class="sxs-lookup"><span data-stu-id="b823a-104">Delete a directory setting.</span></span>

> <span data-ttu-id="b823a-105">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="b823a-105">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="b823a-106">Die Version /v1.0 dieser API wurde zu *löschenden GroupSettings*umbenannt.</span><span class="sxs-lookup"><span data-stu-id="b823a-106">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="b823a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b823a-107">Permissions</span></span>
<span data-ttu-id="b823a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b823a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b823a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b823a-110">Permission type</span></span>      | <span data-ttu-id="b823a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b823a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b823a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b823a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b823a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b823a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b823a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b823a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b823a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b823a-115">Not supported.</span></span>    |
|<span data-ttu-id="b823a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b823a-116">Application</span></span> | <span data-ttu-id="b823a-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b823a-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b823a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b823a-118">HTTP request</span></span>
<span data-ttu-id="b823a-119"><!-- { "blockType": "ignored" } -->Löschen einer bestimmten Mandanten geltende oder gruppeneinstellung</span><span class="sxs-lookup"><span data-stu-id="b823a-119"><!-- { "blockType": "ignored" } --> Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b823a-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b823a-120">Request headers</span></span>
| <span data-ttu-id="b823a-121">Name</span><span class="sxs-lookup"><span data-stu-id="b823a-121">Name</span></span>       | <span data-ttu-id="b823a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b823a-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b823a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b823a-123">Authorization</span></span>  | <span data-ttu-id="b823a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b823a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b823a-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b823a-126">Request body</span></span>
<span data-ttu-id="b823a-127">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b823a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b823a-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="b823a-128">Response</span></span>

<span data-ttu-id="b823a-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b823a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b823a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b823a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b823a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b823a-132">Request</span></span>
<span data-ttu-id="b823a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b823a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="b823a-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="b823a-134">Response</span></span>
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
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directorysetting-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
