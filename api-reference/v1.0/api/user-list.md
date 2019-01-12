---
title: Benutzer auflisten
description: Dient zum Abrufen einer Liste von Benutzerobjekten.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7529097f5d22443b95123cc7a2f578f0521b8ca4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926134"
---
# <a name="list-users"></a><span data-ttu-id="c11f8-103">Benutzer auflisten</span><span class="sxs-lookup"><span data-stu-id="c11f8-103">List users</span></span>

<span data-ttu-id="c11f8-104">Mit dieser API können Sie eine Liste von Benutzerobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="c11f8-104">Retrieve a list of user objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c11f8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c11f8-105">Permissions</span></span>

<span data-ttu-id="c11f8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c11f8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c11f8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c11f8-108">Permission type</span></span>      | <span data-ttu-id="c11f8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c11f8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c11f8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c11f8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c11f8-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c11f8-111">User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c11f8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c11f8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c11f8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c11f8-113">Not supported.</span></span>    |
|<span data-ttu-id="c11f8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c11f8-114">Application</span></span> | <span data-ttu-id="c11f8-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c11f8-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c11f8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c11f8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c11f8-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c11f8-117">Optional query parameters</span></span>

<span data-ttu-id="c11f8-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c11f8-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="c11f8-119">Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="c11f8-119">By default, only a limited set of properties are returned ( _businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_ ).</span></span> 

<span data-ttu-id="c11f8-120">Um einen alternativen Eigenschaftensatz zurückzugeben, müssen Sie den gewünschten Satz von [user](../resources/user.md)-Eigenschaften mithilfe des Odata-Abfrageparameters `$select` angeben.</span><span class="sxs-lookup"><span data-stu-id="c11f8-120">To return an alternative property set, you must specify the desired set of [user](../resources/user.md) properties using the OData `$select` query parameter.</span></span> <span data-ttu-id="c11f8-121">Um zum Beispiel _displayName_, _givenName_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="c11f8-121">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

> <span data-ttu-id="c11f8-p103">Hinweis: Bestimmte Eigenschaften können innerhalb einer Benutzersammlung nicht zurückgegeben werden. Die folgenden Eigenschaften werden nur unterstützt, wenn [ein einzelner Benutzer abgerufen wird](./user-get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span><span class="sxs-lookup"><span data-stu-id="c11f8-p103">Note: Certain properties cannot be returned within a user collection. The following properties are only supported when [retrieving an single user](./user-get.md): _aboutMe, birthday, hireDate, interests, mySite, pastProjects, preferredName, responsibilities, schools, skills, mailboxSettings_</span></span>

## <a name="request-headers"></a><span data-ttu-id="c11f8-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c11f8-124">Request headers</span></span>

| <span data-ttu-id="c11f8-125">Header</span><span class="sxs-lookup"><span data-stu-id="c11f8-125">Header</span></span>        | <span data-ttu-id="c11f8-126">Wert</span><span class="sxs-lookup"><span data-stu-id="c11f8-126">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="c11f8-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c11f8-127">Authorization</span></span> | <span data-ttu-id="c11f8-128">Bearer {token} (erforderlich)</span><span class="sxs-lookup"><span data-stu-id="c11f8-128">Bearer {token} (required)</span></span>  |
| <span data-ttu-id="c11f8-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c11f8-129">Content-Type</span></span>  | <span data-ttu-id="c11f8-130">application/json</span><span class="sxs-lookup"><span data-stu-id="c11f8-130">application/json</span></span>           |

## <a name="request-body"></a><span data-ttu-id="c11f8-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c11f8-131">Request body</span></span>

<span data-ttu-id="c11f8-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c11f8-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c11f8-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="c11f8-133">Response</span></span>

<span data-ttu-id="c11f8-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [user](../resources/user.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c11f8-134">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c11f8-135">Beispiele</span><span class="sxs-lookup"><span data-stu-id="c11f8-135">Examples</span></span>

### <a name="example-1-standard-users-request"></a><span data-ttu-id="c11f8-136">Beispiel 1: Standard-Benutzeranforderung</span><span class="sxs-lookup"><span data-stu-id="c11f8-136">Example 1: Standard users request</span></span>

<span data-ttu-id="c11f8-137">Standardmäßig wird nur ein begrenzter Satz von Eigenschaften zurückgegeben (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span><span class="sxs-lookup"><span data-stu-id="c11f8-137">By default, only a limited set of properties are returned (_businessPhones, displayName, givenName, id, jobTitle, mail, mobilePhone, officeLocation, preferredLanguage, surname, userPrincipalName_).</span></span> <span data-ttu-id="c11f8-138">Dieses Beispiel zeigt die standardmäßige Anforderung und Antwort.</span><span class="sxs-lookup"><span data-stu-id="c11f8-138">This example illustrates the default request and response.</span></span> 

##### <a name="request"></a><span data-ttu-id="c11f8-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c11f8-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users
```

##### <a name="response"></a><span data-ttu-id="c11f8-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="c11f8-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 608

{
  "value": [
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
  ]
}
```

### <a name="example-2-users-request-using-select"></a><span data-ttu-id="c11f8-141">Beispiel 2: Benutzeranforderung mit $select</span><span class="sxs-lookup"><span data-stu-id="c11f8-141">Example 2: Users request using $select</span></span>

<span data-ttu-id="c11f8-142">Wenn Sie einen anderen Eigenschaftensatz benötigen, können Sie den OData-Abfrageparameter `$select` verwenden.</span><span class="sxs-lookup"><span data-stu-id="c11f8-142">If you need a different property set, you can use the OData `$select` query parameter.</span></span> <span data-ttu-id="c11f8-143">Um zum Beispiel _displayName_, _givenName_ und _postalCode_ zurückzugeben, fügen Sie Folgendes zur Abfrage hinzu: `$select=displayName,givenName,postalCode`.</span><span class="sxs-lookup"><span data-stu-id="c11f8-143">For example, to return _displayName_, _givenName_, and _postalCode_, you would use the add the following to your query `$select=displayName,givenName,postalCode`</span></span>

##### <a name="request"></a><span data-ttu-id="c11f8-144">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c11f8-144">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_users"
}-->
```http
GET https://graph.microsoft.com/v1.0/users?$select=displayName,givenName,postalCode
```

##### <a name="response"></a><span data-ttu-id="c11f8-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="c11f8-145">Response</span></span>

<span data-ttu-id="c11f8-146">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="c11f8-146">Note: The response object shown here may be truncated for brevity.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 159

{
  "value": [
    {
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "postalCode": "postalCode-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List users",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
