---
title: contactFolder erstellen
description: 'Dient zum Erstellen eines neuen contactFolder als untergeordnetes Element eines bestimmten Ordners. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 606e6b9dfc906e8b6975c64fa36beede5a7c56b3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513473"
---
# <a name="create-contactfolder"></a><span data-ttu-id="3db16-103">contactFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="3db16-103">Create ContactFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3db16-104">Dient zum Erstellen eines neuen contactFolder als untergeordnetes Element eines bestimmten Ordners.</span><span class="sxs-lookup"><span data-stu-id="3db16-104">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="3db16-105">Sie können auch [eine neue Ressource des Typs „contactFolder“ im Standardkontaktordner des Benutzers erstellen](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="3db16-105">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3db16-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3db16-106">Permissions</span></span>
<span data-ttu-id="3db16-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3db16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3db16-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3db16-109">Permission type</span></span>      | <span data-ttu-id="3db16-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3db16-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3db16-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3db16-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3db16-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3db16-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3db16-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3db16-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3db16-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3db16-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="3db16-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3db16-115">Application</span></span> | <span data-ttu-id="3db16-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3db16-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="3db16-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3db16-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="3db16-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3db16-118">Request headers</span></span>
| <span data-ttu-id="3db16-119">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="3db16-119">Header</span></span>       | <span data-ttu-id="3db16-120">Wert</span><span class="sxs-lookup"><span data-stu-id="3db16-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3db16-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3db16-121">Authorization</span></span>  | <span data-ttu-id="3db16-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3db16-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3db16-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3db16-124">Content-Type</span></span>  | <span data-ttu-id="3db16-p103">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="3db16-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3db16-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3db16-127">Request body</span></span>
<span data-ttu-id="3db16-128">Geben Sie im Anforderungstext eine JSON-Darstellung des [ContactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3db16-128">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3db16-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="3db16-129">Response</span></span>

<span data-ttu-id="3db16-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [ContactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3db16-130">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3db16-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3db16-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3db16-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3db16-132">Request</span></span>
<span data-ttu-id="3db16-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3db16-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_contactfolder_from_contactfolder"
}-->
```http
POST https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
Content-type: application/json
Content-length: 84

{
  "displayName": "displayName-value"
}
```
<span data-ttu-id="3db16-134">Geben Sie im Anforderungstext eine JSON-Darstellung des [contactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="3db16-134">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3db16-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3db16-135">Response</span></span>
<span data-ttu-id="3db16-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3db16-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create ContactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-post-childfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
