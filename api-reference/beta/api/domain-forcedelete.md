---
title: 'Domäne: ForceDelete'
description: Löscht eine Domäne mithilfe eines asynchronen Vorgangs.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5a1a2b2510f0c79f2be4e70deb9efabc65f8dfc4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527689"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="b8cd2-103">Domäne: ForceDelete</span><span class="sxs-lookup"><span data-stu-id="b8cd2-103">domain: forceDelete</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8cd2-104">Löscht eine Domäne mithilfe eines asynchronen Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-104">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="b8cd2-105">Im Rahmen dieses Vorgangs werden die folgenden Aktionen ausgeführt:</span><span class="sxs-lookup"><span data-stu-id="b8cd2-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="b8cd2-106">Benennt den UPN, EmailAddress und ProxyAddress von Benutzern durch Verweise auf die gelöschte Domäne.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-106">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="b8cd2-107">Benennt das EmailAddress-Gruppen mit Verweisen auf die gelöschte Domäne.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-107">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="b8cd2-108">Benennt die IdentifierUris von Anwendungen mit Verweisen auf die gelöschte Domäne.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-108">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="b8cd2-109">Wenn die Anzahl der Objekte umbenannt werden größer als 1000 ist, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="b8cd2-110">Wenn eine der Anwendungen umbenannt werden eine mehrinstanzenfähige app ist, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-110">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="b8cd2-111">Nach Abschluss der Löschvorgang Domäne gibt API-Vorgänge für die gelöschten Domäne ein 404 HTTP-Antwort-Code zurück.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-111">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="b8cd2-112">Zum Löschen einer Domäne zu bestätigen, können Sie die [erste Domäne](domain-get.md)ausführen.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="b8cd2-113">Wenn die Domäne erfolgreich gelöscht wurde, wird ein 404 HTTP-Antwort-Code in der Antwort zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-113">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8cd2-114">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b8cd2-114">Permissions</span></span>

<span data-ttu-id="b8cd2-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8cd2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b8cd2-117">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8cd2-117">Permission type</span></span>      | <span data-ttu-id="b8cd2-118">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8cd2-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8cd2-119">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8cd2-119">Delegated (work or school account)</span></span> | <span data-ttu-id="b8cd2-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b8cd2-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b8cd2-121">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8cd2-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8cd2-122">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8cd2-122">Not supported.</span></span>    |
|<span data-ttu-id="b8cd2-123">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8cd2-123">Application</span></span> | <span data-ttu-id="b8cd2-124">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8cd2-124">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8cd2-125">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8cd2-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="b8cd2-126">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-126">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8cd2-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8cd2-127">Request headers</span></span>

| <span data-ttu-id="b8cd2-128">Name</span><span class="sxs-lookup"><span data-stu-id="b8cd2-128">Name</span></span>       | <span data-ttu-id="b8cd2-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8cd2-129">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b8cd2-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8cd2-130">Authorization</span></span>  | <span data-ttu-id="b8cd2-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="b8cd2-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b8cd2-133">Content-Type</span></span>  | <span data-ttu-id="b8cd2-134">application/json</span><span class="sxs-lookup"><span data-stu-id="b8cd2-134">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8cd2-135">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8cd2-135">Request body</span></span>

<span data-ttu-id="b8cd2-136">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b8cd2-137">Parameter</span><span class="sxs-lookup"><span data-stu-id="b8cd2-137">Parameter</span></span>    | <span data-ttu-id="b8cd2-138">Typ</span><span class="sxs-lookup"><span data-stu-id="b8cd2-138">Type</span></span>   |<span data-ttu-id="b8cd2-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8cd2-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8cd2-140">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="b8cd2-140">disableUserAccounts</span></span>|<span data-ttu-id="b8cd2-141">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="b8cd2-141">Boolean</span></span>| <span data-ttu-id="b8cd2-142">Option zum Deaktivieren von Benutzerkonten umbenannt.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-142">Option to disable renamed user accounts.</span></span> <span data-ttu-id="b8cd2-143">Wenn ein Benutzerkonto deaktiviert ist, wird der Benutzer nicht zulässig ist so melden Sie sich.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-143">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="b8cd2-144">*"True"* (Standard) - Benutzer, die im Rahmen dieses Vorgangs umbenannte Konten deaktiviert wurden.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-144">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="b8cd2-145">*False* - Benutzerkonten, die im Rahmen dieses Vorgangs umbenannt werden nicht deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-145">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="b8cd2-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8cd2-146">Response</span></span>

<span data-ttu-id="b8cd2-147">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8cd2-147">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="b8cd2-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8cd2-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8cd2-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8cd2-149">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

##### <a name="response"></a><span data-ttu-id="b8cd2-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8cd2-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-forcedelete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
