---
title: Domäne löschen
description: Dient zum Löschen einer Domäne aus einem Mandanten.
ms.openlocfilehash: e5d09eebb9c70ec0b9a172aac6b5f5ff7ecbfab7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016495"
---
# <a name="delete-domain"></a><span data-ttu-id="9f460-103">Domäne löschen</span><span class="sxs-lookup"><span data-stu-id="9f460-103">Delete domain</span></span>

<span data-ttu-id="9f460-104">Dient zum Löschen einer Domäne aus einem Mandanten.</span><span class="sxs-lookup"><span data-stu-id="9f460-104">Deletes a domain from a tenant.</span></span>

> <span data-ttu-id="9f460-105">**Wichtig:**</span><span class="sxs-lookup"><span data-stu-id="9f460-105">**Important:**</span></span>
> - <span data-ttu-id="9f460-106">Gelöschte Domänen können nicht wiederhergestellt werden.</span><span class="sxs-lookup"><span data-stu-id="9f460-106">Deleted domains are not recoverable.</span></span><br />
> - <span data-ttu-id="9f460-p101">Bei Löschversuchen tritt ein Fehler auf, wenn noch Ressourcen oder Objekte von der Domäne abhängig sind. Mithilfe der API [domainNameReferences auflisten](domain-list-domainnamereferences.md) können Sie alle abhängige Ressourcen ermitteln.</span><span class="sxs-lookup"><span data-stu-id="9f460-p101">Attempts to delete will fail if there are any resources or objects still dependent on the domain. You can find all dependent resources by using the [List domainNameReferences](domain-list-domainnamereferences.md) API.</span></span>

## <a name="permissions"></a><span data-ttu-id="9f460-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="9f460-109">Permissions</span></span>

<span data-ttu-id="9f460-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f460-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9f460-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="9f460-112">Permission type</span></span>      | <span data-ttu-id="9f460-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="9f460-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9f460-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="9f460-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9f460-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9f460-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9f460-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="9f460-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f460-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="9f460-117">Not supported.</span></span>    |
|<span data-ttu-id="9f460-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="9f460-118">Application</span></span> | <span data-ttu-id="9f460-119">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f460-119">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f460-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f460-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /domains/{id}
```

> <span data-ttu-id="9f460-121">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="9f460-121">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f460-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="9f460-122">Request headers</span></span>

| <span data-ttu-id="9f460-123">Name</span><span class="sxs-lookup"><span data-stu-id="9f460-123">Name</span></span>       | <span data-ttu-id="9f460-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9f460-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9f460-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f460-125">Authorization</span></span>  | <span data-ttu-id="9f460-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="9f460-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9f460-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9f460-128">Content-Type</span></span>  | <span data-ttu-id="9f460-129">application/json</span><span class="sxs-lookup"><span data-stu-id="9f460-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="9f460-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="9f460-130">Request body</span></span>

<span data-ttu-id="9f460-131">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="9f460-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f460-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f460-132">Response</span></span>

<span data-ttu-id="9f460-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Es wird keine Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f460-p104">If successful, this method returns `204 No Content` response code. It does not return a response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f460-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="9f460-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9f460-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="9f460-136">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "delete_domain"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/domains/contoso.com
```

##### <a name="response"></a><span data-ttu-id="9f460-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="9f460-137">Response</span></span>

<span data-ttu-id="9f460-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="9f460-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->