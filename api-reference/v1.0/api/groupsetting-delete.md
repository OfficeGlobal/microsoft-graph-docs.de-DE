---
title: Löschen einer Gruppeneinstellung
description: Mit dieser API können Sie Gruppeneinstellungen löschen.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 32bdd6b2856a96377859d523767f198779d23497
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936109"
---
# <a name="delete-a-group-setting"></a><span data-ttu-id="c088f-103">Löschen einer Gruppeneinstellung</span><span class="sxs-lookup"><span data-stu-id="c088f-103">Delete a group setting</span></span>

<span data-ttu-id="c088f-104">Mit dieser API können Sie Gruppeneinstellungen löschen.</span><span class="sxs-lookup"><span data-stu-id="c088f-104">Delete a group setting.</span></span>

## <a name="permissions"></a><span data-ttu-id="c088f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c088f-105">Permissions</span></span>

<span data-ttu-id="c088f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c088f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c088f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c088f-108">Permission type</span></span>      | <span data-ttu-id="c088f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c088f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c088f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c088f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c088f-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c088f-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c088f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c088f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c088f-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c088f-113">Not supported.</span></span>    |
|<span data-ttu-id="c088f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c088f-114">Application</span></span> | <span data-ttu-id="c088f-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c088f-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c088f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c088f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupSettings/{id}
DELETE /groups/{id}/settings/{id}

```

## <a name="request-headers"></a><span data-ttu-id="c088f-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c088f-117">Request headers</span></span>

| <span data-ttu-id="c088f-118">Name</span><span class="sxs-lookup"><span data-stu-id="c088f-118">Name</span></span> | <span data-ttu-id="c088f-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c088f-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="c088f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c088f-120">Authorization</span></span>  | <span data-ttu-id="c088f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c088f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c088f-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c088f-123">Content-Type</span></span>  | <span data-ttu-id="c088f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c088f-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="c088f-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c088f-125">Request body</span></span>
<span data-ttu-id="c088f-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c088f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c088f-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="c088f-127">Response</span></span>

<span data-ttu-id="c088f-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c088f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c088f-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c088f-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c088f-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c088f-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_groupsetting"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="c088f-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="c088f-132">Response</span></span>
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
  "description": "Delete groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
