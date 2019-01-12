---
title: contactFolder erstellen
description: 'Dient zum Erstellen eines neuen contactFolder als untergeordnetes Element eines bestimmten Ordners. '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 66061d86b3c3894c165788cd408b22b8824b34f9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991769"
---
# <a name="create-contactfolder"></a><span data-ttu-id="c0c3f-103">contactFolder erstellen</span><span class="sxs-lookup"><span data-stu-id="c0c3f-103">Create ContactFolder</span></span>

> <span data-ttu-id="c0c3f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c0c3f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0c3f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c0c3f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0c3f-106">Dient zum Erstellen eines neuen contactFolder als untergeordnetes Element eines bestimmten Ordners.</span><span class="sxs-lookup"><span data-stu-id="c0c3f-106">Create a new contactFolder as a child of a specified folder.</span></span> 

<span data-ttu-id="c0c3f-107">Sie können auch [eine neue Ressource des Typs „contactFolder“ im Standardkontaktordner des Benutzers erstellen](user-post-contactfolders.md).</span><span class="sxs-lookup"><span data-stu-id="c0c3f-107">You can also [create a new contactFolder under the user's default contact folder](user-post-contactfolders.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c0c3f-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c0c3f-108">Permissions</span></span>
<span data-ttu-id="c0c3f-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0c3f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c3f-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c0c3f-111">Permission type</span></span>      | <span data-ttu-id="c0c3f-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c0c3f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c0c3f-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c0c3f-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c0c3f-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0c3f-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c0c3f-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c0c3f-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c0c3f-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0c3f-116">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="c0c3f-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c0c3f-117">Application</span></span> | <span data-ttu-id="c0c3f-118">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c0c3f-118">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="c0c3f-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0c3f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/contactFolders/{id}/childFolders
POST /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="request-headers"></a><span data-ttu-id="c0c3f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c0c3f-120">Request headers</span></span>
| <span data-ttu-id="c0c3f-121">Header</span><span class="sxs-lookup"><span data-stu-id="c0c3f-121">Header</span></span>       | <span data-ttu-id="c0c3f-122">Wert</span><span class="sxs-lookup"><span data-stu-id="c0c3f-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c0c3f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0c3f-123">Authorization</span></span>  | <span data-ttu-id="c0c3f-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c0c3f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c0c3f-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c0c3f-126">Content-Type</span></span>  | <span data-ttu-id="c0c3f-p104">application/json. Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="c0c3f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c0c3f-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c0c3f-129">Request body</span></span>
<span data-ttu-id="c0c3f-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [ContactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c0c3f-130">In the request body, supply a JSON representation of [ContactFolder](../resources/contactfolder.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c0c3f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0c3f-131">Response</span></span>

<span data-ttu-id="c0c3f-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [ContactFolder](../resources/contactfolder.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0c3f-132">If successful, this method returns `201 Created` response code and [ContactFolder](../resources/contactfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0c3f-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c0c3f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c0c3f-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c0c3f-134">Request</span></span>
<span data-ttu-id="c0c3f-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c0c3f-135">Here is an example of the request.</span></span>
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
<span data-ttu-id="c0c3f-136">Geben Sie im Anforderungstext eine JSON-Darstellung des [contactFolder](../resources/contactfolder.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="c0c3f-136">In the request body, supply a JSON representation of [contactFolder](../resources/contactfolder.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c0c3f-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="c0c3f-137">Response</span></span>
<span data-ttu-id="c0c3f-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0c3f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
