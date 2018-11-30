---
title: Domäne erstellen
description: Fügt eine Domäne zum Mandanten hinzu.
ms.openlocfilehash: 40f49f954799af987287b7ce47044fe5e81fa54c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019923"
---
# <a name="create-domain"></a><span data-ttu-id="a8c6a-103">Domäne erstellen</span><span class="sxs-lookup"><span data-stu-id="a8c6a-103">Create domain</span></span>

<span data-ttu-id="a8c6a-104">Fügt eine Domäne zum Mandanten hinzu.</span><span class="sxs-lookup"><span data-stu-id="a8c6a-104">Adds a domain to the tenant.</span></span>

<span data-ttu-id="a8c6a-p101">**Wichtig**: Sie können eine zugeordnete Domäne erst dann mit Ihrem Azure AD-Mandanten verwenden, nachdem der Besitz überprüft wurde. Weitere Informationen finden Sie unter [verificationDnsRecords auflisten](domain-list-verificationdnsrecords.md). Stammdomänen erfordern eine Überprüfung. Beispielsweise muss „contoso.com“ überprüft werden. Wenn eine Stammdomäne überprüft wird, werden Unterdomänen der Stammdomäne automatisch überprüft. Beispielsweise wird „subdomain.contoso.com“ automatisch überprüft, wenn „contoso.com“ überprüft wurde.</span><span class="sxs-lookup"><span data-stu-id="a8c6a-p101">**Important**: You cannot use an associated domain with your Azure AD tenant until ownership is verified. See [List verificationDnsRecords](domain-list-verificationdnsrecords.md) for details. Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8c6a-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a8c6a-111">Permissions</span></span>

<span data-ttu-id="a8c6a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8c6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a8c6a-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a8c6a-114">Permission type</span></span>      | <span data-ttu-id="a8c6a-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a8c6a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a8c6a-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a8c6a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="a8c6a-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a8c6a-117">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a8c6a-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a8c6a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8c6a-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a8c6a-119">Not supported.</span></span>    |
|<span data-ttu-id="a8c6a-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a8c6a-120">Application</span></span> | <span data-ttu-id="a8c6a-121">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8c6a-121">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8c6a-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8c6a-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a><span data-ttu-id="a8c6a-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a8c6a-123">Request headers</span></span>
| <span data-ttu-id="a8c6a-124">Name</span><span class="sxs-lookup"><span data-stu-id="a8c6a-124">Name</span></span>       | <span data-ttu-id="a8c6a-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8c6a-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a8c6a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8c6a-126">Authorization</span></span>  | <span data-ttu-id="a8c6a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a8c6a-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="a8c6a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a8c6a-129">Content-Type</span></span>  | <span data-ttu-id="a8c6a-130">application/json</span><span class="sxs-lookup"><span data-stu-id="a8c6a-130">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8c6a-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a8c6a-131">Request body</span></span>
<span data-ttu-id="a8c6a-132">Geben Sie im Anforderungstext eine JSON-Darstellung des [domain](../resources/domain.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a8c6a-132">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

> <span data-ttu-id="a8c6a-p104">Der Anforderungstext enthält die id-Eigenschaft für die neue Domäne. Die id-Eigenschaft ist die einzige Eigenschaft, die angegeben werden kann, und sie ist erforderlich. Der Wert der id-Eigenschaft ist der vollqualifizierte Domänenname, der erstellt werden soll.</span><span class="sxs-lookup"><span data-stu-id="a8c6a-p104">The request body contains the id property for the new domain. Id is the only property that can be specified and it is required. The id property value is the fully qualified domain name to create.</span></span>

## <a name="response"></a><span data-ttu-id="a8c6a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8c6a-136">Response</span></span>

<span data-ttu-id="a8c6a-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [domain](../resources/domain.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8c6a-137">If successful, this method returns `201 Created` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8c6a-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a8c6a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a8c6a-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a8c6a-139">Request</span></span>

<span data-ttu-id="a8c6a-140">Geben Sie im Anforderungstext eine JSON-Darstellung des [domain](../resources/domain.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a8c6a-140">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/v1.0/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a><span data-ttu-id="a8c6a-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="a8c6a-141">Response</span></span>
<span data-ttu-id="a8c6a-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a8c6a-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->