---
title: Verzeichnisrollenmitglied hinzufügen
description: Mit dieser API können Sie ein neues Verzeichnisrollenmitglied erstellen.
ms.openlocfilehash: 751e1247036a15f0f53ac3aba3a36bca523a5eea
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018029"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="816a1-103">Verzeichnisrollenmitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="816a1-103">Add directory role member</span></span>

<span data-ttu-id="816a1-104">Mit dieser API können Sie ein neues Verzeichnisrollenmitglied erstellen.</span><span class="sxs-lookup"><span data-stu-id="816a1-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="816a1-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="816a1-105">Permissions</span></span>
<span data-ttu-id="816a1-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="816a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="816a1-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="816a1-108">Permission type</span></span>      | <span data-ttu-id="816a1-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="816a1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="816a1-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="816a1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="816a1-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="816a1-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="816a1-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="816a1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="816a1-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="816a1-113">Not supported.</span></span>    |
|<span data-ttu-id="816a1-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="816a1-114">Application</span></span> | <span data-ttu-id="816a1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="816a1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="816a1-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="816a1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="816a1-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="816a1-117">Request headers</span></span>
| <span data-ttu-id="816a1-118">Name</span><span class="sxs-lookup"><span data-stu-id="816a1-118">Name</span></span>       | <span data-ttu-id="816a1-119">Typ</span><span class="sxs-lookup"><span data-stu-id="816a1-119">Type</span></span> | <span data-ttu-id="816a1-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="816a1-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="816a1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="816a1-121">Authorization</span></span>  | <span data-ttu-id="816a1-122">string</span><span class="sxs-lookup"><span data-stu-id="816a1-122">string</span></span>  | <span data-ttu-id="816a1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="816a1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="816a1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="816a1-125">Content-Type</span></span>  | <span data-ttu-id="816a1-126">string</span><span class="sxs-lookup"><span data-stu-id="816a1-126">string</span></span>  | <span data-ttu-id="816a1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="816a1-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="816a1-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="816a1-128">Request body</span></span>
<span data-ttu-id="816a1-129">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="816a1-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="816a1-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="816a1-130">Response</span></span>

<span data-ttu-id="816a1-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="816a1-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="816a1-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="816a1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="816a1-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="816a1-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directoryrole"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/$ref
Content-type: application/json

{
  "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}
```

##### <a name="response"></a><span data-ttu-id="816a1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="816a1-134">Response</span></span>
<span data-ttu-id="816a1-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="816a1-135">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->