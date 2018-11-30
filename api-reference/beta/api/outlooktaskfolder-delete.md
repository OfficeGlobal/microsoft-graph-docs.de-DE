---
title: OutlookTaskFolder löschen
description: Den angegebenen Outlook den Ordner zu löschen.
ms.openlocfilehash: de287113f6e0eded982947d310239db4d028abc7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060360"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="d3548-103">OutlookTaskFolder löschen</span><span class="sxs-lookup"><span data-stu-id="d3548-103">Delete outlookTaskFolder</span></span>

> <span data-ttu-id="d3548-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="d3548-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3548-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d3548-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3548-106">Den angegebenen Outlook den Ordner zu löschen.</span><span class="sxs-lookup"><span data-stu-id="d3548-106">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="d3548-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d3548-107">Permissions</span></span>
<span data-ttu-id="d3548-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3548-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3548-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d3548-110">Permission type</span></span>      | <span data-ttu-id="d3548-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d3548-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3548-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d3548-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d3548-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3548-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d3548-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d3548-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3548-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3548-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d3548-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d3548-116">Application</span></span> | <span data-ttu-id="d3548-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d3548-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3548-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3548-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}

```
## <a name="request-headers"></a><span data-ttu-id="d3548-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d3548-119">Request headers</span></span>
| <span data-ttu-id="d3548-120">Name</span><span class="sxs-lookup"><span data-stu-id="d3548-120">Name</span></span>       | <span data-ttu-id="d3548-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d3548-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d3548-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3548-122">Authorization</span></span>  | <span data-ttu-id="d3548-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d3548-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3548-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d3548-125">Request body</span></span>
<span data-ttu-id="d3548-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="d3548-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3548-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3548-127">Response</span></span>

<span data-ttu-id="d3548-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d3548-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3548-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d3548-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3548-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d3548-131">Request</span></span>
<span data-ttu-id="d3548-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d3548-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPXAAA=')
```
##### <a name="response"></a><span data-ttu-id="d3548-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="d3548-133">Response</span></span>
<span data-ttu-id="d3548-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d3548-134">Here is an example of the response.</span></span> 
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
  "description": "Delete outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->