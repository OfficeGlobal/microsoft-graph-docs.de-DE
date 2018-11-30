---
title: Löschen Sie eine Einstellung für die directory
description: Eine Einstellung für die Verzeichnis zu löschen.
ms.openlocfilehash: 442c4f0433dd1595708b478f527bf881a055713d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063128"
---
# <a name="delete-a-directory-setting"></a><span data-ttu-id="b2b87-103">Löschen Sie eine Einstellung für die directory</span><span class="sxs-lookup"><span data-stu-id="b2b87-103">Delete a directory setting</span></span>

> <span data-ttu-id="b2b87-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b2b87-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2b87-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b2b87-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2b87-106">Eine Einstellung für die Verzeichnis zu löschen.</span><span class="sxs-lookup"><span data-stu-id="b2b87-106">Delete a directory setting.</span></span>

> <span data-ttu-id="b2b87-107">**Hinweis**: die Version /beta diese API ist nur auf Gruppen angewendet wird.</span><span class="sxs-lookup"><span data-stu-id="b2b87-107">**Note**: The /beta version of this API is only applies to groups.</span></span> <span data-ttu-id="b2b87-108">Die Version /v1.0 dieser API wurde zu *löschenden GroupSettings*umbenannt.</span><span class="sxs-lookup"><span data-stu-id="b2b87-108">The /v1.0 version of this API has been renamed to *Delete groupSettings*.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2b87-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b2b87-109">Permissions</span></span>
<span data-ttu-id="b2b87-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2b87-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2b87-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b2b87-112">Permission type</span></span>      | <span data-ttu-id="b2b87-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b2b87-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2b87-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b2b87-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b2b87-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b2b87-115">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b2b87-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b2b87-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b2b87-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b2b87-117">Not supported.</span></span>    |
|<span data-ttu-id="b2b87-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b2b87-118">Application</span></span> | <span data-ttu-id="b2b87-119">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2b87-119">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2b87-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2b87-120">HTTP request</span></span>
<span data-ttu-id="b2b87-121"><!-- { "blockType": "ignored" } -->Löschen einer bestimmten Mandanten geltende oder gruppeneinstellung</span><span class="sxs-lookup"><span data-stu-id="b2b87-121"><!-- { "blockType": "ignored" } --> Delete a specific tenant-wide or group setting</span></span>
```http
DELETE /settings/{id}
DELETE /groups/{id}/settings/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b2b87-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b2b87-122">Request headers</span></span>
| <span data-ttu-id="b2b87-123">Name</span><span class="sxs-lookup"><span data-stu-id="b2b87-123">Name</span></span>       | <span data-ttu-id="b2b87-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2b87-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b2b87-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2b87-125">Authorization</span></span>  | <span data-ttu-id="b2b87-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b2b87-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b2b87-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b2b87-128">Request body</span></span>
<span data-ttu-id="b2b87-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="b2b87-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2b87-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2b87-130">Response</span></span>

<span data-ttu-id="b2b87-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b2b87-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2b87-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b2b87-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b2b87-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b2b87-134">Request</span></span>
<span data-ttu-id="b2b87-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b2b87-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directorysetting"
}-->
```http
DELETE https://graph.microsoft.com/beta/settings/{id}
```
##### <a name="response"></a><span data-ttu-id="b2b87-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b2b87-136">Response</span></span>
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
  "description": "Delete directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->