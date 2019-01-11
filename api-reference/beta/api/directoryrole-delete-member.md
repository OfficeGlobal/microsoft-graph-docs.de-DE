---
title: Verzeichnisrollenmitglied entfernen
description: Mit dieser API können Sie Mitglieder aus einer Ressource des Typs „directoryRole“ entfernen.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 57b99ec59765d58a96ae43919e7907d480e8817a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843323"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="cce92-103">Verzeichnisrollenmitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="cce92-103">Remove directory role member</span></span>

> <span data-ttu-id="cce92-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="cce92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cce92-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="cce92-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cce92-106">Mit dieser API können Sie Mitglieder aus einer Ressource des Typs „directoryRole“ entfernen.</span><span class="sxs-lookup"><span data-stu-id="cce92-106">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="cce92-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cce92-107">Permissions</span></span>

<span data-ttu-id="cce92-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cce92-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cce92-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cce92-110">Permission type</span></span>      | <span data-ttu-id="cce92-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cce92-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cce92-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cce92-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cce92-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cce92-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cce92-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cce92-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cce92-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cce92-115">Not supported.</span></span>    |
|<span data-ttu-id="cce92-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cce92-116">Application</span></span> | <span data-ttu-id="cce92-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cce92-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cce92-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cce92-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryroles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="cce92-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cce92-119">Request headers</span></span>

| <span data-ttu-id="cce92-120">Name</span><span class="sxs-lookup"><span data-stu-id="cce92-120">Name</span></span>       | <span data-ttu-id="cce92-121">Typ</span><span class="sxs-lookup"><span data-stu-id="cce92-121">Type</span></span> | <span data-ttu-id="cce92-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cce92-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="cce92-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cce92-123">Authorization</span></span>  | <span data-ttu-id="cce92-124">string</span><span class="sxs-lookup"><span data-stu-id="cce92-124">string</span></span>  | <span data-ttu-id="cce92-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cce92-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cce92-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cce92-127">Request body</span></span>

<span data-ttu-id="cce92-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cce92-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cce92-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cce92-129">Response</span></span>

<span data-ttu-id="cce92-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cce92-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cce92-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cce92-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cce92-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cce92-133">Request</span></span>

<span data-ttu-id="cce92-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cce92-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/beta/directoryroles/{id}/members/{id}/$ref
```

##### <a name="response"></a><span data-ttu-id="cce92-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cce92-135">Response</span></span>

<span data-ttu-id="cce92-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cce92-136">Here is an example of the response.</span></span> 
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
