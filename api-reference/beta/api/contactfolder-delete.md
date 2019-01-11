---
title: contactFolder löschen
description: Mit dieser API können Sie Ressourcen des Typs „contactFolder“ löschen (nicht jedoch die als Standardordner festgelegte Ressource des Typs „contactFolder“).
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: f9b175251a1a9a4862dc1df36d607ed62e56c3e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864862"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="4cb33-103">contactFolder löschen</span><span class="sxs-lookup"><span data-stu-id="4cb33-103">Delete contactFolder</span></span>

> <span data-ttu-id="4cb33-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4cb33-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4cb33-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4cb33-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4cb33-106">Mit dieser API können Sie Ressourcen des Typs „contactFolder“ löschen (nicht jedoch die als Standardordner festgelegte Ressource des Typs „contactFolder“).</span><span class="sxs-lookup"><span data-stu-id="4cb33-106">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="4cb33-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4cb33-107">Permissions</span></span>
<span data-ttu-id="4cb33-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cb33-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cb33-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4cb33-110">Permission type</span></span>      | <span data-ttu-id="4cb33-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4cb33-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cb33-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4cb33-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4cb33-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cb33-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4cb33-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4cb33-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cb33-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cb33-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="4cb33-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4cb33-116">Application</span></span> | <span data-ttu-id="4cb33-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4cb33-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cb33-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cb33-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4cb33-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4cb33-119">Request headers</span></span>
| <span data-ttu-id="4cb33-120">Name</span><span class="sxs-lookup"><span data-stu-id="4cb33-120">Name</span></span>       | <span data-ttu-id="4cb33-121">Typ</span><span class="sxs-lookup"><span data-stu-id="4cb33-121">Type</span></span> | <span data-ttu-id="4cb33-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cb33-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4cb33-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cb33-123">Authorization</span></span>  | <span data-ttu-id="4cb33-124">string</span><span class="sxs-lookup"><span data-stu-id="4cb33-124">string</span></span>  | <span data-ttu-id="4cb33-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4cb33-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4cb33-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4cb33-127">Request body</span></span>
<span data-ttu-id="4cb33-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4cb33-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cb33-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cb33-129">Response</span></span>

<span data-ttu-id="4cb33-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4cb33-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cb33-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4cb33-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cb33-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cb33-133">Request</span></span>
<span data-ttu-id="4cb33-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4cb33-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="4cb33-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cb33-135">Response</span></span>
<span data-ttu-id="4cb33-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4cb33-136">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
