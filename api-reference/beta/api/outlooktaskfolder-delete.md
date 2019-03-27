---
title: Outlook Task folder löschen
description: Löscht den angegebenen Outlook-Aufgabenordner.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4c526c937f7d92b6e2b0482193f6c0327f4870c1
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869386"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="cd43f-103">Outlook Task folder löschen</span><span class="sxs-lookup"><span data-stu-id="cd43f-103">Delete outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd43f-104">Löscht den angegebenen Outlook-Aufgabenordner.</span><span class="sxs-lookup"><span data-stu-id="cd43f-104">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="cd43f-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cd43f-105">Permissions</span></span>
<span data-ttu-id="cd43f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd43f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd43f-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cd43f-108">Permission type</span></span>      | <span data-ttu-id="cd43f-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cd43f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd43f-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cd43f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cd43f-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd43f-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="cd43f-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cd43f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd43f-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cd43f-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="cd43f-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cd43f-114">Application</span></span> | <span data-ttu-id="cd43f-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="cd43f-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd43f-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd43f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskFolders/{id}
DELETE /me/outlook/taskGroups/{id}/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cd43f-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cd43f-117">Request headers</span></span>
| <span data-ttu-id="cd43f-118">Name</span><span class="sxs-lookup"><span data-stu-id="cd43f-118">Name</span></span>       | <span data-ttu-id="cd43f-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd43f-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cd43f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd43f-120">Authorization</span></span>  | <span data-ttu-id="cd43f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cd43f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd43f-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cd43f-123">Request body</span></span>
<span data-ttu-id="cd43f-124">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cd43f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd43f-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd43f-125">Response</span></span>

<span data-ttu-id="cd43f-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cd43f-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd43f-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cd43f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd43f-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cd43f-129">Request</span></span>
<span data-ttu-id="cd43f-130">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cd43f-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPXAAA=')
```
##### <a name="response"></a><span data-ttu-id="cd43f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="cd43f-131">Response</span></span>
<span data-ttu-id="cd43f-132">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="cd43f-132">Here is an example of the response.</span></span> 
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
  "description": "Delete outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlooktaskfolder-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
