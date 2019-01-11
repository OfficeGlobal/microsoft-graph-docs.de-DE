---
title: Kontakt erstellen
description: Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Endpunkt `contacts` eines anderen Kontaktordners.
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: b23d74e6b1a92cb92d9c5d207d9a8a50235a75e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892288"
---
# <a name="create-contact"></a><span data-ttu-id="7a5ac-103">Kontakt erstellen</span><span class="sxs-lookup"><span data-stu-id="7a5ac-103">Create Contact</span></span>

> <span data-ttu-id="7a5ac-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7a5ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a5ac-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7a5ac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7a5ac-106">Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Endpunkt `contacts` eines anderen Kontaktordners.</span><span class="sxs-lookup"><span data-stu-id="7a5ac-106">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a5ac-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7a5ac-107">Permissions</span></span>
<span data-ttu-id="7a5ac-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a5ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a5ac-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7a5ac-110">Permission type</span></span>      | <span data-ttu-id="7a5ac-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7a5ac-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a5ac-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7a5ac-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7a5ac-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a5ac-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7a5ac-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7a5ac-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a5ac-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a5ac-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="7a5ac-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7a5ac-116">Application</span></span> | <span data-ttu-id="7a5ac-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7a5ac-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a5ac-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a5ac-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```
## <a name="request-headers"></a><span data-ttu-id="7a5ac-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a5ac-119">Request headers</span></span>
## <a name="request-headers"></a><span data-ttu-id="7a5ac-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7a5ac-120">Request headers</span></span>
| <span data-ttu-id="7a5ac-121">Header</span><span class="sxs-lookup"><span data-stu-id="7a5ac-121">Header</span></span>       | <span data-ttu-id="7a5ac-122">Wert</span><span class="sxs-lookup"><span data-stu-id="7a5ac-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7a5ac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a5ac-123">Authorization</span></span>  | <span data-ttu-id="7a5ac-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7a5ac-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7a5ac-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7a5ac-126">Content-Type</span></span>  | <span data-ttu-id="7a5ac-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="7a5ac-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7a5ac-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7a5ac-129">Request body</span></span>
<span data-ttu-id="7a5ac-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [Contact](../resources/contact.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7a5ac-130">In the request body, supply a JSON representation of [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7a5ac-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a5ac-131">Response</span></span>

<span data-ttu-id="7a5ac-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a5ac-132">If successful, this method returns `201 Created` response code and [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a5ac-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7a5ac-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a5ac-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7a5ac-134">Request</span></span>
<span data-ttu-id="7a5ac-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7a5ac-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="7a5ac-136">Geben Sie im Anforderungstext eine JSON-Darstellung des [contact](../resources/contact.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="7a5ac-136">In the request body, supply a JSON representation of [contact](../resources/contact.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="7a5ac-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="7a5ac-137">Response</span></span>
<span data-ttu-id="7a5ac-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7a5ac-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
