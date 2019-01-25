---
title: Kontakte auflisten
description: Rufen Sie Kontakte in das Postfach des Benutzers.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c444a818b933196ddc46ae0d12d64355656bd7f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510911"
---
# <a name="list-contacts"></a><span data-ttu-id="bb2b4-103">Kontakte auflisten</span><span class="sxs-lookup"><span data-stu-id="bb2b4-103">List contacts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb2b4-104">Rufen Sie Kontakte in das Postfach des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="bb2b4-104">Get contacts in the user's mailbox.</span></span>

<span data-ttu-id="bb2b4-105">Es gibt zwei Szenarien, in dem eine app Kontakte in einen anderen Benutzer Kontaktordner abrufen:</span><span class="sxs-lookup"><span data-stu-id="bb2b4-105">There are two scenarios where an app can get contacts in another user's contact folder:</span></span>

* <span data-ttu-id="bb2b4-106">Wenn die app Anwendungsberechtigungen verfügt oder,</span><span class="sxs-lookup"><span data-stu-id="bb2b4-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="bb2b4-107">Wenn die app verfügt die entsprechenden [Berechtigungen](#permissions) delegiert, von einem Benutzer und einen anderen Benutzer diesen Benutzer einen Kontaktordner freigegeben hat, oder delegierten Zugriff, die diesem Benutzer zugewiesen hat.</span><span class="sxs-lookup"><span data-stu-id="bb2b4-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a contact folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="bb2b4-108">Finden Sie [ausführliche Informationen und ein Beispiel](/graph/outlook-get-shared-contacts-folders).</span><span class="sxs-lookup"><span data-stu-id="bb2b4-108">See [details and an example](/graph/outlook-get-shared-contacts-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="bb2b4-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bb2b4-109">Permissions</span></span>
<span data-ttu-id="bb2b4-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bb2b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb2b4-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bb2b4-112">Permission type</span></span>      | <span data-ttu-id="bb2b4-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bb2b4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bb2b4-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bb2b4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bb2b4-115">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb2b4-115">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bb2b4-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bb2b4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bb2b4-117">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb2b4-117">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bb2b4-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bb2b4-118">Application</span></span> | <span data-ttu-id="bb2b4-119">Contacts.Read, Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bb2b4-119">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bb2b4-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb2b4-120">HTTP request</span></span>

<span data-ttu-id="bb2b4-121">So rufen Sie alle Kontakte in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="bb2b4-121">To get all the contacts in a user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

<span data-ttu-id="bb2b4-122">So rufen Sie Kontakte in einem spezifischen Ordner in einem Benutzerpostfach ab:</span><span class="sxs-lookup"><span data-stu-id="bb2b4-122">To get contacts in a specific folder in the user's mailbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bb2b4-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bb2b4-123">Optional query parameters</span></span>
<span data-ttu-id="bb2b4-124">Sie können die `$filter` Abfragezeichenfolgen-Parameter Filter Kontakten basierend auf ihren e-Mail-Adressen:</span><span class="sxs-lookup"><span data-stu-id="bb2b4-124">You can use the `$filter` query parameter to filter contacts based on their email addresses:</span></span>

<!-- { "blockType": "ignored" } -->
``` http
GET https://graph.microsoft.com/beta/me/contacts?$filter=emailAddresses/any(a:a/address eq 'garth@contoso.com')
```

<span data-ttu-id="bb2b4-125">Notiz, die Sie verwenden können `$filter`, `any`, und die `eq` Operator auf nur die **Adresse** Sub-Eigenschaft des Instanzen in einer **EmailAddresses** -Auflistung.</span><span class="sxs-lookup"><span data-stu-id="bb2b4-125">Note that you can use `$filter`, `any`, and the `eq` operator on only the **address** sub-property of instances in an **emailAddresses** collection.</span></span> <span data-ttu-id="bb2b4-126">D. h., Sie können nicht auf den **Namen** oder andere untergeordnete Eigenschaft einer Instanz des **EmailAddresses**filtern, noch können Sie ein beliebiger anderer Operator anwenden oder Funktion mit `filter`, wie `ne`, `le`, und `startswith()`.</span><span class="sxs-lookup"><span data-stu-id="bb2b4-126">That is, you cannot filter on the **name** or any other sub-property of an instance of **emailAddresses**, nor can you apply any other operator or function with `filter`, such as `ne`, `le`, and `startswith()`.</span></span>

<span data-ttu-id="bb2b4-127">Allgemeine Informationen zu den `$filter` Parameter Abfragen, finden Sie unter [OData-Abfrageparametern](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bb2b4-127">For general information on the `$filter` query parameter, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bb2b4-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bb2b4-128">Request headers</span></span>
| <span data-ttu-id="bb2b4-129">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="bb2b4-129">Header</span></span>       | <span data-ttu-id="bb2b4-130">Wert</span><span class="sxs-lookup"><span data-stu-id="bb2b4-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bb2b4-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb2b4-131">Authorization</span></span>  | <span data-ttu-id="bb2b4-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bb2b4-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bb2b4-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bb2b4-134">Request body</span></span>
<span data-ttu-id="bb2b4-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bb2b4-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb2b4-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb2b4-136">Response</span></span>

<span data-ttu-id="bb2b4-137">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und Auflistung von Objekten im Antworttext [wenden Sie sich an](../resources/contact.md) .</span><span class="sxs-lookup"><span data-stu-id="bb2b4-137">If successful, this method returns a `200 OK` response code and collection of [contact](../resources/contact.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bb2b4-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bb2b4-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bb2b4-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bb2b4-139">Request</span></span>
<span data-ttu-id="bb2b4-140">Das folgende Beispiel ruft die Eigenschaften des angemeldeten Benutzers Kontakte **DisplayName** und **EmailAddresses** ab.</span><span class="sxs-lookup"><span data-stu-id="bb2b4-140">The following example gets the **displayName** and **emailAddresses** properties of the signed-in user's contacts.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/beta/me/contacts?$select=displayName,emailAddresses
```


##### <a name="response"></a><span data-ttu-id="bb2b4-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="bb2b4-141">Response</span></span>
<span data-ttu-id="bb2b4-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bb2b4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
