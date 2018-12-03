---
title: Benutzer erstellen
description: Verwenden Sie diese API, um einen neuen Benutzer zu erstellen.
ms.openlocfilehash: 17df752fb3767e82b72e46857e9ce6a2a8769db7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059235"
---
# <a name="create-user"></a><span data-ttu-id="eaa52-103">Benutzer erstellen</span><span class="sxs-lookup"><span data-stu-id="eaa52-103">Create user</span></span>

> <span data-ttu-id="eaa52-104">**Wichtig:** Die APIs der /beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="eaa52-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaa52-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="eaa52-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eaa52-106">Verwenden Sie diese API, um einen neuen Benutzer zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="eaa52-106">Use this API to create a new user.</span></span>
<span data-ttu-id="eaa52-107">Textkörper der Anforderung enthält den Benutzer zum Erstellen.</span><span class="sxs-lookup"><span data-stu-id="eaa52-107">The request body contains the user to create.</span></span> <span data-ttu-id="eaa52-108">Zumindest müssen Sie die erforderlichen Eigenschaften für den Benutzer angeben.</span><span class="sxs-lookup"><span data-stu-id="eaa52-108">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="eaa52-109">Optional können Sie eine beliebige andere schreibbaren Eigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="eaa52-109">You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="eaa52-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="eaa52-110">Permissions</span></span>
<span data-ttu-id="eaa52-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eaa52-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaa52-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="eaa52-113">Permission type</span></span>      | <span data-ttu-id="eaa52-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="eaa52-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaa52-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="eaa52-115">Delegated (work or school account)</span></span> | <span data-ttu-id="eaa52-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="eaa52-116">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="eaa52-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="eaa52-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaa52-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="eaa52-118">Not supported.</span></span>    |
|<span data-ttu-id="eaa52-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="eaa52-119">Application</span></span> | <span data-ttu-id="eaa52-120">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eaa52-120">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaa52-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="eaa52-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="eaa52-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="eaa52-122">Request headers</span></span>
| <span data-ttu-id="eaa52-123">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="eaa52-123">Header</span></span>       | <span data-ttu-id="eaa52-124">Wert</span><span class="sxs-lookup"><span data-stu-id="eaa52-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eaa52-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaa52-125">Authorization</span></span>  | <span data-ttu-id="eaa52-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="eaa52-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eaa52-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eaa52-128">Content-Type</span></span>  | <span data-ttu-id="eaa52-129">application/json</span><span class="sxs-lookup"><span data-stu-id="eaa52-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eaa52-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="eaa52-130">Request body</span></span>
<span data-ttu-id="eaa52-131">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="eaa52-131">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="eaa52-132">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen eines Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="eaa52-132">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="eaa52-133">Parameter</span><span class="sxs-lookup"><span data-stu-id="eaa52-133">Parameter</span></span> | <span data-ttu-id="eaa52-134">Typ</span><span class="sxs-lookup"><span data-stu-id="eaa52-134">Type</span></span> | <span data-ttu-id="eaa52-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="eaa52-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eaa52-136">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="eaa52-136">accountEnabled</span></span> |<span data-ttu-id="eaa52-137">boolean</span><span class="sxs-lookup"><span data-stu-id="eaa52-137">boolean</span></span> |<span data-ttu-id="eaa52-138">true, wenn das Konto aktiviert ist; andernfalls false.</span><span class="sxs-lookup"><span data-stu-id="eaa52-138">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="eaa52-139">displayName</span><span class="sxs-lookup"><span data-stu-id="eaa52-139">displayName</span></span> |<span data-ttu-id="eaa52-140">string</span><span class="sxs-lookup"><span data-stu-id="eaa52-140">string</span></span> |<span data-ttu-id="eaa52-141">Der Name des Benutzers, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="eaa52-141">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="eaa52-142">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="eaa52-142">onPremisesImmutableId</span></span> |<span data-ttu-id="eaa52-143">string</span><span class="sxs-lookup"><span data-stu-id="eaa52-143">string</span></span> |<span data-ttu-id="eaa52-144">Muss nur angegeben werden, wenn ein neues Benutzerkonto erstellt wird, wenn Sie eine Verbunddomäne für die UserPrincipalName-Eigenschaft (UPN) des Benutzers verwenden.</span><span class="sxs-lookup"><span data-stu-id="eaa52-144">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="eaa52-145">mailNickname</span><span class="sxs-lookup"><span data-stu-id="eaa52-145">mailNickname</span></span> |<span data-ttu-id="eaa52-146">string</span><span class="sxs-lookup"><span data-stu-id="eaa52-146">string</span></span> |<span data-ttu-id="eaa52-147">Der E-Mail-Alias für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="eaa52-147">The mail alias for the user.</span></span>|
|<span data-ttu-id="eaa52-148">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="eaa52-148">passwordProfile</span></span>|[<span data-ttu-id="eaa52-149">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="eaa52-149">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="eaa52-150">Das Kennwortprofil für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="eaa52-150">The password profile for the user.</span></span>|
|<span data-ttu-id="eaa52-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="eaa52-151">userPrincipalName</span></span> |<span data-ttu-id="eaa52-152">string</span><span class="sxs-lookup"><span data-stu-id="eaa52-152">string</span></span> |<span data-ttu-id="eaa52-153">Der Benutzerprinzipalname (someuser@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="eaa52-153">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="eaa52-154">Da die Ressource **Benutzer** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `POST` Vorgang und Hinzufügen von benutzerdefinierten Eigenschaften mit Ihren eigenen Daten auf die Benutzerinstanz beim Erstellen.</span><span class="sxs-lookup"><span data-stu-id="eaa52-154">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="eaa52-155">Antwort</span><span class="sxs-lookup"><span data-stu-id="eaa52-155">Response</span></span>

<span data-ttu-id="eaa52-156">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eaa52-156">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eaa52-157">Beispiel</span><span class="sxs-lookup"><span data-stu-id="eaa52-157">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eaa52-158">Anforderung</span><span class="sxs-lookup"><span data-stu-id="eaa52-158">Request</span></span>
<span data-ttu-id="eaa52-159">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="eaa52-159">Here is an example of the request.</span></span>
<!-- {  
  "blockType": "request",   
  "name": "create_user_from_users_2"    
}-->

```http
POST https://graph.microsoft.com/beta/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value@onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="eaa52-160">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="eaa52-160">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="eaa52-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="eaa52-161">Response</span></span>
<span data-ttu-id="eaa52-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="eaa52-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "id-value",
    "businessPhones": [],
    "displayName": "displayName-value",
    "givenName": null,
    "jobTitle": null,
    "mail": null,
    "mobilePhone": null,
    "officeLocation": null,
    "preferredLanguage": null,
    "surname": null,
    "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com"
}
```

## <a name="see-also"></a><span data-ttu-id="eaa52-165">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="eaa52-165">See also</span></span>

- [<span data-ttu-id="eaa52-166">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="eaa52-166">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="eaa52-167">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="eaa52-167">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="eaa52-168">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="eaa52-168">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
