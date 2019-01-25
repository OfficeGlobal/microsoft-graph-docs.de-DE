---
title: Kontakt erstellen
description: Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Endpunkt `contacts` eines anderen Kontaktordners.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 3fd45ee7f77e2d485b7a972b8454807368796226
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528060"
---
# <a name="create-contact"></a><span data-ttu-id="e667a-103">Kontakt erstellen</span><span class="sxs-lookup"><span data-stu-id="e667a-103">Create Contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e667a-104">Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Endpunkt `contacts` eines anderen Kontaktordners.</span><span class="sxs-lookup"><span data-stu-id="e667a-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="e667a-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e667a-105">Permissions</span></span>
<span data-ttu-id="e667a-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e667a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e667a-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e667a-108">Permission type</span></span>      | <span data-ttu-id="e667a-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e667a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e667a-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e667a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e667a-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e667a-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e667a-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e667a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e667a-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e667a-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e667a-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e667a-114">Application</span></span> | <span data-ttu-id="e667a-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e667a-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e667a-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e667a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="e667a-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e667a-117">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="e667a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e667a-118">Request headers</span></span>
| <span data-ttu-id="e667a-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e667a-119">Header</span></span>       | <span data-ttu-id="e667a-120">Wert</span><span class="sxs-lookup"><span data-stu-id="e667a-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e667a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e667a-121">Authorization</span></span>  | <span data-ttu-id="e667a-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e667a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e667a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e667a-124">Content-Type</span></span>  | <span data-ttu-id="e667a-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="e667a-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e667a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e667a-127">Request body</span></span>
<span data-ttu-id="e667a-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [Contact](../resources/contact.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e667a-128">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e667a-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e667a-129">Response</span></span>

<span data-ttu-id="e667a-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e667a-130">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e667a-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e667a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e667a-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e667a-132">Request</span></span>
<span data-ttu-id="e667a-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e667a-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```
<span data-ttu-id="e667a-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [contact](../resources/contact.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="e667a-134">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e667a-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="e667a-135">Response</span></span>
<span data-ttu-id="e667a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e667a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "2016-10-19T10:37:00Z",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-post-contacts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
