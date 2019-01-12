---
title: registeredUsers auflisten
description: Dient zum Abrufen einer Liste von Benutzern, die registrierte Benutzer des Geräts sind.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d3a5e8dbc92860ac4829f4aa4c3e509e6f4ec9b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980601"
---
# <a name="list-registeredusers"></a><span data-ttu-id="3761e-103">registeredUsers auflisten</span><span class="sxs-lookup"><span data-stu-id="3761e-103">List registeredUsers</span></span>

> <span data-ttu-id="3761e-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3761e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3761e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3761e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3761e-106">Dient zum Abrufen einer Liste von Benutzern, die registrierte Benutzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="3761e-106">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="3761e-107">Für mit der Cloud verknüpfte Geräte und registrierte persönliche Geräte werden registrierte Benutzer bei der Registrierung auf den gleichen Wert wie registrierte Besitzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="3761e-107">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="3761e-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3761e-108">Permissions</span></span>
<span data-ttu-id="3761e-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3761e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3761e-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3761e-111">Permission type</span></span>      | <span data-ttu-id="3761e-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3761e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3761e-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3761e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3761e-114">Directory.Read.All oder Directory.ReadWrite.All oder Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3761e-114">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3761e-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3761e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3761e-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3761e-116">Not supported.</span></span> |
|<span data-ttu-id="3761e-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3761e-117">Application</span></span> | <span data-ttu-id="3761e-118">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3761e-118">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3761e-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3761e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="3761e-120">Hinweis: Die „id“ in der Anforderung entspricht der „id“-Eigenschaft des Geräts, nicht der „deviceId“-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="3761e-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="3761e-121">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="3761e-121">Optional query parameters</span></span>
<span data-ttu-id="3761e-122">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="3761e-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3761e-123">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3761e-123">Request headers</span></span>
| <span data-ttu-id="3761e-124">Name</span><span class="sxs-lookup"><span data-stu-id="3761e-124">Name</span></span>       | <span data-ttu-id="3761e-125">Typ</span><span class="sxs-lookup"><span data-stu-id="3761e-125">Type</span></span> | <span data-ttu-id="3761e-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3761e-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3761e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="3761e-127">Authorization</span></span>  | <span data-ttu-id="3761e-128">string</span><span class="sxs-lookup"><span data-stu-id="3761e-128">string</span></span>  | <span data-ttu-id="3761e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3761e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3761e-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3761e-131">Request body</span></span>
<span data-ttu-id="3761e-132">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3761e-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3761e-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="3761e-133">Response</span></span>

<span data-ttu-id="3761e-134">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3761e-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3761e-135">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3761e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3761e-136">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3761e-136">Request</span></span>
<span data-ttu-id="3761e-137">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3761e-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="3761e-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="3761e-138">Response</span></span>
<span data-ttu-id="3761e-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="3761e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
