---
title: registeredOwners auflisten
description: Dient zum Abrufen einer Liste von Benutzern, die registrierte Besitzer des Geräts sind. Ein registrierter Besitzer ist der Benutzer, dessen Gerät mit der Cloud verknüpft ist oder der sein persönliches Gerät registriert hat. Der registrierte Besitzer wird zum Zeitpunkt der Registrierung festgelegt. Derzeit kann jeweils nur ein Besitzer vorhanden sein.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ec8990a2b0c2d0f674304c4005fbf28a0b5a631e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976891"
---
# <a name="list-registeredowners"></a><span data-ttu-id="4cffa-106">registeredOwners auflisten</span><span class="sxs-lookup"><span data-stu-id="4cffa-106">List registeredOwners</span></span>

<span data-ttu-id="4cffa-107">Dient zum Abrufen einer Liste von Benutzern, die registrierte Besitzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="4cffa-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="4cffa-108">Ein registrierter Besitzer ist der Benutzer, dessen Gerät mit der Cloud verknüpft ist oder der sein persönliches Gerät registriert hat.</span><span class="sxs-lookup"><span data-stu-id="4cffa-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="4cffa-109">Der registrierte Besitzer wird zum Zeitpunkt der Registrierung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="4cffa-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="4cffa-110">Derzeit kann jeweils nur ein Besitzer vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="4cffa-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cffa-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4cffa-111">Permissions</span></span>
<span data-ttu-id="4cffa-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cffa-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4cffa-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4cffa-114">Permission type</span></span>      | <span data-ttu-id="4cffa-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4cffa-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cffa-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4cffa-116">Delegated (work or school account)</span></span> | <span data-ttu-id="4cffa-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4cffa-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4cffa-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4cffa-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cffa-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4cffa-119">Not supported.</span></span>    |
|<span data-ttu-id="4cffa-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4cffa-120">Application</span></span> | <span data-ttu-id="4cffa-121">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cffa-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cffa-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cffa-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4cffa-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4cffa-123">Optional query parameters</span></span>
<span data-ttu-id="4cffa-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4cffa-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4cffa-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4cffa-125">Request headers</span></span>
| <span data-ttu-id="4cffa-126">Name</span><span class="sxs-lookup"><span data-stu-id="4cffa-126">Name</span></span>       | <span data-ttu-id="4cffa-127">Typ</span><span class="sxs-lookup"><span data-stu-id="4cffa-127">Type</span></span> | <span data-ttu-id="4cffa-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4cffa-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4cffa-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cffa-129">Authorization</span></span>  | <span data-ttu-id="4cffa-130">string</span><span class="sxs-lookup"><span data-stu-id="4cffa-130">string</span></span>  | <span data-ttu-id="4cffa-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4cffa-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4cffa-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4cffa-133">Request body</span></span>
<span data-ttu-id="4cffa-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4cffa-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cffa-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cffa-135">Response</span></span>

<span data-ttu-id="4cffa-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4cffa-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4cffa-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4cffa-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cffa-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4cffa-138">Request</span></span>
<span data-ttu-id="4cffa-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4cffa-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="4cffa-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="4cffa-140">Response</span></span>
<span data-ttu-id="4cffa-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4cffa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
