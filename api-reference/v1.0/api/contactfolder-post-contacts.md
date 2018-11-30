---
title: Kontakt erstellen
description: Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Endpunkt `contacts` eines anderen Kontaktordners.
ms.openlocfilehash: d17072285b52a70a8d30533c073678d9bf2ec95d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016879"
---
# <a name="create-contact"></a><span data-ttu-id="66507-103">Kontakt erstellen</span><span class="sxs-lookup"><span data-stu-id="66507-103">Create contact</span></span>

<span data-ttu-id="66507-104">Dient zum Hinzufügen eines Kontakts zum Stammordner der Kontakte oder zum Endpunkt `contacts` eines anderen Kontaktordners.</span><span class="sxs-lookup"><span data-stu-id="66507-104">Add a contact to the root Contacts folder or to the `contacts` endpoint of another contact folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="66507-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="66507-105">Permissions</span></span>

<span data-ttu-id="66507-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="66507-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66507-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="66507-108">Permission type</span></span>      | <span data-ttu-id="66507-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="66507-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66507-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="66507-110">Delegated (work or school account)</span></span> | <span data-ttu-id="66507-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66507-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="66507-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="66507-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66507-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66507-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="66507-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="66507-114">Application</span></span> | <span data-ttu-id="66507-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="66507-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="66507-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="66507-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/contacts
POST /users/{id | userPrincipalName}/contacts

POST /me/contactFolders/{id}/contacts
POST /users/{id | userPrincipalName}/contactFolders/{id}/contacts
```

<br/>

## <a name="request-headers"></a><span data-ttu-id="66507-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="66507-117">Request headers</span></span>

| <span data-ttu-id="66507-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="66507-118">Header</span></span>       | <span data-ttu-id="66507-119">Wert</span><span class="sxs-lookup"><span data-stu-id="66507-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="66507-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="66507-120">Authorization</span></span>  | <span data-ttu-id="66507-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="66507-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="66507-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66507-123">Content-Type</span></span>  | <span data-ttu-id="66507-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="66507-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="66507-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="66507-126">Request body</span></span>
<span data-ttu-id="66507-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [Contact](../resources/contact.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="66507-127">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="66507-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="66507-128">Response</span></span>

<span data-ttu-id="66507-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [Contact](../resources/contact.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="66507-129">If successful, this method returns `201 Created` response code and the [Contact](../resources/contact.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66507-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="66507-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="66507-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="66507-131">Request</span></span>

<span data-ttu-id="66507-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="66507-132">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_contact_from_contactfolder"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/contacts
Content-type: application/json
Content-length: 210

{
  "parentFolderId": "parentFolderId-value",
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<span data-ttu-id="66507-133">Geben Sie im Anforderungstext eine JSON-Darstellung des [Contact](../resources/contact.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="66507-133">In the request body, supply a JSON representation of the [Contact](../resources/contact.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="66507-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="66507-134">Response</span></span>

<span data-ttu-id="66507-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="66507-135">Here is an example of the response.</span></span> <span data-ttu-id="66507-136">**Hinweis:** Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="66507-136">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="66507-137">Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="66507-137">All the properties will be returned from an actual call.</span></span>

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
  "birthday": "datetime-value",
  "fileAs": "fileAs-value",
  "displayName": "displayName-value",
  "givenName": "givenName-value",
  "initials": "initials-value"
}
```

<br/>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
