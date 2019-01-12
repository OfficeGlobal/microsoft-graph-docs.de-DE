---
title: Liste Gerätegruppen
description: Rufen Sie die Gruppen, denen dieses Gerät ein direktes Mitglied ist. Dieser Vorgang ist nicht transitiv.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1642b6ee758af5d2ab4004ea5b7a5293f33f7d01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912379"
---
# <a name="list-device-groups"></a><span data-ttu-id="2e25b-104">Liste Gerätegruppen</span><span class="sxs-lookup"><span data-stu-id="2e25b-104">List device groups</span></span>

<span data-ttu-id="2e25b-105">Rufen Sie die Gruppen, denen dieses Gerät ein direktes Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="2e25b-105">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="2e25b-106">Dieser Vorgang ist nicht transitiv.</span><span class="sxs-lookup"><span data-stu-id="2e25b-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e25b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2e25b-107">Permissions</span></span>

<span data-ttu-id="2e25b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e25b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e25b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2e25b-110">Permission type</span></span>      | <span data-ttu-id="2e25b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2e25b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e25b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2e25b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2e25b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2e25b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2e25b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2e25b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e25b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2e25b-115">Not supported.</span></span>    |
|<span data-ttu-id="2e25b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2e25b-116">Application</span></span> | <span data-ttu-id="2e25b-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e25b-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e25b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e25b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2e25b-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2e25b-119">Optional query parameters</span></span>
<span data-ttu-id="2e25b-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2e25b-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2e25b-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2e25b-121">Request headers</span></span>
| <span data-ttu-id="2e25b-122">Header</span><span class="sxs-lookup"><span data-stu-id="2e25b-122">Header</span></span>       | <span data-ttu-id="2e25b-123">Wert</span><span class="sxs-lookup"><span data-stu-id="2e25b-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2e25b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e25b-124">Authorization</span></span>  | <span data-ttu-id="2e25b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2e25b-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2e25b-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="2e25b-127">Accept</span></span>  | <span data-ttu-id="2e25b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2e25b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e25b-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2e25b-129">Request body</span></span>
<span data-ttu-id="2e25b-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2e25b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e25b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e25b-131">Response</span></span>

<span data-ttu-id="2e25b-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e25b-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e25b-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2e25b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e25b-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2e25b-134">Request</span></span>

<span data-ttu-id="2e25b-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2e25b-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="2e25b-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="2e25b-136">Response</span></span>
<span data-ttu-id="2e25b-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2e25b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
