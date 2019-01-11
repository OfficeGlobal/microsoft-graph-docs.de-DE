---
title: Liste Gerätegruppen
description: Rufen Sie die Gruppen, denen dieses Gerät ein direktes Mitglied ist. Dieser Vorgang ist nicht transitiv.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a189b6fc0c06862b444d741767c20a46f0fa115a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804809"
---
# <a name="list-device-groups"></a><span data-ttu-id="5b380-104">Liste Gerätegruppen</span><span class="sxs-lookup"><span data-stu-id="5b380-104">List device groups</span></span>

<span data-ttu-id="5b380-105">Rufen Sie die Gruppen, denen dieses Gerät ein direktes Mitglied ist.</span><span class="sxs-lookup"><span data-stu-id="5b380-105">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="5b380-106">Dieser Vorgang ist nicht transitiv.</span><span class="sxs-lookup"><span data-stu-id="5b380-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b380-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="5b380-107">Permissions</span></span>

<span data-ttu-id="5b380-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b380-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b380-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="5b380-110">Permission type</span></span>      | <span data-ttu-id="5b380-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="5b380-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5b380-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="5b380-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5b380-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5b380-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="5b380-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="5b380-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b380-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="5b380-115">Not supported.</span></span>    |
|<span data-ttu-id="5b380-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="5b380-116">Application</span></span> | <span data-ttu-id="5b380-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b380-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b380-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b380-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5b380-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="5b380-119">Optional query parameters</span></span>
<span data-ttu-id="5b380-120">Diese Methode unterstützt die [OData-Abfrageparameter](/graph/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="5b380-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5b380-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="5b380-121">Request headers</span></span>
| <span data-ttu-id="5b380-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="5b380-122">Header</span></span>       | <span data-ttu-id="5b380-123">Wert</span><span class="sxs-lookup"><span data-stu-id="5b380-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5b380-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b380-124">Authorization</span></span>  | <span data-ttu-id="5b380-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="5b380-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5b380-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="5b380-127">Accept</span></span>  | <span data-ttu-id="5b380-128">application/json</span><span class="sxs-lookup"><span data-stu-id="5b380-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b380-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="5b380-129">Request body</span></span>
<span data-ttu-id="5b380-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="5b380-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b380-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b380-131">Response</span></span>

<span data-ttu-id="5b380-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b380-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b380-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="5b380-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b380-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="5b380-134">Request</span></span>

<span data-ttu-id="5b380-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="5b380-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="5b380-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="5b380-136">Response</span></span>
<span data-ttu-id="5b380-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="5b380-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
