---
title: 'Domäne: ForceDelete'
description: Löscht eine Domäne mithilfe eines asynchronen Vorgangs.
author: lleonard-msft
ms.openlocfilehash: 4af5b70fca7600538d4212768243d8de82eb79ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316212"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="871d8-103">Domäne: ForceDelete</span><span class="sxs-lookup"><span data-stu-id="871d8-103">domain: forceDelete</span></span>

> <span data-ttu-id="871d8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="871d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="871d8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="871d8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="871d8-106">Löscht eine Domäne mithilfe eines asynchronen Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="871d8-106">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="871d8-107">Im Rahmen dieses Vorgangs werden die folgenden Aktionen ausgeführt:</span><span class="sxs-lookup"><span data-stu-id="871d8-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="871d8-108">Benennt den UPN, EmailAddress und ProxyAddress von Benutzern durch Verweise auf die gelöschte Domäne.</span><span class="sxs-lookup"><span data-stu-id="871d8-108">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="871d8-109">Benennt das EmailAddress-Gruppen mit Verweisen auf die gelöschte Domäne.</span><span class="sxs-lookup"><span data-stu-id="871d8-109">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="871d8-110">Benennt die IdentifierUris von Anwendungen mit Verweisen auf die gelöschte Domäne.</span><span class="sxs-lookup"><span data-stu-id="871d8-110">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="871d8-111">Wenn die Anzahl der Objekte umbenannt werden größer als 1000 ist, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="871d8-111">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="871d8-112">Wenn eine der Anwendungen umbenannt werden eine mehrinstanzenfähige app ist, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="871d8-112">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="871d8-113">Nach Abschluss der Löschvorgang Domäne gibt API-Vorgänge für die gelöschten Domäne ein 404 HTTP-Antwort-Code zurück.</span><span class="sxs-lookup"><span data-stu-id="871d8-113">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="871d8-114">Zum Löschen einer Domäne zu bestätigen, können Sie die [erste Domäne](domain-get.md)ausführen.</span><span class="sxs-lookup"><span data-stu-id="871d8-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="871d8-115">Wenn die Domäne erfolgreich gelöscht wurde, wird ein 404 HTTP-Antwort-Code in der Antwort zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="871d8-115">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="871d8-116">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="871d8-116">Permissions</span></span>

<span data-ttu-id="871d8-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="871d8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="871d8-119">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="871d8-119">Permission type</span></span>      | <span data-ttu-id="871d8-120">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="871d8-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="871d8-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="871d8-121">Delegated (work or school account)</span></span> | <span data-ttu-id="871d8-122">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="871d8-122">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="871d8-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="871d8-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="871d8-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="871d8-124">Not supported.</span></span>    |
|<span data-ttu-id="871d8-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="871d8-125">Application</span></span> | <span data-ttu-id="871d8-126">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="871d8-126">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="871d8-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="871d8-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="871d8-128">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="871d8-128">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="871d8-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="871d8-129">Request headers</span></span>

| <span data-ttu-id="871d8-130">Name</span><span class="sxs-lookup"><span data-stu-id="871d8-130">Name</span></span>       | <span data-ttu-id="871d8-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="871d8-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="871d8-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="871d8-132">Authorization</span></span>  | <span data-ttu-id="871d8-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="871d8-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="871d8-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="871d8-135">Content-Type</span></span>  | <span data-ttu-id="871d8-136">application/json</span><span class="sxs-lookup"><span data-stu-id="871d8-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="871d8-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="871d8-137">Request body</span></span>

<span data-ttu-id="871d8-138">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="871d8-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="871d8-139">Parameter</span><span class="sxs-lookup"><span data-stu-id="871d8-139">Parameter</span></span>    | <span data-ttu-id="871d8-140">Typ</span><span class="sxs-lookup"><span data-stu-id="871d8-140">Type</span></span>   |<span data-ttu-id="871d8-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="871d8-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="871d8-142">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="871d8-142">disableUserAccounts</span></span>|<span data-ttu-id="871d8-143">Boolesch</span><span class="sxs-lookup"><span data-stu-id="871d8-143">Boolean</span></span>| <span data-ttu-id="871d8-144">Option zum Deaktivieren von Benutzerkonten umbenannt.</span><span class="sxs-lookup"><span data-stu-id="871d8-144">Option to disable renamed user accounts.</span></span> <span data-ttu-id="871d8-145">Wenn ein Benutzerkonto deaktiviert ist, wird der Benutzer nicht zulässig ist so melden Sie sich.</span><span class="sxs-lookup"><span data-stu-id="871d8-145">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="871d8-146">*"True"* (Standard) - Benutzer, die im Rahmen dieses Vorgangs umbenannte Konten deaktiviert wurden.</span><span class="sxs-lookup"><span data-stu-id="871d8-146">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="871d8-147">*False* - Benutzerkonten, die im Rahmen dieses Vorgangs umbenannt werden nicht deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="871d8-147">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="871d8-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="871d8-148">Response</span></span>

<span data-ttu-id="871d8-149">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="871d8-149">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="871d8-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="871d8-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="871d8-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="871d8-151">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="871d8-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="871d8-152">Response</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domain: forcedelete",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->