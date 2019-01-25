---
title: registeredUsers auflisten
description: Dient zum Abrufen einer Liste von Benutzern, die registrierte Benutzer des Geräts sind.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c5327c246c3a1dc58b0b1431fdff330cf7b6a732
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526312"
---
# <a name="list-registeredusers"></a><span data-ttu-id="4033c-103">registeredUsers auflisten</span><span class="sxs-lookup"><span data-stu-id="4033c-103">List registeredUsers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4033c-104">Dient zum Abrufen einer Liste von Benutzern, die registrierte Benutzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="4033c-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="4033c-105">Für mit der Cloud verknüpfte Geräte und registrierte persönliche Geräte werden registrierte Benutzer bei der Registrierung auf den gleichen Wert wie registrierte Besitzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="4033c-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="4033c-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4033c-106">Permissions</span></span>
<span data-ttu-id="4033c-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4033c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4033c-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4033c-109">Permission type</span></span>      | <span data-ttu-id="4033c-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4033c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4033c-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4033c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4033c-112">Directory.Read.All oder Directory.ReadWrite.All oder Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4033c-112">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4033c-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4033c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4033c-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4033c-114">Not supported.</span></span> |
|<span data-ttu-id="4033c-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4033c-115">Application</span></span> | <span data-ttu-id="4033c-116">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4033c-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4033c-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4033c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="4033c-118">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="4033c-118">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="4033c-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4033c-119">Optional query parameters</span></span>
<span data-ttu-id="4033c-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4033c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4033c-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4033c-121">Request headers</span></span>
| <span data-ttu-id="4033c-122">Name</span><span class="sxs-lookup"><span data-stu-id="4033c-122">Name</span></span>       | <span data-ttu-id="4033c-123">Typ</span><span class="sxs-lookup"><span data-stu-id="4033c-123">Type</span></span> | <span data-ttu-id="4033c-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4033c-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4033c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="4033c-125">Authorization</span></span>  | <span data-ttu-id="4033c-126">string</span><span class="sxs-lookup"><span data-stu-id="4033c-126">string</span></span>  | <span data-ttu-id="4033c-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4033c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4033c-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4033c-129">Request body</span></span>
<span data-ttu-id="4033c-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4033c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4033c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="4033c-131">Response</span></span>

<span data-ttu-id="4033c-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4033c-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4033c-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4033c-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4033c-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4033c-134">Request</span></span>
<span data-ttu-id="4033c-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4033c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="4033c-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="4033c-136">Response</span></span>
<span data-ttu-id="4033c-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4033c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-list-registeredusers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
