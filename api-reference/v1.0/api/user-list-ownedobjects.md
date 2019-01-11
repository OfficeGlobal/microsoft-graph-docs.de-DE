---
title: ownedObjects auflisten
description: Mit dieser API können Sie eine Liste aller Verzeichnisobjekte abrufen, denen ein Benutzer als Besitzer zugewiesen ist.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: fc9a39ef672d62cb0f68a8cca09aecf8d6507b90
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811501"
---
# <a name="list-ownedobjects"></a><span data-ttu-id="bc884-103">ownedObjects auflisten</span><span class="sxs-lookup"><span data-stu-id="bc884-103">List ownedObjects</span></span>

<span data-ttu-id="bc884-104">Mit dieser API können Sie eine Liste aller Verzeichnisobjekte abrufen, denen ein Benutzer als Besitzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="bc884-104">Get the list of directory objects that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="bc884-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="bc884-105">Permissions</span></span>
<span data-ttu-id="bc884-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc884-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc884-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="bc884-108">Permission type</span></span>      | <span data-ttu-id="bc884-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="bc884-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc884-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="bc884-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bc884-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bc884-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bc884-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="bc884-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc884-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="bc884-113">Not supported.</span></span>    |
|<span data-ttu-id="bc884-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="bc884-114">Application</span></span> | <span data-ttu-id="bc884-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc884-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc884-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc884-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bc884-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="bc884-117">Optional query parameters</span></span>
<span data-ttu-id="bc884-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="bc884-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bc884-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="bc884-119">Request headers</span></span>
| <span data-ttu-id="bc884-120">Header</span><span class="sxs-lookup"><span data-stu-id="bc884-120">Header</span></span>       | <span data-ttu-id="bc884-121">Wert</span><span class="sxs-lookup"><span data-stu-id="bc884-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bc884-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc884-122">Authorization</span></span>  | <span data-ttu-id="bc884-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="bc884-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bc884-125">Annehmen</span><span class="sxs-lookup"><span data-stu-id="bc884-125">Accept</span></span>  | <span data-ttu-id="bc884-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bc884-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc884-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="bc884-127">Request body</span></span>
<span data-ttu-id="bc884-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="bc884-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bc884-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc884-129">Response</span></span>

<span data-ttu-id="bc884-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc884-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bc884-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="bc884-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc884-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="bc884-132">Request</span></span>
<span data-ttu-id="bc884-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="bc884-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/ownedObjects
```
##### <a name="response"></a><span data-ttu-id="bc884-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="bc884-134">Response</span></span>
<span data-ttu-id="bc884-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="bc884-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
