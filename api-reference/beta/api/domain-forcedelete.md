---
title: 'Domäne: ForceDelete'
description: Löscht eine Domäne mithilfe eines asynchronen Vorgangs.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6c3d942352a0db20d6e46a4b00686ad948bd6798
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965124"
---
# <a name="domain-forcedelete"></a><span data-ttu-id="1fa3f-103">Domäne: ForceDelete</span><span class="sxs-lookup"><span data-stu-id="1fa3f-103">domain: forceDelete</span></span>

> <span data-ttu-id="1fa3f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fa3f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1fa3f-106">Löscht eine Domäne mithilfe eines asynchronen Vorgangs.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-106">Deletes a domain using an asynchronous operation.</span></span>

<span data-ttu-id="1fa3f-107">Im Rahmen dieses Vorgangs werden die folgenden Aktionen ausgeführt:</span><span class="sxs-lookup"><span data-stu-id="1fa3f-107">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="1fa3f-108">Benennt den UPN, EmailAddress und ProxyAddress von Benutzern durch Verweise auf die gelöschte Domäne.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-108">Renames the UPN, EmailAddress, and ProxyAddress of users with references to the deleted domain.</span></span>

* <span data-ttu-id="1fa3f-109">Benennt das EmailAddress-Gruppen mit Verweisen auf die gelöschte Domäne.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-109">Renames the EmailAddress of groups with references to the deleted domain.</span></span>

* <span data-ttu-id="1fa3f-110">Benennt die IdentifierUris von Anwendungen mit Verweisen auf die gelöschte Domäne.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-110">Renames the identifierUris of applications with references to the deleted domain.</span></span>

* <span data-ttu-id="1fa3f-111">Wenn die Anzahl der Objekte umbenannt werden größer als 1000 ist, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-111">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="1fa3f-112">Wenn eine der Anwendungen umbenannt werden eine mehrinstanzenfähige app ist, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-112">If one of the applications to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="1fa3f-113">Nach Abschluss der Löschvorgang Domäne gibt API-Vorgänge für die gelöschten Domäne ein 404 HTTP-Antwort-Code zurück.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-113">After the domain deletion completes, API operations for the deleted domain will return a 404 HTTP response code.</span></span> <span data-ttu-id="1fa3f-114">Zum Löschen einer Domäne zu bestätigen, können Sie die [erste Domäne](domain-get.md)ausführen.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-114">To verify deletion of a domain, you can perform a [get domain](domain-get.md).</span></span> <span data-ttu-id="1fa3f-115">Wenn die Domäne erfolgreich gelöscht wurde, wird ein 404 HTTP-Antwort-Code in der Antwort zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-115">If the domain was successfully deleted, a 404 HTTP response code will be returned in the response.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fa3f-116">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1fa3f-116">Permissions</span></span>

<span data-ttu-id="1fa3f-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fa3f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1fa3f-119">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1fa3f-119">Permission type</span></span>      | <span data-ttu-id="1fa3f-120">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1fa3f-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fa3f-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1fa3f-121">Delegated (work or school account)</span></span> | <span data-ttu-id="1fa3f-122">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1fa3f-122">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1fa3f-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1fa3f-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fa3f-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1fa3f-124">Not supported.</span></span>    |
|<span data-ttu-id="1fa3f-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1fa3f-125">Application</span></span> | <span data-ttu-id="1fa3f-126">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa3f-126">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fa3f-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1fa3f-127">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="1fa3f-128">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-128">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fa3f-129">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1fa3f-129">Request headers</span></span>

| <span data-ttu-id="1fa3f-130">Name</span><span class="sxs-lookup"><span data-stu-id="1fa3f-130">Name</span></span>       | <span data-ttu-id="1fa3f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1fa3f-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1fa3f-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fa3f-132">Authorization</span></span>  | <span data-ttu-id="1fa3f-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="1fa3f-135">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1fa3f-135">Content-Type</span></span>  | <span data-ttu-id="1fa3f-136">application/json</span><span class="sxs-lookup"><span data-stu-id="1fa3f-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fa3f-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1fa3f-137">Request body</span></span>

<span data-ttu-id="1fa3f-138">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1fa3f-139">Parameter</span><span class="sxs-lookup"><span data-stu-id="1fa3f-139">Parameter</span></span>    | <span data-ttu-id="1fa3f-140">Typ</span><span class="sxs-lookup"><span data-stu-id="1fa3f-140">Type</span></span>   |<span data-ttu-id="1fa3f-141">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1fa3f-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fa3f-142">disableUserAccounts</span><span class="sxs-lookup"><span data-stu-id="1fa3f-142">disableUserAccounts</span></span>|<span data-ttu-id="1fa3f-143">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="1fa3f-143">Boolean</span></span>| <span data-ttu-id="1fa3f-144">Option zum Deaktivieren von Benutzerkonten umbenannt.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-144">Option to disable renamed user accounts.</span></span> <span data-ttu-id="1fa3f-145">Wenn ein Benutzerkonto deaktiviert ist, wird der Benutzer nicht zulässig ist so melden Sie sich.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-145">If a user account is disabled, the user will not be allowed to sign in.</span></span><br><span data-ttu-id="1fa3f-146">*"True"* (Standard) - Benutzer, die im Rahmen dieses Vorgangs umbenannte Konten deaktiviert wurden.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-146">*True* (default) - User accounts renamed as part of this operation are disabled.</span></span><br><span data-ttu-id="1fa3f-147">*False* - Benutzerkonten, die im Rahmen dieses Vorgangs umbenannt werden nicht deaktiviert.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-147">*False* - User accounts renamed as part of this operation are not disabled.</span></span> |

## <a name="response"></a><span data-ttu-id="1fa3f-148">Antwort</span><span class="sxs-lookup"><span data-stu-id="1fa3f-148">Response</span></span>

<span data-ttu-id="1fa3f-149">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `200 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1fa3f-149">If successful, this method returns `200 OK` response code.</span></span> 

## <a name="example"></a><span data-ttu-id="1fa3f-150">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1fa3f-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1fa3f-151">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1fa3f-151">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="1fa3f-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="1fa3f-152">Response</span></span>

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
