---
title: Besitzer entfernen
description: Verwenden Sie diese API, um einen Besitzer aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die owners-Navigationseigenschaft zu entfernen.
ms.openlocfilehash: 7ed56ae78f99c583e382b25652702f4189b7842e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062669"
---
# <a name="remove-owner"></a><span data-ttu-id="3ce10-103">Besitzer entfernen</span><span class="sxs-lookup"><span data-stu-id="3ce10-103">Remove owner</span></span>

> <span data-ttu-id="3ce10-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3ce10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ce10-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3ce10-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3ce10-106">Verwenden Sie diese API, um einen Besitzer aus einer Office 365-Gruppe, einer Sicherheitsgruppe oder einer E-Mail-aktivierten Sicherheitsgruppe durch die owners-Navigationseigenschaft zu entfernen.</span><span class="sxs-lookup"><span data-stu-id="3ce10-106">Use this API to remove an owner from an Office 365 group, a security group, or a mail-enabled security group through the owners navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ce10-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3ce10-107">Permissions</span></span>
<span data-ttu-id="3ce10-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ce10-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ce10-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3ce10-110">Permission type</span></span>      | <span data-ttu-id="3ce10-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3ce10-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ce10-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3ce10-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3ce10-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3ce10-113">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3ce10-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3ce10-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ce10-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3ce10-115">Not supported.</span></span>    |
|<span data-ttu-id="3ce10-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3ce10-116">Application</span></span> | <span data-ttu-id="3ce10-117">Group.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ce10-117">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ce10-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ce10-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/owners/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="3ce10-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3ce10-119">Request headers</span></span>
| <span data-ttu-id="3ce10-120">Name</span><span class="sxs-lookup"><span data-stu-id="3ce10-120">Name</span></span>       | <span data-ttu-id="3ce10-121">Typ</span><span class="sxs-lookup"><span data-stu-id="3ce10-121">Type</span></span> | <span data-ttu-id="3ce10-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3ce10-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ce10-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ce10-123">Authorization</span></span>  | <span data-ttu-id="3ce10-124">string</span><span class="sxs-lookup"><span data-stu-id="3ce10-124">string</span></span>  | <span data-ttu-id="3ce10-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3ce10-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ce10-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3ce10-127">Request body</span></span>
<span data-ttu-id="3ce10-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3ce10-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ce10-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ce10-129">Response</span></span>
<span data-ttu-id="3ce10-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3ce10-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ce10-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3ce10-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3ce10-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3ce10-133">Request</span></span>
<span data-ttu-id="3ce10-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3ce10-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/owners/{id}/$ref
```
<span data-ttu-id="3ce10-135">Geben Sie in der Anforderung das `id` des Verzeichnisobjekts, das Sie entfernen möchten, nach dem $ref-Segment an.</span><span class="sxs-lookup"><span data-stu-id="3ce10-135">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="3ce10-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="3ce10-136">Response</span></span>
<span data-ttu-id="3ce10-137">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3ce10-137">The following is an example of the response.</span></span>
><span data-ttu-id="3ce10-138">**Hinweis:** im Response-Objekt dargestellten möglicherweise zur besseren Lesbarkeit gekürzt werden.</span><span class="sxs-lookup"><span data-stu-id="3ce10-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="3ce10-139">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="3ce10-139">All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->