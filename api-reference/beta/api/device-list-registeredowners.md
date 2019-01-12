---
title: registeredOwners auflisten
description: Dient zum Abrufen einer Liste von Benutzern, die registrierte Besitzer des Geräts sind. Ein registrierter Besitzer ist der Benutzer, dessen Gerät mit der Cloud verknüpft ist oder der sein persönliches Gerät registriert hat. Der registrierte Besitzer wird zum Zeitpunkt der Registrierung festgelegt. Derzeit kann jeweils nur ein Besitzer vorhanden sein.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ebf6350de33d2dfa70f9c098cd618abf7d7df4ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931713"
---
# <a name="list-registeredowners"></a><span data-ttu-id="fd70f-106">registeredOwners auflisten</span><span class="sxs-lookup"><span data-stu-id="fd70f-106">List registeredOwners</span></span>

> <span data-ttu-id="fd70f-107">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="fd70f-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd70f-108">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fd70f-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd70f-109">Dient zum Abrufen einer Liste von Benutzern, die registrierte Besitzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="fd70f-109">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="fd70f-110">Ein registrierter Besitzer ist der Benutzer, dessen Gerät mit der Cloud verknüpft ist oder der sein persönliches Gerät registriert hat.</span><span class="sxs-lookup"><span data-stu-id="fd70f-110">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="fd70f-111">Der registrierte Besitzer wird zum Zeitpunkt der Registrierung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="fd70f-111">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="fd70f-112">Derzeit kann jeweils nur ein Besitzer vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="fd70f-112">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd70f-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fd70f-113">Permissions</span></span>

<span data-ttu-id="fd70f-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd70f-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd70f-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fd70f-116">Permission type</span></span>      | <span data-ttu-id="fd70f-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fd70f-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd70f-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fd70f-118">Delegated (work or school account)</span></span> | <span data-ttu-id="fd70f-119">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fd70f-119">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fd70f-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fd70f-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd70f-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fd70f-121">Not supported.</span></span>    |
|<span data-ttu-id="fd70f-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fd70f-122">Application</span></span> | <span data-ttu-id="fd70f-123">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd70f-123">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd70f-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd70f-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```

> <span data-ttu-id="fd70f-125">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="fd70f-125">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="fd70f-126">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="fd70f-126">Optional query parameters</span></span>
<span data-ttu-id="fd70f-127">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="fd70f-127">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fd70f-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fd70f-128">Request headers</span></span>
| <span data-ttu-id="fd70f-129">Name</span><span class="sxs-lookup"><span data-stu-id="fd70f-129">Name</span></span>       | <span data-ttu-id="fd70f-130">Typ</span><span class="sxs-lookup"><span data-stu-id="fd70f-130">Type</span></span> | <span data-ttu-id="fd70f-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fd70f-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fd70f-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd70f-132">Authorization</span></span>  | <span data-ttu-id="fd70f-133">string</span><span class="sxs-lookup"><span data-stu-id="fd70f-133">string</span></span>  | <span data-ttu-id="fd70f-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fd70f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd70f-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fd70f-136">Request body</span></span>
<span data-ttu-id="fd70f-137">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="fd70f-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd70f-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd70f-138">Response</span></span>

<span data-ttu-id="fd70f-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd70f-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd70f-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fd70f-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd70f-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fd70f-141">Request</span></span>
<span data-ttu-id="fd70f-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="fd70f-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="fd70f-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="fd70f-143">Response</span></span>
<span data-ttu-id="fd70f-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fd70f-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
