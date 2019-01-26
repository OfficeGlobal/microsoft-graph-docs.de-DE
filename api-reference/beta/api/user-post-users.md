---
title: Benutzer erstellen
description: Verwenden Sie diese API, um einen neuen Benutzer zu erstellen.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 04ae713cca285bd9fc16c3957ea1ca71dfea01a6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574089"
---
# <a name="create-user"></a><span data-ttu-id="ec626-103">Benutzer erstellen</span><span class="sxs-lookup"><span data-stu-id="ec626-103">Create user</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec626-104">Verwenden Sie diese API, um einen neuen Benutzer zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="ec626-104">Use this API to create a new user.</span></span>
<span data-ttu-id="ec626-105">Textkörper der Anforderung enthält den Benutzer zum Erstellen.</span><span class="sxs-lookup"><span data-stu-id="ec626-105">The request body contains the user to create.</span></span> <span data-ttu-id="ec626-106">Zumindest müssen Sie die erforderlichen Eigenschaften für den Benutzer angeben.</span><span class="sxs-lookup"><span data-stu-id="ec626-106">At a minimum, you must specify the required properties for the user.</span></span> <span data-ttu-id="ec626-107">Optional können Sie eine beliebige andere schreibbaren Eigenschaften angeben.</span><span class="sxs-lookup"><span data-stu-id="ec626-107">You can optionally specify any other writable properties.</span></span>
## <a name="permissions"></a><span data-ttu-id="ec626-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ec626-108">Permissions</span></span>
<span data-ttu-id="ec626-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec626-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec626-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ec626-111">Permission type</span></span>      | <span data-ttu-id="ec626-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ec626-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec626-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ec626-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ec626-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ec626-114">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ec626-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ec626-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec626-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ec626-116">Not supported.</span></span>    |
|<span data-ttu-id="ec626-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ec626-117">Application</span></span> | <span data-ttu-id="ec626-118">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec626-118">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec626-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec626-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users
```
## <a name="request-headers"></a><span data-ttu-id="ec626-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ec626-120">Request headers</span></span>
| <span data-ttu-id="ec626-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ec626-121">Header</span></span>       | <span data-ttu-id="ec626-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ec626-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ec626-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec626-123">Authorization</span></span>  | <span data-ttu-id="ec626-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ec626-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ec626-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ec626-126">Content-Type</span></span>  | <span data-ttu-id="ec626-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ec626-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ec626-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ec626-128">Request body</span></span>
<span data-ttu-id="ec626-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ec626-129">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>

<span data-ttu-id="ec626-130">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Erstellen eines Benutzers erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="ec626-130">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="ec626-131">Parameter</span><span class="sxs-lookup"><span data-stu-id="ec626-131">Parameter</span></span> | <span data-ttu-id="ec626-132">Typ</span><span class="sxs-lookup"><span data-stu-id="ec626-132">Type</span></span> | <span data-ttu-id="ec626-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ec626-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ec626-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="ec626-134">accountEnabled</span></span> |<span data-ttu-id="ec626-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="ec626-135">boolean</span></span> |<span data-ttu-id="ec626-136">true, wenn das Konto aktiviert ist; andernfalls false.</span><span class="sxs-lookup"><span data-stu-id="ec626-136">true if the account is enabled; otherwise, false.</span></span>|
|<span data-ttu-id="ec626-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ec626-137">displayName</span></span> |<span data-ttu-id="ec626-138">string</span><span class="sxs-lookup"><span data-stu-id="ec626-138">string</span></span> |<span data-ttu-id="ec626-139">Der Name des Benutzers, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="ec626-139">The name to display in the address book for the user.</span></span>|
|<span data-ttu-id="ec626-140">onPremisesImmutableId</span><span class="sxs-lookup"><span data-stu-id="ec626-140">onPremisesImmutableId</span></span> |<span data-ttu-id="ec626-141">string</span><span class="sxs-lookup"><span data-stu-id="ec626-141">string</span></span> |<span data-ttu-id="ec626-142">Muss nur angegeben werden, wenn ein neues Benutzerkonto erstellt wird, wenn Sie eine Verbunddomäne für die UserPrincipalName-Eigenschaft (UPN) des Benutzers verwenden.</span><span class="sxs-lookup"><span data-stu-id="ec626-142">Only needs to be specified when creating a new user account if you are using a federated domain for the user's userPrincipalName (UPN) property.</span></span>|
|<span data-ttu-id="ec626-143">mailNickname</span><span class="sxs-lookup"><span data-stu-id="ec626-143">mailNickname</span></span> |<span data-ttu-id="ec626-144">string</span><span class="sxs-lookup"><span data-stu-id="ec626-144">string</span></span> |<span data-ttu-id="ec626-145">Der E-Mail-Alias für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="ec626-145">The mail alias for the user.</span></span>|
|<span data-ttu-id="ec626-146">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="ec626-146">passwordProfile</span></span>|[<span data-ttu-id="ec626-147">passwordProfile</span><span class="sxs-lookup"><span data-stu-id="ec626-147">passwordProfile</span></span>](../resources/passwordprofile.md) |<span data-ttu-id="ec626-148">Das Kennwortprofil für den Benutzer.</span><span class="sxs-lookup"><span data-stu-id="ec626-148">The password profile for the user.</span></span>|
|<span data-ttu-id="ec626-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ec626-149">userPrincipalName</span></span> |<span data-ttu-id="ec626-150">string</span><span class="sxs-lookup"><span data-stu-id="ec626-150">string</span></span> |<span data-ttu-id="ec626-151">Der Benutzerprinzipalname (someuser@contoso.com).</span><span class="sxs-lookup"><span data-stu-id="ec626-151">The user principal name (someuser@contoso.com).</span></span>|

<span data-ttu-id="ec626-152">Da die Ressource **Benutzer** [Extensions](/graph/extensibility-overview)unterstützt, können Sie die `POST` Vorgang und Hinzufügen von benutzerdefinierten Eigenschaften mit Ihren eigenen Daten auf die Benutzerinstanz beim Erstellen.</span><span class="sxs-lookup"><span data-stu-id="ec626-152">Since the **user** resource supports [extensions](/graph/extensibility-overview), you can use the `POST` operation and add custom properties with your own data to the user instance while creating it.</span></span>

## <a name="response"></a><span data-ttu-id="ec626-153">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec626-153">Response</span></span>

<span data-ttu-id="ec626-154">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec626-154">If successful, this method returns `201 Created` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec626-155">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ec626-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ec626-156">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ec626-156">Request</span></span>
<span data-ttu-id="ec626-157">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ec626-157">Here is an example of the request.</span></span>
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
  "userPrincipalName": "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    "forceChangePasswordNextSignIn": true,
    "password": "password-value"
  }
}
```
<span data-ttu-id="ec626-158">Geben Sie im Anforderungstext eine JSON-Darstellung des [user](../resources/user.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="ec626-158">In the request body, supply a JSON representation of [user](../resources/user.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ec626-159">Antwort</span><span class="sxs-lookup"><span data-stu-id="ec626-159">Response</span></span>
<span data-ttu-id="ec626-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ec626-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="ec626-163">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="ec626-163">See also</span></span>

- [<span data-ttu-id="ec626-164">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="ec626-164">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="ec626-165">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="ec626-165">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="ec626-166">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="ec626-166">Add custom data to groups using schema extensions (preview)</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create User",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-post-users.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
