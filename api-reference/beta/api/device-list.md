---
title: Geräte auflisten
description: 'Dient zum Abrufen einer Liste von Geräten, die in dem Verzeichnis registriert sind. '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: df612a24d9ffd50a432d7b6787b60de62764723c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511023"
---
# <a name="list-devices"></a><span data-ttu-id="1947b-103">Geräte auflisten</span><span class="sxs-lookup"><span data-stu-id="1947b-103">List devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1947b-104">Dient zum Abrufen einer Liste von Geräten, die in dem Verzeichnis registriert sind.</span><span class="sxs-lookup"><span data-stu-id="1947b-104">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="1947b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1947b-105">Permissions</span></span>
<span data-ttu-id="1947b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1947b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1947b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1947b-108">Permission type</span></span>      | <span data-ttu-id="1947b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1947b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1947b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1947b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1947b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1947b-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1947b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1947b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1947b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1947b-113">Not supported.</span></span>    |
|<span data-ttu-id="1947b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1947b-114">Application</span></span> | <span data-ttu-id="1947b-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1947b-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1947b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1947b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1947b-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1947b-117">Optional query parameters</span></span>
<span data-ttu-id="1947b-118">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1947b-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1947b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1947b-119">Request headers</span></span>
| <span data-ttu-id="1947b-120">Name</span><span class="sxs-lookup"><span data-stu-id="1947b-120">Name</span></span>       | <span data-ttu-id="1947b-121">Typ</span><span class="sxs-lookup"><span data-stu-id="1947b-121">Type</span></span> | <span data-ttu-id="1947b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1947b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1947b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1947b-123">Authorization</span></span>  | <span data-ttu-id="1947b-124">string</span><span class="sxs-lookup"><span data-stu-id="1947b-124">string</span></span>  | <span data-ttu-id="1947b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1947b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1947b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1947b-127">Request body</span></span>
<span data-ttu-id="1947b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1947b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1947b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="1947b-129">Response</span></span>

<span data-ttu-id="1947b-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [device](../resources/device.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1947b-130">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1947b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1947b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1947b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1947b-132">Request</span></span>
<span data-ttu-id="1947b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1947b-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/beta/devices
```
##### <a name="response"></a><span data-ttu-id="1947b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="1947b-134">Response</span></span>
<span data-ttu-id="1947b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1947b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled": true,
      "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
      "deviceId": "deviceId-value",
      "deviceMetadata": "deviceMetadata-value",
      "displayName" : "displayName-value",
      "id" : "id-value", 
      "operatingSystem" : "operatingSystem-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
