# <a name="force-domain-deletion"></a><span data-ttu-id="e4605-101">Domäne löschen erzwingen</span><span class="sxs-lookup"><span data-stu-id="e4605-101">Force domain deletion</span></span>

<span data-ttu-id="e4605-102">Löscht eine Domäne mithilfe eines asynchronen Vorgangs langer.</span><span class="sxs-lookup"><span data-stu-id="e4605-102">Deletes a domain using an asynchronous long-running operation.</span></span>

<span data-ttu-id="e4605-103">Im Rahmen dieses Vorgangs werden die folgenden Aktionen ausgeführt:</span><span class="sxs-lookup"><span data-stu-id="e4605-103">The following actions are performed as part of this operation:</span></span>

* <span data-ttu-id="e4605-104">Updates der `userPrincipalName`, `mail`, und `proxyAddresses` Eigenschaften des `users` durch Verweise auf die gelöschte Domäne die Domäne der anfänglichen "onmicrosoft.com" verwenden.</span><span class="sxs-lookup"><span data-stu-id="e4605-104">Updates the `userPrincipalName`, `mail`, and `proxyAddresses` properties of `users` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="e4605-105">Updates der `mail` -Eigenschaft des `groups` durch Verweise auf die gelöschte Domäne die Domäne der anfänglichen "onmicrosoft.com" verwenden.</span><span class="sxs-lookup"><span data-stu-id="e4605-105">Updates the `mail` property of `groups` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="e4605-106">Updates der `identifierUris` -Eigenschaft des `applications` durch Verweise auf die gelöschte Domäne die Domäne der anfänglichen "onmicrosoft.com" verwenden.</span><span class="sxs-lookup"><span data-stu-id="e4605-106">Updates the `identifierUris` property of `applications` with references to the deleted domain to use the initial onmicrosoft.com domain.</span></span>

* <span data-ttu-id="e4605-107">Wenn die Anzahl der Objekte umbenannt werden größer als 1000 ist, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4605-107">If the number of objects to be renamed is greater than 1000, an error is returned.</span></span>

* <span data-ttu-id="e4605-108">Wenn eine von der `applications` umbenannt werden, ist eine app mit mehreren Mandanten, wird ein Fehler zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e4605-108">If one of the `applications` to be renamed is a multi-tenant app, an error is returned.</span></span>

<span data-ttu-id="e4605-109">Nach Abschluss der Löschvorgang Domäne gibt API-Vorgänge für die gelöschten Domäne einen HTTP 404-Statuscode zurück.</span><span class="sxs-lookup"><span data-stu-id="e4605-109">After the domain deletion completes, API operations for the deleted domain will return a HTTP 404 status code.</span></span> <span data-ttu-id="e4605-110">Zum Löschen einer Domäne zu bestätigen, können Sie einen Vorgang [Abrufen Domäne](domain_get.md) ausführen.</span><span class="sxs-lookup"><span data-stu-id="e4605-110">To verify deletion of a domain, you can perform a [get domain](domain_get.md) operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4605-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e4605-111">Permissions</span></span>

<span data-ttu-id="e4605-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e4605-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e4605-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e4605-114">Permission type</span></span>      | <span data-ttu-id="e4605-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e4605-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4605-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e4605-116">Delegated (work or school account)</span></span> | <span data-ttu-id="e4605-117">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e4605-117">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e4605-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e4605-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4605-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e4605-119">Not supported.</span></span>    |
|<span data-ttu-id="e4605-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e4605-120">Application</span></span> | <span data-ttu-id="e4605-121">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4605-121">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4605-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4605-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /domains/{id}/forceDelete
```

> <span data-ttu-id="e4605-123">Geben Sie für {id} die Domäne mit ihrem vollqualifizierten Domänennamen an.</span><span class="sxs-lookup"><span data-stu-id="e4605-123">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4605-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e4605-124">Request headers</span></span>

| <span data-ttu-id="e4605-125">Name</span><span class="sxs-lookup"><span data-stu-id="e4605-125">Name</span></span> | <span data-ttu-id="e4605-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4605-126">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="e4605-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4605-127">Authorization</span></span>  | <span data-ttu-id="e4605-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e4605-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e4605-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4605-130">Content-Type</span></span>  | <span data-ttu-id="e4605-131">application/json</span><span class="sxs-lookup"><span data-stu-id="e4605-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4605-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e4605-132">Request body</span></span>

<span data-ttu-id="e4605-133">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="e4605-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e4605-134">Parameter</span><span class="sxs-lookup"><span data-stu-id="e4605-134">Parameter</span></span> | <span data-ttu-id="e4605-135">Typ</span><span class="sxs-lookup"><span data-stu-id="e4605-135">Type</span></span> | <span data-ttu-id="e4605-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e4605-136">Description</span></span> |
|:---------------|:--------|:----------|
|`disableUserAccounts`|`Boolean`| <span data-ttu-id="e4605-137">Option zum Deaktivieren von Benutzerkonten die umbenannt werden.</span><span class="sxs-lookup"><span data-stu-id="e4605-137">Option to disable user accounts which are renamed.</span></span> <span data-ttu-id="e4605-138">Wenn ein Benutzerkonto deaktiviert ist, wird der Benutzer nicht zulässig ist so melden Sie sich.</span><span class="sxs-lookup"><span data-stu-id="e4605-138">If a user account is disabled, the user will not be allowed to sign in.</span></span> <span data-ttu-id="e4605-139">Wenn auf **true** festgelegt, die `users` als Teil von diesem Vorgang wird deaktiviert werden aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="e4605-139">If set to **true** the `users` updated as part of this operation will be disabled.</span></span>  <span data-ttu-id="e4605-140">Standardwert ist **true**.</span><span class="sxs-lookup"><span data-stu-id="e4605-140">Default value is **true**.</span></span> |

## <a name="response-body"></a><span data-ttu-id="e4605-141">Antworttext</span><span class="sxs-lookup"><span data-stu-id="e4605-141">Response body</span></span>

<span data-ttu-id="e4605-142">Wenn der Vorgang erfolgreich war, gibt diese Methode `HTTP/1.1 204 OK` Statuscode.</span><span class="sxs-lookup"><span data-stu-id="e4605-142">If successful, this method returns `HTTP/1.1 204 OK` status code.</span></span>

## <a name="example"></a><span data-ttu-id="e4605-143">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e4605-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4605-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e4605-144">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="e4605-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="e4605-145">Response</span></span>

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