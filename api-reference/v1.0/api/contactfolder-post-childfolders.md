---
title: contactFolder erstellen
description: 'Dient zum Erstellen eines neuen contactFolder als untergeordnetes Element eines bestimmten Ordners. '
ms.openlocfilehash: b6a4779b52a554e3a4050009e68b4124c17ca935
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016696"
---
# <a name="create-contactfolder"></a><span data-ttu-id="f492f-103">contactFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="f492f-103">Create ContactFolder</span></span>

<span data-ttu-id="f492f-104">Dient zum Erstellen eines neuen contactFolder als untergeordnetes Element eines bestimmten Ordners.</span><span class="sxs-lookup"><span data-stu-id="f492f-104">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="f492f-105">Sie können auch [eine neue Ressource des Typs „contactFolder“ im Standardkontaktordner des Benutzers erstellen](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="f492f-105">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="f492f-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f492f-106">Permissions</span></span>
<span data-ttu-id="f492f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f492f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f492f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="f492f-109">Permission type</span></span>      | <span data-ttu-id="f492f-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="f492f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f492f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="f492f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f492f-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f492f-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f492f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="f492f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f492f-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f492f-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="f492f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="f492f-115">Application</span></span> | <span data-ttu-id="f492f-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f492f-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="f492f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="f492f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="f492f-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="f492f-118">Request headers</span></span>
| <span data-ttu-id="f492f-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="f492f-119">Header</span></span>       | <span data-ttu-id="f492f-120">Wert</span><span class="sxs-lookup"><span data-stu-id="f492f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f492f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f492f-121">Authorization</span></span>  | <span data-ttu-id="f492f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f492f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f492f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f492f-124">Content-Type</span></span>  | <span data-ttu-id="f492f-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="f492f-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f492f-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="f492f-127">Request body</span></span>
<span data-ttu-id="f492f-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [ContactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f492f-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f492f-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="f492f-129">Response</span></span>

<span data-ttu-id="f492f-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [ContactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f492f-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f492f-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="f492f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f492f-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="f492f-132">Request</span></span>
<span data-ttu-id="f492f-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="f492f-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
<span data-ttu-id="f492f-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [contactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="f492f-134">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f492f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="f492f-135">Response</span></span>
<span data-ttu-id="f492f-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f492f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
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
