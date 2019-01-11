---
title: Benutzer erstellen
description: Verwenden Sie diese API, um einen neuen Benutzer zu erstellen.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 218752a382da4ccb2bdbe240c8c57d03007b0169
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851653"
---
# <a name="create-user"></a><span data-ttu-id="3a779-103">Benutzer erstellen</span><span class="sxs-lookup"><span data-stu-id="3a779-103">Create User</span></span>

<span data-ttu-id="3a779-p101">Verwenden Sie diese API zum Erstellen eines neuen Benutzers. Der Anforderungstext enthält den zu erstellenden Benutzer. Sie müssen für den Benutzer mindestens die erforderlichen Eigenschaften angeben. Optional können Sie weitere schreibbare Eigenschaften festlegen.</span><span class="sxs-lookup"><span data-stu-id="3a779-p101">Use this API to create a new User. The request body contains the user to create. At a minimum, you must specify the required properties for the user. You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="3a779-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3a779-108">Permissions</span></span>
<span data-ttu-id="3a779-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a779-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a779-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3a779-111">Permission type</span></span>      | <span data-ttu-id="3a779-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3a779-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a779-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3a779-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3a779-114">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3a779-114">User.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3a779-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3a779-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a779-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3a779-116">Not supported.</span></span>    |
|<span data-ttu-id="3a779-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3a779-117">Application</span></span> | <span data-ttu-id="3a779-118">User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a779-118">User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a779-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a779-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="3a779-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3a779-120">Request headers</span></span>
| <span data-ttu-id="3a779-121">Header</span><span class="sxs-lookup"><span data-stu-id="3a779-121">Header</span></span>       | <span data-ttu-id="3a779-122">Wert</span><span class="sxs-lookup"><span data-stu-id="3a779-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3a779-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a779-123">Authorization</span></span>  | <span data-ttu-id="3a779-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3a779-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3a779-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a779-126">Content-Type</span></span>  | <span data-ttu-id="3a779-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3a779-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3a779-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3a779-128">Request body</span></span>
<span data-ttu-id="3a779-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3a779-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="3a779-130">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen eines Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="3a779-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="3a779-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="3a779-131">Parameter</span></span> | <span data-ttu-id="3a779-132">Typ</span><span class="sxs-lookup"><span data-stu-id="3a779-132">Type</span></span> | <span data-ttu-id="3a779-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3a779-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a779-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="3a779-134">accountEnabled</span></span> |<span data-ttu-id="3a779-135">boolean</span><span class="sxs-lookup"><span data-stu-id="3a779-135">boolean</span></span> |<span data-ttu-id="3a779-136">true, wenn das Konto aktiviert ist; andernfalls false.</span><span class="sxs-lookup"><span data-stu-id="3a779-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="3a779-137">displayName</span><span class="sxs-lookup"><span data-stu-id="3a779-137">displayName</span></span> |<span data-ttu-id="3a779-138">string</span><span class="sxs-lookup"><span data-stu-id="3a779-138">string</span></span> |<span data-ttu-id="3a779-139">Der Name des Benutzers, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="3a779-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="3a779-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="3a779-140">onPremisesImmutableId</span></span> |<span data-ttu-id="3a779-141">string</span><span class="sxs-lookup"><span data-stu-id="3a779-141">string</span></span> |<span data-ttu-id="3a779-142">Muss nur angegeben werden, wenn ein neues Benutzerkonto erstellt wird, wenn Sie eine Verbunddomäne für die UserPrincipalName-Eigenschaft (UPN) des Benutzers verwenden.</span><span class="sxs-lookup"><span data-stu-id="3a779-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="3a779-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="3a779-143">mailNickname</span></span> |<span data-ttu-id="3a779-144">string</span><span class="sxs-lookup"><span data-stu-id="3a779-144">string</span></span> |<span data-ttu-id="3a779-145">Der E-Mail-Alias für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="3a779-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="3a779-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="3a779-146">passwordProfile</span></span>|[<span data-ttu-id="3a779-147">PasswordProfile</span><span class="sxs-lookup"><span data-stu-id="3a779-147">PasswordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="3a779-148">Das Kennwortprofil für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="3a779-148">The password profile for the user.</span></span>|
|<span data-ttu-id="3a779-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3a779-149">userPrincipalName</span></span> |<span data-ttu-id="3a779-150">string</span><span class="sxs-lookup"><span data-stu-id="3a779-150">string</span></span> |<span data-ttu-id="3a779-151">Der Benutzerprinzipalname (someuser@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="3a779-151">The user principal name (someuser@contoso.com).</span></span>|

## <a name="response"></a><span data-ttu-id="3a779-152">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a779-152">Response</span></span>

<span data-ttu-id="3a779-153">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a779-153">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a779-154">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3a779-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3a779-155">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3a779-155">Request</span></span>
<span data-ttu-id="3a779-156">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3a779-156">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled": true,
  "displayName": "displayName-value",
  "mailNickname": "mailNickname-value",
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="3a779-157">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3a779-157">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3a779-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="3a779-158">Response</span></span>
<span data-ttu-id="3a779-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3a779-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
