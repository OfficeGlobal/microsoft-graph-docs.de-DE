---
title: Verzeichnisrollenmitglied entfernen
description: Mit dieser API können Sie Mitglieder aus einer Ressource des Typs „directoryRole“ entfernen.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0c218351d9c8e556220630f150f5e43592c626f0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956142"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="2095a-103">Verzeichnisrollenmitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="2095a-103">Remove directory role member</span></span>

> <span data-ttu-id="2095a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="2095a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2095a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="2095a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2095a-106">Mit dieser API können Sie Mitglieder aus einer Ressource des Typs „directoryRole“ entfernen.</span><span class="sxs-lookup"><span data-stu-id="2095a-106">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="2095a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2095a-107">Permissions</span></span>

<span data-ttu-id="2095a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2095a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2095a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2095a-110">Permission type</span></span>      | <span data-ttu-id="2095a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2095a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2095a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2095a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2095a-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2095a-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2095a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2095a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2095a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2095a-115">Not supported.</span></span>    |
|<span data-ttu-id="2095a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2095a-116">Application</span></span> | <span data-ttu-id="2095a-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2095a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2095a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2095a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2095a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2095a-119">Request headers</span></span>

| <span data-ttu-id="2095a-120">Name</span><span class="sxs-lookup"><span data-stu-id="2095a-120">Name</span></span>       | <span data-ttu-id="2095a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="2095a-121">Type</span></span> | <span data-ttu-id="2095a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2095a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2095a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2095a-123">Authorization</span></span>  | <span data-ttu-id="2095a-124">string</span><span class="sxs-lookup"><span data-stu-id="2095a-124">string</span></span>  | <span data-ttu-id="2095a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2095a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2095a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2095a-127">Request body</span></span>

<span data-ttu-id="2095a-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2095a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2095a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2095a-129">Response</span></span>

<span data-ttu-id="2095a-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2095a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2095a-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2095a-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="2095a-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2095a-133">Request</span></span>

<span data-ttu-id="2095a-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2095a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="2095a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2095a-135">Response</span></span>

<span data-ttu-id="2095a-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2095a-136">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
