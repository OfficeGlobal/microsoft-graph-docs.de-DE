---
title: Kontakte auflisten
description: Rufen Sie eine Kontakte-Auflistung aus dem Standardordner Kontakte des angemeldeten Benutzers.
ms.openlocfilehash: 9322810d90f38c0b7643379f22a90a89cf7070df
ms.sourcegitcommit: 12c6e82f1417022540e534ebadbd0e8d7fb5abde
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/08/2018
ms.locfileid: "27209733"
---
# <a name="list-contacts"></a><span data-ttu-id="f30e5-103">Kontakte auflisten</span><span class="sxs-lookup"><span data-stu-id="f30e5-103">List contacts</span></span>

<span data-ttu-id="f30e5-104">Rufen Sie eine Kontakte-Auflistung aus dem Standardordner Kontakte des angemeldeten Benutzers.</span><span class="sxs-lookup"><span data-stu-id="f30e5-104">Get a contact collection from the default contacts folder of the signed-in user.</span></span>

<span data-ttu-id="f30e5-105">Es gibt zwei Szenarien, in dem eine app Kontakte in einen anderen Benutzer Kontaktordner abrufen:</span><span class="sxs-lookup"><span data-stu-id="f30e5-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="f30e5-106">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="f30e5-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="f30e5-107">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer diesen Benutzer einen Kontaktordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="f30e5-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="f30e5-108">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="f30e5-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="f30e5-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f30e5-109">Permissions</span></span>
<span data-ttu-id="f30e5-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f30e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f30e5-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f30e5-112">Permission type</span></span>      | <span data-ttu-id="f30e5-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f30e5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f30e5-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f30e5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f30e5-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f30e5-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f30e5-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f30e5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f30e5-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f30e5-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f30e5-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f30e5-118">Application</span></span> | <span data-ttu-id="f30e5-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f30e5-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f30e5-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f30e5-120">HTTP request</span></span>

<span data-ttu-id="f30e5-121">So rufen Sie alle Kontakte in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="f30e5-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="f30e5-122">So rufen Sie Kontakte in einem spezifischen Ordner in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="f30e5-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f30e5-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="f30e5-123">Optional query parameters</span></span>
<span data-ttu-id="f30e5-124">Sie können die `$filter` Abfragezeichenfolgen-Parameter Filter Kontakten basierend auf ihren e-Mail-Adressen:</span><span class="sxs-lookup"><span data-stu-id="f30e5-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="f30e5-125">Notiz, die Sie verwenden können `$filter`, `any`, und die `eq` Operator auf nur die **Adresse** Sub-Eigenschaft des Instanzen in einer **EmailAddresses** -Auflistung.</span><span class="sxs-lookup"><span data-stu-id="f30e5-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="f30e5-126">D. h., Sie können nicht auf den **Namen** oder andere untergeordnete Eigenschaft einer Instanz des **EmailAddresses**filtern, noch können Sie ein beliebiger anderer Operator anwenden oder Funktion mit `filter`, wie `ne`, `le`, und `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="f30e5-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="f30e5-127">Allgemeine Informationen zu den `$filter` Parameter Abfragen, finden Sie unter [OData-Abfrageparametern](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f30e5-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>



## <a name="request-headers"></a><span data-ttu-id="f30e5-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f30e5-128">Request headers</span></span>
| <span data-ttu-id="f30e5-129">Header</span><span class="sxs-lookup"><span data-stu-id="f30e5-129">Header</span></span>       | <span data-ttu-id="f30e5-130">Wert</span><span class="sxs-lookup"><span data-stu-id="f30e5-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f30e5-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="f30e5-131">Authorization</span></span>  | <span data-ttu-id="f30e5-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f30e5-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f30e5-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f30e5-134">Content-Type</span></span>   | <span data-ttu-id="f30e5-135">application/json</span><span class="sxs-lookup"><span data-stu-id="f30e5-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f30e5-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f30e5-136">Request body</span></span>
<span data-ttu-id="f30e5-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="f30e5-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f30e5-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="f30e5-138">Response</span></span>

<span data-ttu-id="f30e5-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [Contact](../resources/contact.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f30e5-139">If successful, this method returns a `200 OK` response code and collection of [Contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f30e5-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f30e5-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f30e5-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f30e5-141">Request</span></span>
<span data-ttu-id="f30e5-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f30e5-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a><span data-ttu-id="f30e5-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="f30e5-143">Response</span></span>
<span data-ttu-id="f30e5-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f30e5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
