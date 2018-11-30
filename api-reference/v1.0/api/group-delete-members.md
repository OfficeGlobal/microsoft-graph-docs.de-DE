---
title: Mitglied entfernen
description: Verwenden Sie diese API, um ein Mitglied aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **members**-Navigationseigenschaft zu entfernen. Sie können Benutzer oder andere Gruppen entfernen.
ms.openlocfilehash: 4c58fd4cbd67143959a35546f69f4f24e8cdd1d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019255"
---
# <a name="remove-member"></a><span data-ttu-id="2a8c1-104">Mitglied entfernen</span><span class="sxs-lookup"><span data-stu-id="2a8c1-104">Remove member</span></span>
<span data-ttu-id="2a8c1-p102">Verwenden Sie diese API, um ein Mitglied aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die **members**-Navigationseigenschaft zu entfernen. Sie können Benutzer oder andere Gruppen entfernen.</span><span class="sxs-lookup"><span data-stu-id="2a8c1-p102">Use this API to remove a member from an Office 365 group, a security group, or a mail-enabled security group through the **members** navigation property. You can remove users or other groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a8c1-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2a8c1-107">Permissions</span></span>
<span data-ttu-id="2a8c1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a8c1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a8c1-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2a8c1-110">Permission type</span></span>      | <span data-ttu-id="2a8c1-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2a8c1-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a8c1-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2a8c1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2a8c1-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2a8c1-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2a8c1-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2a8c1-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a8c1-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2a8c1-115">Not supported.</span></span>    |
|<span data-ttu-id="2a8c1-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2a8c1-116">Application</span></span> | <span data-ttu-id="2a8c1-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a8c1-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2a8c1-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a8c1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2a8c1-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2a8c1-119">Request headers</span></span>
| <span data-ttu-id="2a8c1-120">Name</span><span class="sxs-lookup"><span data-stu-id="2a8c1-120">Name</span></span>       | <span data-ttu-id="2a8c1-121">Typ</span><span class="sxs-lookup"><span data-stu-id="2a8c1-121">Type</span></span> | <span data-ttu-id="2a8c1-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2a8c1-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2a8c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a8c1-123">Authorization</span></span>  | <span data-ttu-id="2a8c1-124">string</span><span class="sxs-lookup"><span data-stu-id="2a8c1-124">string</span></span>  | <span data-ttu-id="2a8c1-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2a8c1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a8c1-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2a8c1-127">Request body</span></span>
<span data-ttu-id="2a8c1-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2a8c1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a8c1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a8c1-129">Response</span></span>
<span data-ttu-id="2a8c1-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2a8c1-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a8c1-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2a8c1-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2a8c1-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2a8c1-133">Request</span></span>
<span data-ttu-id="2a8c1-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2a8c1-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="2a8c1-135">Geben Sie in der Anforderung das `id` des Verzeichnisobjekts, das Sie entfernen möchten, nach dem $ref-Segment an.</span><span class="sxs-lookup"><span data-stu-id="2a8c1-135">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="2a8c1-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="2a8c1-136">Response</span></span>
<span data-ttu-id="2a8c1-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2a8c1-137">The following is an example of the response.</span></span>
><span data-ttu-id="2a8c1-138">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="2a8c1-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="2a8c1-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="2a8c1-139">All the properties will be returned from an actual call.</span></span>
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