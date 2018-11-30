---
title: registeredOwners auflisten
description: Dient zum Abrufen einer Liste von Benutzern, die registrierte Besitzer des Geräts sind. Ein registrierter Besitzer ist der Benutzer, dessen Gerät mit der Cloud verknüpft ist oder der sein persönliches Gerät registriert hat. Der registrierte Besitzer wird zum Zeitpunkt der Registrierung festgelegt. Derzeit kann jeweils nur ein Besitzer vorhanden sein.
ms.openlocfilehash: 7a56e036ac904f98fdc1cc2d4f781f97f43c85dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016828"
---
# <a name="list-registeredowners"></a><span data-ttu-id="56bf1-106">registeredOwners auflisten</span><span class="sxs-lookup"><span data-stu-id="56bf1-106">List registeredOwners</span></span>

<span data-ttu-id="56bf1-107">Dient zum Abrufen einer Liste von Benutzern, die registrierte Besitzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="56bf1-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="56bf1-108">Ein registrierter Besitzer ist der Benutzer, dessen Gerät mit der Cloud verknüpft ist oder der sein persönliches Gerät registriert hat.</span><span class="sxs-lookup"><span data-stu-id="56bf1-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="56bf1-109">Der registrierte Besitzer wird zum Zeitpunkt der Registrierung festgelegt.</span><span class="sxs-lookup"><span data-stu-id="56bf1-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="56bf1-110">Derzeit kann jeweils nur ein Besitzer vorhanden sein.</span><span class="sxs-lookup"><span data-stu-id="56bf1-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="56bf1-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="56bf1-111">Permissions</span></span>
<span data-ttu-id="56bf1-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56bf1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="56bf1-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="56bf1-114">Permission type</span></span>      | <span data-ttu-id="56bf1-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="56bf1-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56bf1-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="56bf1-116">Delegated (work or school account)</span></span> | <span data-ttu-id="56bf1-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="56bf1-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="56bf1-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="56bf1-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56bf1-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="56bf1-119">Not supported.</span></span>    |
|<span data-ttu-id="56bf1-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="56bf1-120">Application</span></span> | <span data-ttu-id="56bf1-121">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56bf1-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="56bf1-122">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="56bf1-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="56bf1-123">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="56bf1-123">Optional query parameters</span></span>
<span data-ttu-id="56bf1-124">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="56bf1-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="56bf1-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="56bf1-125">Request headers</span></span>
| <span data-ttu-id="56bf1-126">Name</span><span class="sxs-lookup"><span data-stu-id="56bf1-126">Name</span></span>       | <span data-ttu-id="56bf1-127">Typ</span><span class="sxs-lookup"><span data-stu-id="56bf1-127">Type</span></span> | <span data-ttu-id="56bf1-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="56bf1-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="56bf1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="56bf1-129">Authorization</span></span>  | <span data-ttu-id="56bf1-130">string</span><span class="sxs-lookup"><span data-stu-id="56bf1-130">string</span></span>  | <span data-ttu-id="56bf1-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="56bf1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56bf1-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="56bf1-133">Request body</span></span>
<span data-ttu-id="56bf1-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="56bf1-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56bf1-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="56bf1-135">Response</span></span>

<span data-ttu-id="56bf1-136">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56bf1-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="56bf1-137">Beispiel</span><span class="sxs-lookup"><span data-stu-id="56bf1-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56bf1-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="56bf1-138">Request</span></span>
<span data-ttu-id="56bf1-139">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="56bf1-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="56bf1-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="56bf1-140">Response</span></span>
<span data-ttu-id="56bf1-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="56bf1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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