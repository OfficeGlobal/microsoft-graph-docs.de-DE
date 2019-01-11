---
title: Benutzer abrufen
description: Dient zum Abrufen der Eigenschaften und der Beziehungen des Benutzerobjekts.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: 8b21e45c5b6e86a539a2056859a0afa007614fcf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886212"
---
# <a name="get-a-user"></a><span data-ttu-id="a6e02-103">Benutzer abrufen</span><span class="sxs-lookup"><span data-stu-id="a6e02-103">Get a user</span></span>

<span data-ttu-id="a6e02-104">Dient zum Abrufen der Eigenschaften und der Beziehungen des Benutzerobjekts.</span><span class="sxs-lookup"><span data-stu-id="a6e02-104">Retrieve the properties and relationships of user object.</span></span>

> <span data-ttu-id="a6e02-p101">Hinweis: Durch das Auflisten eines Benutzers wird nur ein standardmäßiger Satz von Eigenschaften zurückgegeben (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Verwenden Sie `$select`, um die anderen Eigenschaften und Beziehungen für das [user](../resources/user.md)-Objekt abzurufen.</span><span class="sxs-lookup"><span data-stu-id="a6e02-p101">Note: Getting a user returns a default set of properties only (*businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName*). Use `$select` to get the other properties and relationships for the [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6e02-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a6e02-107">Permissions</span></span>
<span data-ttu-id="a6e02-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6e02-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6e02-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a6e02-110">Permission type</span></span>      | <span data-ttu-id="a6e02-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a6e02-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6e02-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a6e02-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a6e02-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a6e02-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a6e02-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a6e02-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6e02-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a6e02-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="a6e02-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a6e02-116">Application</span></span> | <span data-ttu-id="a6e02-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6e02-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6e02-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6e02-118">HTTP request</span></span>
<span data-ttu-id="a6e02-119">Für einen bestimmten Benutzer:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="a6e02-119">For a specific user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /users/{id | userPrincipalName}
```

<span data-ttu-id="a6e02-120">Für den angemeldeten Benutzer:<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="a6e02-120">For the signed-in user: <!-- { "blockType": "ignored" } --></span></span>
```http
GET /me
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6e02-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a6e02-121">Optional query parameters</span></span>
<span data-ttu-id="a6e02-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="a6e02-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="a6e02-123">Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="a6e02-123">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="a6e02-124">Um einen alternativen Eigenschaftensatz zurückzugeben, müssen Sie den gewünschten Satz von [user](../resources/user.md)-Eigenschaften mithilfe des Odata-Abfrageparameters `$select` angeben.</span><span class="sxs-lookup"><span data-stu-id="a6e02-124">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="a6e02-125">Um zum Beispiel _displayName_, _givenName_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="a6e02-125">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6e02-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a6e02-126">Request headers</span></span>
| <span data-ttu-id="a6e02-127">Header</span><span class="sxs-lookup"><span data-stu-id="a6e02-127">Header</span></span>       | <span data-ttu-id="a6e02-128">Wert</span><span class="sxs-lookup"><span data-stu-id="a6e02-128">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="a6e02-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6e02-129">Authorization</span></span>  | <span data-ttu-id="a6e02-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a6e02-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a6e02-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6e02-132">Content-Type</span></span>   | <span data-ttu-id="a6e02-133">application/json</span><span class="sxs-lookup"><span data-stu-id="a6e02-133">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6e02-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a6e02-134">Request body</span></span>
<span data-ttu-id="a6e02-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a6e02-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6e02-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6e02-136">Response</span></span>

<span data-ttu-id="a6e02-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [user](../resources/user.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a6e02-137">If successful, this method returns a `200 OK` response code and [user](../resources/user.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6e02-138">Beispiele</span><span class="sxs-lookup"><span data-stu-id="a6e02-138">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="a6e02-139">Beispiel 1: Standard-Benutzeranforderung</span><span class="sxs-lookup"><span data-stu-id="a6e02-139">Example 1: Standard users request</span></span>

<span data-ttu-id="a6e02-140">Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="a6e02-140">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> <span data-ttu-id="a6e02-141">Dieses Beispiel zeigt die standardmäßige Anforderung und Antwort.</span><span class="sxs-lookup"><span data-stu-id="a6e02-141">This example illustrates the default request and response.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}
```

##### <a name="response"></a><span data-ttu-id="a6e02-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6e02-142">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```


### <a name="example-2-signed-in-user-request"></a><span data-ttu-id="a6e02-143">Beispiel 2: Anforderung des angemeldeten Benutzers</span><span class="sxs-lookup"><span data-stu-id="a6e02-143">Example 2: Signed-in user request</span></span>

<span data-ttu-id="a6e02-144">Sie können die Benutzerinformationen des angemeldeten Benutzers abrufen, indem Sie `/users/{id | userPrincipalName}` durch `/me` ersetzen.</span><span class="sxs-lookup"><span data-stu-id="a6e02-144">You can get the user information for the signed-in user by replacing `/users/{id | userPrincipalName}` with `/me`.</span></span>

##### <a name="request"></a><span data-ttu-id="a6e02-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6e02-145">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_user"
}-->
```http
GET https://graph.microsoft.com/v1.0/me
```
##### <a name="response"></a><span data-ttu-id="a6e02-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6e02-146">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
  "businessPhones": [
       "businessPhones-value"
   ],
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "jobTitle": "jobTitle-value",
   "mail": "mail-value",
   "mobilePhone": "mobilePhone-value",
   "officeLocation": "officeLocation-value",
   "preferredLanguage": "preferredLanguage-value",
   "surname": "surname-value",
   "userPrincipalName": "userPrincipalName-value",
   "id": "id-value"
}
```

### <a name="example-3-users-request-using-select"></a><span data-ttu-id="a6e02-147">Beispiel 3: Benutzeranforderung mit $select</span><span class="sxs-lookup"><span data-stu-id="a6e02-147">Example 3: Users request using $select</span></span>

<span data-ttu-id="a6e02-148">Wenn Sie einen anderen Eigenschaftensatz benötigen, können Sie den OData-Abfrageparameter `$select` verwenden.</span><span class="sxs-lookup"><span data-stu-id="a6e02-148">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="a6e02-149">Um zum Beispiel _displayName_, _givenName_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="a6e02-149">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="a6e02-150">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a6e02-150">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}?$select=displayName,givenName,postalCode
```
##### <a name="response"></a><span data-ttu-id="a6e02-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="a6e02-151">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 491

{
   "displayName": "displayName-value",
   "givenName": "givenName-value",
   "postalCode": "postalCode-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
