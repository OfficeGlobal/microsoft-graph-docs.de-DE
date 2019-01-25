---
title: Kontakt löschen
description: Kontakt löschen
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: be83bb8f655190d2da6aace13def579e371ef024
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514768"
---
# <a name="delete-contact"></a><span data-ttu-id="cc4c6-103">Kontakt löschen</span><span class="sxs-lookup"><span data-stu-id="cc4c6-103">Delete contact</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc4c6-104">Kontakt löschen</span><span class="sxs-lookup"><span data-stu-id="cc4c6-104">Delete contact.</span></span>
## <a name="permissions"></a><span data-ttu-id="cc4c6-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="cc4c6-105">Permissions</span></span>
<span data-ttu-id="cc4c6-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc4c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc4c6-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="cc4c6-108">Permission type</span></span>      | <span data-ttu-id="cc4c6-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="cc4c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc4c6-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="cc4c6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cc4c6-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc4c6-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cc4c6-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="cc4c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc4c6-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc4c6-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="cc4c6-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="cc4c6-114">Application</span></span> | <span data-ttu-id="cc4c6-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cc4c6-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc4c6-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="cc4c6-116">HTTP request</span></span>
<span data-ttu-id="cc4c6-117"><!-- { "blockType": "ignored" } -->[Wenden Sie sich an](../resources/contact.md) von des Benutzers Standard [ContactFolder](../resources/contactfolder.md).</span><span class="sxs-lookup"><span data-stu-id="cc4c6-117"><!-- { "blockType": "ignored" } --> A [contact](../resources/contact.md) from user's default [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contacts/{id}
DELETE /users/{id | userPrincipalName}/contacts/{id}
```
<span data-ttu-id="cc4c6-118">Ein [Kontakt](../resources/contact.md) aus dem [contactFolder](../resources/contactfolder.md) oberster Ebene eines Benutzers.</span><span class="sxs-lookup"><span data-stu-id="cc4c6-118">A [contact](../resources/contact.md) from a user's top level [contactFolder](../resources/contactfolder.md).</span></span>
```http
DELETE /me/contactFolders/{id}/contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
<span data-ttu-id="cc4c6-119">[Wenden Sie sich an](../resources/contact.md) , die in einem untergeordneten Ordner von einem [ContactFolder](../resources/mailfolder.md)enthalten sind.</span><span class="sxs-lookup"><span data-stu-id="cc4c6-119">A [contact](../resources/contact.md) contained in a child folder of a [contactFolder](../resources/mailfolder.md).</span></span>  <span data-ttu-id="cc4c6-120">Das folgende Beispiel zeigt eine Ebene von schachteln, aber ein Kontakt kann befindet sich ein untergeordnetes Element des ein untergeordnetes Element und so weiter.</span><span class="sxs-lookup"><span data-stu-id="cc4c6-120">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>
```http
DELETE /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a><span data-ttu-id="cc4c6-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="cc4c6-121">Request headers</span></span>
| <span data-ttu-id="cc4c6-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="cc4c6-122">Header</span></span>       | <span data-ttu-id="cc4c6-123">Wert</span><span class="sxs-lookup"><span data-stu-id="cc4c6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cc4c6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc4c6-124">Authorization</span></span>  | <span data-ttu-id="cc4c6-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="cc4c6-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="cc4c6-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="cc4c6-127">Request body</span></span>
<span data-ttu-id="cc4c6-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="cc4c6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc4c6-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="cc4c6-129">Response</span></span>

<span data-ttu-id="cc4c6-p104">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cc4c6-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc4c6-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="cc4c6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cc4c6-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="cc4c6-133">Request</span></span>
<span data-ttu-id="cc4c6-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="cc4c6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contact"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/contacts/{id}
```
##### <a name="response"></a><span data-ttu-id="cc4c6-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="cc4c6-135">Response</span></span>
<span data-ttu-id="cc4c6-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="cc4c6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contact-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
