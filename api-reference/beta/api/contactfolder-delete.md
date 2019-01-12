---
title: contactFolder löschen
description: Mit dieser API können Sie Ressourcen des Typs „contactFolder“ löschen (nicht jedoch die als Standardordner festgelegte Ressource des Typs „contactFolder“).
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e8004d726bc8a47270d040ab295bc41dbf1dbef4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980573"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="c9194-103">contactFolder löschen</span><span class="sxs-lookup"><span data-stu-id="c9194-103">Delete contactFolder</span></span>

> <span data-ttu-id="c9194-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c9194-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9194-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c9194-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9194-106">Mit dieser API können Sie Ressourcen des Typs „contactFolder“ löschen (nicht jedoch die als Standardordner festgelegte Ressource des Typs „contactFolder“).</span><span class="sxs-lookup"><span data-stu-id="c9194-106">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="c9194-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c9194-107">Permissions</span></span>
<span data-ttu-id="c9194-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c9194-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9194-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c9194-110">Permission type</span></span>      | <span data-ttu-id="c9194-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c9194-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9194-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c9194-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c9194-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9194-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c9194-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c9194-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9194-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9194-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c9194-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c9194-116">Application</span></span> | <span data-ttu-id="c9194-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c9194-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9194-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9194-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c9194-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c9194-119">Request headers</span></span>
| <span data-ttu-id="c9194-120">Name</span><span class="sxs-lookup"><span data-stu-id="c9194-120">Name</span></span>       | <span data-ttu-id="c9194-121">Typ</span><span class="sxs-lookup"><span data-stu-id="c9194-121">Type</span></span> | <span data-ttu-id="c9194-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9194-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c9194-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9194-123">Authorization</span></span>  | <span data-ttu-id="c9194-124">string</span><span class="sxs-lookup"><span data-stu-id="c9194-124">string</span></span>  | <span data-ttu-id="c9194-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c9194-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c9194-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c9194-127">Request body</span></span>
<span data-ttu-id="c9194-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c9194-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9194-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9194-129">Response</span></span>

<span data-ttu-id="c9194-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c9194-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9194-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c9194-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c9194-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c9194-133">Request</span></span>
<span data-ttu-id="c9194-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c9194-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="c9194-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="c9194-135">Response</span></span>
<span data-ttu-id="c9194-136">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c9194-136">Here is an example of the response.</span></span> 
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
