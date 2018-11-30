---
title: ownedDevices auflisten
description: Mit dieser API können Sie eine Liste aller Geräte abrufen, denen der betreffende Benutzer als Besitzer zugewiesen ist.
ms.openlocfilehash: 2346c40fa8d74c71decc16170506a7ad6dc7bdb1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016073"
---
# <a name="list-owneddevices"></a><span data-ttu-id="e2782-103">ownedDevices auflisten</span><span class="sxs-lookup"><span data-stu-id="e2782-103">List ownedDevices</span></span>

<span data-ttu-id="e2782-104">Mit dieser API können Sie eine Liste aller Geräte abrufen, denen der betreffende Benutzer als Besitzer zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="e2782-104">Get the list of devices that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="e2782-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="e2782-105">Permissions</span></span>
<span data-ttu-id="e2782-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2782-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2782-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="e2782-108">Permission type</span></span>      | <span data-ttu-id="e2782-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="e2782-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2782-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="e2782-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e2782-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e2782-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e2782-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="e2782-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2782-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="e2782-113">Not supported.</span></span>    |
|<span data-ttu-id="e2782-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="e2782-114">Application</span></span> | <span data-ttu-id="e2782-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2782-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2782-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2782-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e2782-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="e2782-117">Optional query parameters</span></span>
<span data-ttu-id="e2782-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e2782-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e2782-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="e2782-119">Request headers</span></span>
| <span data-ttu-id="e2782-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="e2782-120">Header</span></span>       | <span data-ttu-id="e2782-121">Wert</span><span class="sxs-lookup"><span data-stu-id="e2782-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e2782-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2782-122">Authorization</span></span>  | <span data-ttu-id="e2782-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="e2782-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e2782-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e2782-125">Accept</span></span>  | <span data-ttu-id="e2782-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2782-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2782-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="e2782-127">Request body</span></span>
<span data-ttu-id="e2782-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="e2782-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2782-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2782-129">Response</span></span>

<span data-ttu-id="e2782-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2782-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e2782-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e2782-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e2782-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e2782-132">Request</span></span>
<span data-ttu-id="e2782-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e2782-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owneddevices"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/ownedDevices
```
##### <a name="response"></a><span data-ttu-id="e2782-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="e2782-134">Response</span></span>
<span data-ttu-id="e2782-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e2782-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List ownedDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->