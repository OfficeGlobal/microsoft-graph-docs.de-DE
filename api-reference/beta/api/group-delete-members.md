---
title: Mitglied entfernen
description: Verwenden Sie diese API, um ein Mitglied aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **members**-Navigationseigenschaft zu entfernen. Sie können Benutzer oder andere Gruppen entfernen.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 0ab1dff154903149b2cfc92f5d6cb9cbacbae166
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926113"
---
# <a name="remove-member"></a><span data-ttu-id="56e3b-104">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="56e3b-104">Remove member</span></span>

> <span data-ttu-id="56e3b-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="56e3b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56e3b-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="56e3b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56e3b-p103">Verwenden Sie diese API, um ein Mitglied aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **members**-Navigationseigenschaft zu entfernen. Sie können Benutzer oder andere Gruppen entfernen.</span><span class="sxs-lookup"><span data-stu-id="56e3b-p103">Use this API to remove a member from an Office 365 group, a security group, or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="56e3b-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="56e3b-109">Permissions</span></span>
<span data-ttu-id="56e3b-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56e3b-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56e3b-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56e3b-112">Permission type</span></span>      | <span data-ttu-id="56e3b-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56e3b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56e3b-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56e3b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="56e3b-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="56e3b-115">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56e3b-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56e3b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56e3b-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56e3b-117">Not supported.</span></span>    |
|<span data-ttu-id="56e3b-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56e3b-118">Application</span></span> | <span data-ttu-id="56e3b-119">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56e3b-119">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56e3b-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56e3b-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="56e3b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56e3b-121">Request headers</span></span>
| <span data-ttu-id="56e3b-122">Name</span><span class="sxs-lookup"><span data-stu-id="56e3b-122">Name</span></span>       | <span data-ttu-id="56e3b-123">Typ</span><span class="sxs-lookup"><span data-stu-id="56e3b-123">Type</span></span> | <span data-ttu-id="56e3b-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56e3b-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="56e3b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="56e3b-125">Authorization</span></span>  | <span data-ttu-id="56e3b-126">string</span><span class="sxs-lookup"><span data-stu-id="56e3b-126">string</span></span>  | <span data-ttu-id="56e3b-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="56e3b-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56e3b-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56e3b-129">Request body</span></span>
<span data-ttu-id="56e3b-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="56e3b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56e3b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="56e3b-131">Response</span></span>
<span data-ttu-id="56e3b-p106">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56e3b-p106">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56e3b-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56e3b-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="56e3b-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56e3b-135">Request</span></span>
<span data-ttu-id="56e3b-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56e3b-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="56e3b-137">Geben Sie in der Anforderung das `id` des Verzeichnisobjekts, das Sie entfernen möchten, nach dem $ref-Segment an.</span><span class="sxs-lookup"><span data-stu-id="56e3b-137">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="56e3b-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="56e3b-138">Response</span></span>
<span data-ttu-id="56e3b-139">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="56e3b-139">The following is an example of the response.</span></span>
><span data-ttu-id="56e3b-140">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="56e3b-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="56e3b-141">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="56e3b-141">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
