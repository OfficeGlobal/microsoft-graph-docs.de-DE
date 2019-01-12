---
title: Kontakt löschen
description: Löschen Sie Kontakt.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1cacb801ad872d14898e1799987acb248cfdb446
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990418"
---
# <a name="delete-contact"></a><span data-ttu-id="06956-103">Kontakt löschen</span><span class="sxs-lookup"><span data-stu-id="06956-103">Delete contact</span></span>

> <span data-ttu-id="06956-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="06956-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06956-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="06956-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06956-106">Löschen Sie Kontakt.</span><span class="sxs-lookup"><span data-stu-id="06956-106">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="06956-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="06956-107">Permissions</span></span>
<span data-ttu-id="06956-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06956-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06956-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="06956-110">Permission type</span></span>      | <span data-ttu-id="06956-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="06956-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06956-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="06956-112">Delegated (work or school account)</span></span> | <span data-ttu-id="06956-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06956-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="06956-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="06956-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06956-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06956-115">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="06956-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="06956-116">Application</span></span> | <span data-ttu-id="06956-117">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="06956-117">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="06956-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="06956-118">HTTP request</span></span>
<span data-ttu-id="06956-119"><!-- { "blockType": "ignored" } -->[Wenden Sie sich an](../resources/contact.md) von des Benutzers Standard [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="06956-119"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="06956-120">Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="06956-120">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="06956-121">[Wenden Sie sich an](../resources/contact.md) , die in einem untergeordneten Ordner von einem [ContactFolder](../resources/mailfolder.md)enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="06956-121">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="06956-122">Das folgende Beispiel zeigt eine Ebene von schachteln, aber ein Kontakt kann befindet sich ein untergeordnetes Element des ein untergeordnetes Element und so weiter.</span><span class="sxs-lookup"><span data-stu-id="06956-122">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="06956-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="06956-123">Request headers</span></span>
| <span data-ttu-id="06956-124">Header</span><span class="sxs-lookup"><span data-stu-id="06956-124">Header</span></span>       | <span data-ttu-id="06956-125">Wert</span><span class="sxs-lookup"><span data-stu-id="06956-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="06956-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="06956-126">Authorization</span></span>  | <span data-ttu-id="06956-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="06956-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="06956-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="06956-129">Request body</span></span>
<span data-ttu-id="06956-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="06956-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06956-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="06956-131">Response</span></span>

<span data-ttu-id="06956-p105">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06956-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06956-134">Beispiel</span><span class="sxs-lookup"><span data-stu-id="06956-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06956-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="06956-135">Request</span></span>
<span data-ttu-id="06956-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="06956-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="06956-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="06956-137">Response</span></span>
<span data-ttu-id="06956-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="06956-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
