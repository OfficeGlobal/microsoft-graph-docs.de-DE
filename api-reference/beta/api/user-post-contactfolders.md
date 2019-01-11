---
title: ContactFolder erstellen
description: Erstellt einen neuen contactFolder unter dem Standardkontaktordner des Benutzers.
localization_priority: Normal
ms.openlocfilehash: 4bd4fb26c78127fce9fff691cf187020428d9ab5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889707"
---
# <a name="create-contactfolder"></a><span data-ttu-id="bc459-103">contactFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="bc459-103">Create ContactFolder</span></span>

> <span data-ttu-id="bc459-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bc459-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc459-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc459-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc459-106">Erstellt einen neuen contactFolder unter dem Standardkontaktordner des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="bc459-106">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="bc459-107">Sie können auch [eine neue Ressource des Typs „contactfolder“ als untergeordnetes Element eines anderen Kontaktordners erstellen](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="bc459-107">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="bc459-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bc459-108">Permissions</span></span>
<span data-ttu-id="bc459-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc459-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc459-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc459-111">Permission type</span></span>      | <span data-ttu-id="bc459-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc459-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc459-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc459-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bc459-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc459-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bc459-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc459-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc459-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc459-116">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="bc459-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc459-117">Application</span></span> | <span data-ttu-id="bc459-118">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc459-118">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc459-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc459-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="bc459-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc459-120">Request headers</span></span>
| <span data-ttu-id="bc459-121">Header</span><span class="sxs-lookup"><span data-stu-id="bc459-121">Header</span></span>       | <span data-ttu-id="bc459-122">Wert</span><span class="sxs-lookup"><span data-stu-id="bc459-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bc459-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc459-123">Authorization</span></span>  | <span data-ttu-id="bc459-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc459-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bc459-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bc459-126">Content-Type</span></span>  | <span data-ttu-id="bc459-127">application/json</span><span class="sxs-lookup"><span data-stu-id="bc459-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc459-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc459-128">Request body</span></span>
<span data-ttu-id="bc459-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [ContactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bc459-129">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bc459-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc459-130">Response</span></span>

<span data-ttu-id="bc459-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [ContactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc459-131">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc459-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc459-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc459-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc459-133">Request</span></span>
<span data-ttu-id="bc459-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc459-134">Here is an example of the request.</span></span>
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
<span data-ttu-id="bc459-135">Geben Sie im Anforderungstext eine JSON-Darstellung des [contactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="bc459-135">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bc459-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc459-136">Response</span></span>
<span data-ttu-id="bc459-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc459-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
