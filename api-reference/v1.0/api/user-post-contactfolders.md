---
title: ContactFolder erstellen
description: Erstellt einen neuen contactFolder unter dem Standardkontaktordner des Benutzers.
localization_priority: Normal
ms.openlocfilehash: fe17eb6c94c113a733ac2b9024ed28f910d43e71
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862755"
---
# <a name="create-contactfolder"></a><span data-ttu-id="6cb45-103">ContactFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="6cb45-103">Create ContactFolder</span></span>

<span data-ttu-id="6cb45-104">Erstellt einen neuen contactFolder unter dem Standardkontaktordner des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="6cb45-104">Create a new contactFolder under the user's default contacts folder.</span></span>

<span data-ttu-id="6cb45-105">Sie können auch [eine neue Ressource des Typs „contactfolder“ als untergeordnetes Element eines anderen Kontaktordners erstellen](contactfolder-post-childfolders.md).</span><span class="sxs-lookup"><span data-stu-id="6cb45-105">You can also [create a new contactfolder as a child of any specified contact folder](contactfolder-post-childfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="6cb45-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6cb45-106">Permissions</span></span>
<span data-ttu-id="6cb45-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6cb45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6cb45-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6cb45-109">Permission type</span></span>      | <span data-ttu-id="6cb45-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6cb45-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6cb45-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6cb45-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6cb45-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cb45-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6cb45-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6cb45-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6cb45-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cb45-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="6cb45-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6cb45-115">Application</span></span> | <span data-ttu-id="6cb45-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6cb45-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6cb45-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6cb45-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/contactFolders
```
## <a name="request-headers"></a><span data-ttu-id="6cb45-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6cb45-118">Request headers</span></span>
| <span data-ttu-id="6cb45-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="6cb45-119">Header</span></span>       | <span data-ttu-id="6cb45-120">Wert</span><span class="sxs-lookup"><span data-stu-id="6cb45-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6cb45-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6cb45-121">Authorization</span></span>  | <span data-ttu-id="6cb45-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6cb45-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6cb45-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6cb45-124">Content-Type</span></span>  | <span data-ttu-id="6cb45-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6cb45-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6cb45-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6cb45-126">Request body</span></span>
<span data-ttu-id="6cb45-127">Geben Sie im Anforderungstext eine JSON-Darstellung des [ContactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6cb45-127">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6cb45-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="6cb45-128">Response</span></span>

<span data-ttu-id="6cb45-129">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [ContactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6cb45-129">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6cb45-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6cb45-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6cb45-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6cb45-131">Request</span></span>
<span data-ttu-id="6cb45-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6cb45-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
<span data-ttu-id="6cb45-133">Geben Sie im Anforderungstext eine JSON-Darstellung des [contactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="6cb45-133">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="6cb45-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="6cb45-134">Response</span></span>
<span data-ttu-id="6cb45-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6cb45-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
