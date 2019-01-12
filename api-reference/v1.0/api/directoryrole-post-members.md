---
title: Verzeichnisrollenmitglied hinzufügen
description: Mit dieser API können Sie ein neues Verzeichnisrollenmitglied erstellen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f138be1632c72f8c31eb08fcdaefc50e7affb3e5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991531"
---
# <a name="add-directory-role-member"></a><span data-ttu-id="344b9-103">Verzeichnisrollenmitglied hinzufügen</span><span class="sxs-lookup"><span data-stu-id="344b9-103">Add directory role member</span></span>

<span data-ttu-id="344b9-104">Mit dieser API können Sie ein neues Verzeichnisrollenmitglied erstellen.</span><span class="sxs-lookup"><span data-stu-id="344b9-104">Use this API to create a new directory role member.</span></span>

## <a name="permissions"></a><span data-ttu-id="344b9-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="344b9-105">Permissions</span></span>
<span data-ttu-id="344b9-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="344b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="344b9-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="344b9-108">Permission type</span></span>      | <span data-ttu-id="344b9-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="344b9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="344b9-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="344b9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="344b9-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="344b9-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="344b9-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="344b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="344b9-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="344b9-113">Not supported.</span></span>    |
|<span data-ttu-id="344b9-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="344b9-114">Application</span></span> | <span data-ttu-id="344b9-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="344b9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="344b9-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="344b9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="344b9-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="344b9-117">Request headers</span></span>
| <span data-ttu-id="344b9-118">Name</span><span class="sxs-lookup"><span data-stu-id="344b9-118">Name</span></span>       | <span data-ttu-id="344b9-119">Typ</span><span class="sxs-lookup"><span data-stu-id="344b9-119">Type</span></span> | <span data-ttu-id="344b9-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="344b9-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="344b9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="344b9-121">Authorization</span></span>  | <span data-ttu-id="344b9-122">string</span><span class="sxs-lookup"><span data-stu-id="344b9-122">string</span></span>  | <span data-ttu-id="344b9-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="344b9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="344b9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="344b9-125">Content-Type</span></span>  | <span data-ttu-id="344b9-126">string</span><span class="sxs-lookup"><span data-stu-id="344b9-126">string</span></span>  | <span data-ttu-id="344b9-127">application/json</span><span class="sxs-lookup"><span data-stu-id="344b9-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="344b9-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="344b9-128">Request body</span></span>
<span data-ttu-id="344b9-129">Geben Sie im Anforderungstext eine JSON-Darstellung eines [directoryObject](../resources/directoryobject.md)- oder [user](../resources/user.md)-Objekts an, das hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="344b9-129">In the request body, supply a JSON representation of a [directoryObject](../resources/directoryobject.md) or [user](../resources/user.md) object to be added.</span></span>

## <a name="response"></a><span data-ttu-id="344b9-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="344b9-130">Response</span></span>

<span data-ttu-id="344b9-131">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="344b9-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="344b9-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="344b9-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="344b9-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="344b9-133">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="344b9-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="344b9-134">Response</span></span>
<span data-ttu-id="344b9-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="344b9-135">Note: The response object shown here may be truncated for brevity.</span></span> 
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
