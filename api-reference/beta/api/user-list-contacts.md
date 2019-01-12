---
title: Kontakte auflisten
description: Rufen Sie Kontakte in das Postfach des Benutzers.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2b427be9872aff70ecf5ed3166e94a48b94a62ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953630"
---
# <a name="list-contacts"></a><span data-ttu-id="bfe1c-103">Kontakte auflisten</span><span class="sxs-lookup"><span data-stu-id="bfe1c-103">List contacts</span></span>

> <span data-ttu-id="bfe1c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bfe1c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfe1c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bfe1c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfe1c-106">Rufen Sie Kontakte in das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="bfe1c-106">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="bfe1c-107">Es gibt zwei Szenarien, in dem eine app Kontakte in einen anderen Benutzer Kontaktordner abrufen:</span><span class="sxs-lookup"><span data-stu-id="bfe1c-107">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="bfe1c-108">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="bfe1c-108">If the app has application permissions, or,</span></span>
* <span data-ttu-id="bfe1c-109">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer diesen Benutzer einen Kontaktordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="bfe1c-109">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="bfe1c-110">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="bfe1c-110">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="bfe1c-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bfe1c-111">Permissions</span></span>
<span data-ttu-id="bfe1c-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bfe1c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfe1c-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bfe1c-114">Permission type</span></span>      | <span data-ttu-id="bfe1c-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bfe1c-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfe1c-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bfe1c-116">Delegated (work or school account)</span></span> | <span data-ttu-id="bfe1c-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfe1c-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bfe1c-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bfe1c-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfe1c-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfe1c-119">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bfe1c-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bfe1c-120">Application</span></span> | <span data-ttu-id="bfe1c-121">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfe1c-121">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bfe1c-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfe1c-122">HTTP request</span></span>

<span data-ttu-id="bfe1c-123">So rufen Sie alle Kontakte in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="bfe1c-123">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="bfe1c-124">So rufen Sie Kontakte in einem spezifischen Ordner in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="bfe1c-124">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bfe1c-125">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bfe1c-125">Optional query parameters</span></span>
<span data-ttu-id="bfe1c-126">Sie können die `$filter` Abfragezeichenfolgen-Parameter Filter Kontakten basierend auf ihren e-Mail-Adressen:</span><span class="sxs-lookup"><span data-stu-id="bfe1c-126">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="bfe1c-127">Notiz, die Sie verwenden können `$filter`, `any`, und die `eq` Operator auf nur die **Adresse** Sub-Eigenschaft des Instanzen in einer **EmailAddresses** -Auflistung.</span><span class="sxs-lookup"><span data-stu-id="bfe1c-127">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="bfe1c-128">D. h., Sie können nicht auf den **Namen** oder andere untergeordnete Eigenschaft einer Instanz des **EmailAddresses**filtern, noch können Sie ein beliebiger anderer Operator anwenden oder Funktion mit `filter`, wie `ne`, `le`, und `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="bfe1c-128">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="bfe1c-129">Allgemeine Informationen zu den `$filter` Parameter Abfragen, finden Sie unter [OData-Abfrageparametern](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bfe1c-129">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfe1c-130">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bfe1c-130">Request headers</span></span>
| <span data-ttu-id="bfe1c-131">Header</span><span class="sxs-lookup"><span data-stu-id="bfe1c-131">Header</span></span>       | <span data-ttu-id="bfe1c-132">Wert</span><span class="sxs-lookup"><span data-stu-id="bfe1c-132">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bfe1c-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfe1c-133">Authorization</span></span>  | <span data-ttu-id="bfe1c-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bfe1c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bfe1c-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bfe1c-136">Request body</span></span>
<span data-ttu-id="bfe1c-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bfe1c-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bfe1c-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfe1c-138">Response</span></span>

<span data-ttu-id="bfe1c-139">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [wenden Sie sich an](../resources/contact.md) .</span><span class="sxs-lookup"><span data-stu-id="bfe1c-139">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bfe1c-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bfe1c-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfe1c-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bfe1c-141">Request</span></span>
<span data-ttu-id="bfe1c-142">Das folgende Beispiel ruft die Eigenschaften des angemeldeten Benutzers Kontakte **DisplayName** und **EmailAddresses** ab.</span><span class="sxs-lookup"><span data-stu-id="bfe1c-142">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="bfe1c-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="bfe1c-143">Response</span></span>
<span data-ttu-id="bfe1c-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bfe1c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts(displayName,emailAddresses)",
    "value":[
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7f6\"",
            "id":"AAMkADh6v5AAAvgTCFAAA=",
            "displayName":"Elvis Blank",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Elvis Blank",
                    "address":"elvisb@relecloud.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Elvis Blank",
                    "address":"elvisb@fabrikam.onmicrosoft.com"
                }
            ]
        },
        {
            "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fn\"",
            "id":"AAMkADh6v5AAAvgTCEAAA=",
            "displayName":"Pavel Bansky",
            "emailAddresses":[
                {
                    "type":"personal",
                    "name":"Pavel Bansky",
                    "address":"pavelb@contoso.onmicrosoft.com"
                },
                {
                    "type":"other",
                    "otherLabel":"Volunteer work",
                    "name":"Pavel Bansky",
                    "address":"pavelb@fabrikam.onmicrosoft.com"
                }
            ]
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
