---
title: registeredUsers auflisten
description: Dient zum Abrufen einer Liste von Benutzern, die registrierte Benutzer des Geräts sind.
ms.openlocfilehash: 08c6cc2268daa31b0d365e0201536df3586a798c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060555"
---
# <a name="list-registeredusers"></a><span data-ttu-id="209a7-103">registeredUsers auflisten</span><span class="sxs-lookup"><span data-stu-id="209a7-103">List registeredUsers</span></span>

> <span data-ttu-id="209a7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="209a7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="209a7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="209a7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="209a7-106">Dient zum Abrufen einer Liste von Benutzern, die registrierte Benutzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="209a7-106">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="209a7-107">Für mit der Cloud verknüpfte Geräte und registrierte persönliche Geräte werden registrierte Benutzer bei der Registrierung auf den gleichen Wert wie registrierte Besitzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="209a7-107">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="209a7-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="209a7-108">Permissions</span></span>
<span data-ttu-id="209a7-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="209a7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="209a7-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="209a7-111">Permission type</span></span>      | <span data-ttu-id="209a7-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="209a7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="209a7-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="209a7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="209a7-114">Directory.Read.All oder Directory.ReadWrite.All oder Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="209a7-114">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="209a7-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="209a7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="209a7-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="209a7-116">Not supported.</span></span> |
|<span data-ttu-id="209a7-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="209a7-117">Application</span></span> | <span data-ttu-id="209a7-118">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="209a7-118">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="209a7-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="209a7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="209a7-120">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="209a7-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="209a7-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="209a7-121">Optional query parameters</span></span>
<span data-ttu-id="209a7-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="209a7-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="209a7-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="209a7-123">Request headers</span></span>
| <span data-ttu-id="209a7-124">Name</span><span class="sxs-lookup"><span data-stu-id="209a7-124">Name</span></span>       | <span data-ttu-id="209a7-125">Typ</span><span class="sxs-lookup"><span data-stu-id="209a7-125">Type</span></span> | <span data-ttu-id="209a7-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="209a7-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="209a7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="209a7-127">Authorization</span></span>  | <span data-ttu-id="209a7-128">string</span><span class="sxs-lookup"><span data-stu-id="209a7-128">string</span></span>  | <span data-ttu-id="209a7-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="209a7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="209a7-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="209a7-131">Request body</span></span>
<span data-ttu-id="209a7-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="209a7-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="209a7-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="209a7-133">Response</span></span>

<span data-ttu-id="209a7-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="209a7-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="209a7-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="209a7-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="209a7-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="209a7-136">Request</span></span>
<span data-ttu-id="209a7-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="209a7-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="209a7-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="209a7-138">Response</span></span>
<span data-ttu-id="209a7-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="209a7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->