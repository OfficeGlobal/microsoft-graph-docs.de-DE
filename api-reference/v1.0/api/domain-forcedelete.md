---
title: Domäne löschen erzwingen
description: Löscht eine Domäne mithilfe eines asynchronen Vorgangs langer.
ms.openlocfilehash: 20f00679998070b95af65292cadf83d76aa2add1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019940"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="4d36f-103">Domäne löschen erzwingen</span><span class="sxs-lookup"><span data-stu-id="4d36f-103">Force domain deletion</span></span>

<span data-ttu-id="4d36f-104">Löscht eine Domäne mithilfe eines asynchronen Vorgangs langer.</span><span class="sxs-lookup"><span data-stu-id="4d36f-104">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="4d36f-105">Im Rahmen dieses Vorgangs werden die folgenden Aktionen ausgeführt:</span><span class="sxs-lookup"><span data-stu-id="4d36f-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="4d36f-106">Updates der `userPrincipalName`, `mail`, und `proxyAddresses` Eigenschaften des `users` durch Verweise auf die gelöschte Domäne die Domäne der anfänglichen "onmicrosoft.com" verwenden.</span><span class="sxs-lookup"><span data-stu-id="4d36f-106">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="4d36f-107">Updates der `mail` -Eigenschaft des `groups` durch Verweise auf die gelöschte Domäne die Domäne der anfänglichen "onmicrosoft.com" verwenden.</span><span class="sxs-lookup"><span data-stu-id="4d36f-107">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="4d36f-108">Updates der `identifierUris` -Eigenschaft des `applications` durch Verweise auf die gelöschte Domäne die Domäne der anfänglichen "onmicrosoft.com" verwenden.</span><span class="sxs-lookup"><span data-stu-id="4d36f-108">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="4d36f-109">Wenn die Anzahl der Objekte umbenannt werden größer als 1000 ist, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d36f-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="4d36f-110">Wenn eine von der `applications` umbenannt werden, ist eine app mit mehreren Mandanten, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d36f-110">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="4d36f-111">Nach Abschluss der Löschvorgang Domäne gibt API-Vorgänge für die gelöschten Domäne einen HTTP 404-Statuscode zurück.</span><span class="sxs-lookup"><span data-stu-id="4d36f-111">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="4d36f-112">Zum Löschen einer Domäne zu bestätigen, können Sie einen Vorgang [Abrufen Domäne](domain-get.md) ausführen.</span><span class="sxs-lookup"><span data-stu-id="4d36f-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d36f-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4d36f-113">Permissions</span></span>

<span data-ttu-id="4d36f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d36f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d36f-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d36f-116">Permission type</span></span>      | <span data-ttu-id="4d36f-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d36f-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d36f-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d36f-118">Delegated (work or school account)</span></span> | <span data-ttu-id="4d36f-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4d36f-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4d36f-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d36f-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d36f-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d36f-121">Not supported.</span></span>    |
|<span data-ttu-id="4d36f-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d36f-122">Application</span></span> | <span data-ttu-id="4d36f-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d36f-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d36f-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d36f-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="4d36f-125">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="4d36f-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d36f-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d36f-126">Request headers</span></span>

| <span data-ttu-id="4d36f-127">Name</span><span class="sxs-lookup"><span data-stu-id="4d36f-127">Name</span></span> | <span data-ttu-id="4d36f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d36f-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4d36f-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d36f-129">Authorization</span></span>  | <span data-ttu-id="4d36f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d36f-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="4d36f-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d36f-132">Content-Type</span></span>  | <span data-ttu-id="4d36f-133">application/json</span><span class="sxs-lookup"><span data-stu-id="4d36f-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d36f-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d36f-134">Request body</span></span>

<span data-ttu-id="4d36f-135">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="4d36f-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4d36f-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="4d36f-136">Parameter</span></span> | <span data-ttu-id="4d36f-137">Typ</span><span class="sxs-lookup"><span data-stu-id="4d36f-137">Type</span></span> | <span data-ttu-id="4d36f-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4d36f-138">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="4d36f-139">Option zum Deaktivieren von Benutzerkonten die umbenannt werden.</span><span class="sxs-lookup"><span data-stu-id="4d36f-139">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="4d36f-140">Wenn ein Benutzerkonto deaktiviert ist, wird der Benutzer nicht zulässig ist so melden Sie sich.</span><span class="sxs-lookup"><span data-stu-id="4d36f-140">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="4d36f-141">Wenn auf **true** festgelegt, die `users` als Teil von diesem Vorgang wird deaktiviert werden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="4d36f-141">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="4d36f-142">Standardwert ist **true**.</span><span class="sxs-lookup"><span data-stu-id="4d36f-142">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="4d36f-143">Antworttext</span><span class="sxs-lookup"><span data-stu-id="4d36f-143">Response body</span></span>

<span data-ttu-id="4d36f-144">Wenn der Vorgang erfolgreich war, gibt diese Methode `HTTP/1.1 204 OK` Statuscode.</span><span class="sxs-lookup"><span data-stu-id="4d36f-144">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="4d36f-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d36f-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="4d36f-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d36f-146">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "domain_forcedelete"
}-->

```http
POST https://graph.microsoft.com/beta/domains/{id}/forceDelete
Content-type: application/json
Content-length: 33

{
  "disableUserAccounts": true
}
```

### <a name="response"></a><span data-ttu-id="4d36f-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d36f-147">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 OK
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