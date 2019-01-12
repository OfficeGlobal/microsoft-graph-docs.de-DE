---
title: createdObjects auflisten
description: Mit dieser API können Sie eine Liste aller vom betreffenden Benutzer erstellten Verzeichnisobjekte abrufen.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f8d420e60b96cbcc65fff8ba9b29942c9ee4ecd9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944166"
---
# <a name="list-createdobjects"></a><span data-ttu-id="5be68-103">createdObjects auflisten</span><span class="sxs-lookup"><span data-stu-id="5be68-103">List createdObjects</span></span>

> <span data-ttu-id="5be68-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="5be68-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5be68-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5be68-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5be68-106">Mit dieser API können Sie eine Liste aller vom betreffenden Benutzer erstellten Verzeichnisobjekte abrufen.</span><span class="sxs-lookup"><span data-stu-id="5be68-106">Get a list of directory objects that were created by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="5be68-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5be68-107">Permissions</span></span>
<span data-ttu-id="5be68-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5be68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5be68-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5be68-110">Permission type</span></span>      | <span data-ttu-id="5be68-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5be68-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5be68-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5be68-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5be68-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5be68-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5be68-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5be68-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5be68-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5be68-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="5be68-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5be68-116">Application</span></span> | <span data-ttu-id="5be68-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5be68-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5be68-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5be68-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5be68-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5be68-119">Optional query parameters</span></span>
<span data-ttu-id="5be68-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5be68-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5be68-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5be68-121">Request headers</span></span>
| <span data-ttu-id="5be68-122">Header</span><span class="sxs-lookup"><span data-stu-id="5be68-122">Header</span></span>       | <span data-ttu-id="5be68-123">Wert</span><span class="sxs-lookup"><span data-stu-id="5be68-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5be68-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5be68-124">Authorization</span></span>  | <span data-ttu-id="5be68-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5be68-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5be68-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5be68-127">Content-Type</span></span>  | <span data-ttu-id="5be68-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5be68-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5be68-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5be68-129">Request body</span></span>
<span data-ttu-id="5be68-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5be68-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5be68-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5be68-131">Response</span></span>

<span data-ttu-id="5be68-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5be68-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5be68-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5be68-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5be68-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5be68-134">Request</span></span>
<span data-ttu-id="5be68-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5be68-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/beta/me/createdObjects
```
##### <a name="response"></a><span data-ttu-id="5be68-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5be68-136">Response</span></span>
<span data-ttu-id="5be68-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5be68-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
