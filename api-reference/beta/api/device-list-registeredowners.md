---
title: registeredOwners auflisten
description: Dient zum Abrufen einer Liste von Benutzern, die registrierte Besitzer des Geräts sind. Ein registrierter Besitzer ist der Benutzer, dessen Gerät mit der Cloud verknüpft ist oder der sein persönliches Gerät registriert hat. Der registrierte Besitzer wird zum Zeitpunkt der Registrierung festgelegt. Derzeit kann jeweils nur ein Besitzer vorhanden sein.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4b9020c4fad74990a18023bdddd63ae3bd050998
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522959"
---
# <a name="list-registeredowners"></a><span data-ttu-id="8ce1a-106">registeredOwners auflisten</span><span class="sxs-lookup"><span data-stu-id="8ce1a-106">List registeredOwners</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ce1a-107">Dient zum Abrufen einer Liste von Benutzern, die registrierte Besitzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="8ce1a-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="8ce1a-108">Ein registrierter Besitzer ist der Benutzer, dessen Gerät mit der Cloud verknüpft ist oder der sein persönliches Gerät registriert hat.</span><span class="sxs-lookup"><span data-stu-id="8ce1a-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="8ce1a-109">Der registrierte Besitzer wird zum Zeitpunkt der Registrierung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="8ce1a-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="8ce1a-110">Derzeit kann jeweils nur ein Besitzer vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="8ce1a-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ce1a-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8ce1a-111">Permissions</span></span>

<span data-ttu-id="8ce1a-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ce1a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ce1a-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8ce1a-114">Permission type</span></span>      | <span data-ttu-id="8ce1a-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8ce1a-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ce1a-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8ce1a-116">Delegated (work or school account)</span></span> | <span data-ttu-id="8ce1a-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8ce1a-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8ce1a-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8ce1a-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ce1a-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8ce1a-119">Not supported.</span></span>    |
|<span data-ttu-id="8ce1a-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8ce1a-120">Application</span></span> | <span data-ttu-id="8ce1a-121">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ce1a-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ce1a-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ce1a-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="8ce1a-123">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="8ce1a-123">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="8ce1a-124">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="8ce1a-124">Optional query parameters</span></span>
<span data-ttu-id="8ce1a-125">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8ce1a-125">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="8ce1a-126">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8ce1a-126">Request headers</span></span>
| <span data-ttu-id="8ce1a-127">Name</span><span class="sxs-lookup"><span data-stu-id="8ce1a-127">Name</span></span>       | <span data-ttu-id="8ce1a-128">Typ</span><span class="sxs-lookup"><span data-stu-id="8ce1a-128">Type</span></span> | <span data-ttu-id="8ce1a-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ce1a-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8ce1a-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ce1a-130">Authorization</span></span>  | <span data-ttu-id="8ce1a-131">string</span><span class="sxs-lookup"><span data-stu-id="8ce1a-131">string</span></span>  | <span data-ttu-id="8ce1a-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8ce1a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ce1a-134">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8ce1a-134">Request body</span></span>
<span data-ttu-id="8ce1a-135">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8ce1a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ce1a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ce1a-136">Response</span></span>

<span data-ttu-id="8ce1a-137">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ce1a-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8ce1a-138">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8ce1a-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ce1a-139">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8ce1a-139">Request</span></span>
<span data-ttu-id="8ce1a-140">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8ce1a-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="8ce1a-141">Antwort</span><span class="sxs-lookup"><span data-stu-id="8ce1a-141">Response</span></span>
<span data-ttu-id="8ce1a-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8ce1a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-list-registeredowners.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
