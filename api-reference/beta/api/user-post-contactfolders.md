---
title: ContactFolder erstellen
description: Erstellt einen neuen contactFolder unter dem Standardkontaktordner des Benutzers.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0b9cf3dfb855b261b47e1a5614eda7602a50a363
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953563"
---
# <a name="create-contactfolder"></a><span data-ttu-id="a509c-103">contactFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="a509c-103">Create ContactFolder</span></span>

> <span data-ttu-id="a509c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a509c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a509c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a509c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a509c-106">Erstellt einen neuen contactFolder unter dem Standardkontaktordner des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="a509c-106">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="a509c-107">Sie können auch [eine neue Ressource des Typs „contactfolder“ als untergeordnetes Element eines anderen Kontaktordners erstellen](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="a509c-107">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a509c-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a509c-108">Permissions</span></span>
<span data-ttu-id="a509c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a509c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a509c-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a509c-111">Permission type</span></span>      | <span data-ttu-id="a509c-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a509c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a509c-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a509c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a509c-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a509c-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a509c-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a509c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a509c-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a509c-116">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a509c-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a509c-117">Application</span></span> | <span data-ttu-id="a509c-118">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a509c-118">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a509c-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a509c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="a509c-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a509c-120">Request headers</span></span>
| <span data-ttu-id="a509c-121">Header</span><span class="sxs-lookup"><span data-stu-id="a509c-121">Header</span></span>       | <span data-ttu-id="a509c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="a509c-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a509c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a509c-123">Authorization</span></span>  | <span data-ttu-id="a509c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a509c-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a509c-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a509c-126">Content-Type</span></span>  | <span data-ttu-id="a509c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a509c-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a509c-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a509c-128">Request body</span></span>
<span data-ttu-id="a509c-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [ContactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a509c-129">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a509c-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="a509c-130">Response</span></span>

<span data-ttu-id="a509c-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [ContactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a509c-131">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a509c-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a509c-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a509c-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a509c-133">Request</span></span>
<span data-ttu-id="a509c-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a509c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
<span data-ttu-id="a509c-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [contactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="a509c-135">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a509c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a509c-136">Response</span></span>
<span data-ttu-id="a509c-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a509c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
