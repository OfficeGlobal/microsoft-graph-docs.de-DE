---
title: Domäne löschen erzwingen
description: Löscht eine Domäne mithilfe eines asynchronen Vorgangs langer.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bbf56fdd2f623a918b43298626bd08269ad922ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918427"
---
# <a name="force-domain-deletion"></a><span data-ttu-id="3299e-103">Domäne löschen erzwingen</span><span class="sxs-lookup"><span data-stu-id="3299e-103">Force domain deletion</span></span>

<span data-ttu-id="3299e-104">Löscht eine Domäne mithilfe eines asynchronen Vorgangs langer.</span><span class="sxs-lookup"><span data-stu-id="3299e-104">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="3299e-105">Im Rahmen dieses Vorgangs werden die folgenden Aktionen ausgeführt:</span><span class="sxs-lookup"><span data-stu-id="3299e-105">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="3299e-106">Updates der `userPrincipalName`, `mail`, und `proxyAddresses` Eigenschaften des `users` durch Verweise auf die gelöschte Domäne die Domäne der anfänglichen "onmicrosoft.com" verwenden.</span><span class="sxs-lookup"><span data-stu-id="3299e-106">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="3299e-107">Updates der `mail` -Eigenschaft des `groups` durch Verweise auf die gelöschte Domäne die Domäne der anfänglichen "onmicrosoft.com" verwenden.</span><span class="sxs-lookup"><span data-stu-id="3299e-107">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="3299e-108">Updates der `identifierUris` -Eigenschaft des `applications` durch Verweise auf die gelöschte Domäne die Domäne der anfänglichen "onmicrosoft.com" verwenden.</span><span class="sxs-lookup"><span data-stu-id="3299e-108">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="3299e-109">Wenn die Anzahl der Objekte umbenannt werden größer als 1000 ist, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3299e-109">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="3299e-110">Wenn eine von der `applications` umbenannt werden, ist eine app mit mehreren Mandanten, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3299e-110">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="3299e-111">Nach Abschluss der Löschvorgang Domäne gibt API-Vorgänge für die gelöschten Domäne einen HTTP 404-Statuscode zurück.</span><span class="sxs-lookup"><span data-stu-id="3299e-111">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="3299e-112">Zum Löschen einer Domäne zu bestätigen, können Sie einen Vorgang [Abrufen Domäne](domain-get.md) ausführen.</span><span class="sxs-lookup"><span data-stu-id="3299e-112">To verify deletion of a domain, you can perform a [get domain](domain-get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="3299e-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3299e-113">Permissions</span></span>

<span data-ttu-id="3299e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3299e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3299e-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3299e-116">Permission type</span></span>      | <span data-ttu-id="3299e-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3299e-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3299e-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3299e-118">Delegated (work or school account)</span></span> | <span data-ttu-id="3299e-119">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3299e-119">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3299e-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3299e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3299e-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3299e-121">Not supported.</span></span>    |
|<span data-ttu-id="3299e-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3299e-122">Application</span></span> | <span data-ttu-id="3299e-123">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3299e-123">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3299e-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3299e-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="3299e-125">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="3299e-125">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3299e-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3299e-126">Request headers</span></span>

| <span data-ttu-id="3299e-127">Name</span><span class="sxs-lookup"><span data-stu-id="3299e-127">Name</span></span> | <span data-ttu-id="3299e-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3299e-128">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3299e-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="3299e-129">Authorization</span></span>  | <span data-ttu-id="3299e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3299e-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="3299e-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3299e-132">Content-Type</span></span>  | <span data-ttu-id="3299e-133">application/json</span><span class="sxs-lookup"><span data-stu-id="3299e-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3299e-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3299e-134">Request body</span></span>

<span data-ttu-id="3299e-135">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="3299e-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3299e-136">Parameter</span><span class="sxs-lookup"><span data-stu-id="3299e-136">Parameter</span></span> | <span data-ttu-id="3299e-137">Typ</span><span class="sxs-lookup"><span data-stu-id="3299e-137">Type</span></span> | <span data-ttu-id="3299e-138">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3299e-138">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="3299e-139">Option zum Deaktivieren von Benutzerkonten die umbenannt werden.</span><span class="sxs-lookup"><span data-stu-id="3299e-139">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="3299e-140">Wenn ein Benutzerkonto deaktiviert ist, wird der Benutzer nicht zulässig ist so melden Sie sich.</span><span class="sxs-lookup"><span data-stu-id="3299e-140">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="3299e-141">Wenn auf **true** festgelegt, die `users` als Teil von diesem Vorgang wird deaktiviert werden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="3299e-141">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="3299e-142">Standardwert ist **true**.</span><span class="sxs-lookup"><span data-stu-id="3299e-142">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="3299e-143">Antworttext</span><span class="sxs-lookup"><span data-stu-id="3299e-143">Response body</span></span>

<span data-ttu-id="3299e-144">Wenn der Vorgang erfolgreich war, gibt diese Methode `HTTP/1.1 204 OK` Statuscode.</span><span class="sxs-lookup"><span data-stu-id="3299e-144">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="3299e-145">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3299e-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="3299e-146">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3299e-146">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="3299e-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="3299e-147">Response</span></span>

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
