---
title: Kontakt löschen
description: Mit dieser API können Sie Kontakte löschen.
ms.openlocfilehash: d81eb136702afd94537ea4651015ad6bbcab5450
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016355"
---
# <a name="delete-contact"></a><span data-ttu-id="04e61-103">Kontakt löschen</span><span class="sxs-lookup"><span data-stu-id="04e61-103">Delete contact</span></span>

<span data-ttu-id="04e61-104">Mit dieser API können Sie Kontakte löschen.</span><span class="sxs-lookup"><span data-stu-id="04e61-104">Delete a contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="04e61-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="04e61-105">Permissions</span></span>
<span data-ttu-id="04e61-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04e61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04e61-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="04e61-108">Permission type</span></span>      | <span data-ttu-id="04e61-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="04e61-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04e61-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="04e61-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04e61-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04e61-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="04e61-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="04e61-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04e61-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04e61-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="04e61-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="04e61-114">Application</span></span> | <span data-ttu-id="04e61-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="04e61-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="04e61-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="04e61-116">HTTP request</span></span>
<span data-ttu-id="04e61-117"><!-- { "blockType": "ignored" } -->[Wenden Sie sich](../resources/contact.md) von einem Benutzer standardmäßig [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="04e61-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from a user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="04e61-118">Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="04e61-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="04e61-p102">Ein [Kontakt](../resources/contact.md) in einem untergeordneten Ordner eines [contactFolder](../resources/mailfolder.md). Das Beispiel unten zeigt eine einzige Schachtelungsebene, aber ein Kontakt kann sich auch in einem untergeordneten Element eines untergeordneten Elements usw. befinden.</span><span class="sxs-lookup"><span data-stu-id="04e61-p102">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md). The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="04e61-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="04e61-121">Request headers</span></span>
| <span data-ttu-id="04e61-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="04e61-122">Header</span></span>       | <span data-ttu-id="04e61-123">Wert</span><span class="sxs-lookup"><span data-stu-id="04e61-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="04e61-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="04e61-124">Authorization</span></span>  | <span data-ttu-id="04e61-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="04e61-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="04e61-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="04e61-127">Request body</span></span>
<span data-ttu-id="04e61-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="04e61-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04e61-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="04e61-129">Response</span></span>

<span data-ttu-id="04e61-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04e61-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04e61-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="04e61-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04e61-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="04e61-133">Request</span></span>
<span data-ttu-id="04e61-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="04e61-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="04e61-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="04e61-135">Response</span></span>
<span data-ttu-id="04e61-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="04e61-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->