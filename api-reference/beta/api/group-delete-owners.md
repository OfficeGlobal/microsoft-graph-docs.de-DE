---
title: Besitzer entfernen
description: Verwenden Sie diese API, um einen Besitzer aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die owners-Navigationseigenschaft zu entfernen.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 761849207983157a770c6c9cd5bea90a6c1b14ef
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522910"
---
# <a name="remove-owner"></a><span data-ttu-id="96360-103">Besitzer entfernen</span><span class="sxs-lookup"><span data-stu-id="96360-103">Remove owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96360-104">Verwenden Sie diese API, um einen Besitzer aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die owners-Navigationseigenschaft zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="96360-104">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="96360-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="96360-105">Permissions</span></span>
<span data-ttu-id="96360-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96360-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96360-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="96360-108">Permission type</span></span>      | <span data-ttu-id="96360-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="96360-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96360-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="96360-110">Delegated (work or school account)</span></span> | <span data-ttu-id="96360-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="96360-111">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="96360-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="96360-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96360-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="96360-113">Not supported.</span></span>    |
|<span data-ttu-id="96360-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="96360-114">Application</span></span> | <span data-ttu-id="96360-115">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96360-115">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="96360-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="96360-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="96360-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="96360-117">Request headers</span></span>
| <span data-ttu-id="96360-118">Name</span><span class="sxs-lookup"><span data-stu-id="96360-118">Name</span></span>       | <span data-ttu-id="96360-119">Typ</span><span class="sxs-lookup"><span data-stu-id="96360-119">Type</span></span> | <span data-ttu-id="96360-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="96360-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="96360-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="96360-121">Authorization</span></span>  | <span data-ttu-id="96360-122">string</span><span class="sxs-lookup"><span data-stu-id="96360-122">string</span></span>  | <span data-ttu-id="96360-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="96360-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="96360-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="96360-125">Request body</span></span>
<span data-ttu-id="96360-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="96360-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96360-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="96360-127">Response</span></span>
<span data-ttu-id="96360-p103">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="96360-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96360-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="96360-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="96360-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="96360-131">Request</span></span>
<span data-ttu-id="96360-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="96360-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="96360-133">Geben Sie in der Anforderung das `id` des Verzeichnisobjekts, das Sie entfernen möchten, nach dem $ref-Segment an.</span><span class="sxs-lookup"><span data-stu-id="96360-133">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="96360-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="96360-134">Response</span></span>
<span data-ttu-id="96360-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="96360-135">The following is an example of the response.</span></span>
><span data-ttu-id="96360-136">**Hinweis:**  Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="96360-136">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="96360-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="96360-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-owners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
