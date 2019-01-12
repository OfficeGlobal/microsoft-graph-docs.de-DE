---
title: registeredUsers auflisten
description: Dient zum Abrufen einer Liste von Benutzern, die registrierte Benutzer des Geräts sind.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14b7c3b31d2edfde093a0c5d8cd1ed48a25ba1cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954218"
---
# <a name="list-registeredusers"></a><span data-ttu-id="2de1f-103">registeredUsers auflisten</span><span class="sxs-lookup"><span data-stu-id="2de1f-103">List registeredUsers</span></span>

<span data-ttu-id="2de1f-104">Dient zum Abrufen einer Liste von Benutzern, die registrierte Benutzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="2de1f-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="2de1f-105">Für mit der Cloud verknüpfte Geräte und registrierte persönliche Geräte werden registrierte Benutzer bei der Registrierung auf den gleichen Wert wie registrierte Besitzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="2de1f-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="2de1f-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2de1f-106">Permissions</span></span>
<span data-ttu-id="2de1f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2de1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2de1f-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2de1f-109">Permission type</span></span>      | <span data-ttu-id="2de1f-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2de1f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2de1f-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2de1f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2de1f-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2de1f-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2de1f-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2de1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2de1f-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2de1f-114">Not supported.</span></span>    |
|<span data-ttu-id="2de1f-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2de1f-115">Application</span></span> | <span data-ttu-id="2de1f-116">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2de1f-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2de1f-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2de1f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2de1f-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="2de1f-118">Optional query parameters</span></span>
<span data-ttu-id="2de1f-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2de1f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2de1f-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2de1f-120">Request headers</span></span>
| <span data-ttu-id="2de1f-121">Name</span><span class="sxs-lookup"><span data-stu-id="2de1f-121">Name</span></span>       | <span data-ttu-id="2de1f-122">Typ</span><span class="sxs-lookup"><span data-stu-id="2de1f-122">Type</span></span> | <span data-ttu-id="2de1f-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2de1f-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2de1f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2de1f-124">Authorization</span></span>  | <span data-ttu-id="2de1f-125">string</span><span class="sxs-lookup"><span data-stu-id="2de1f-125">string</span></span>  | <span data-ttu-id="2de1f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2de1f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2de1f-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2de1f-128">Request body</span></span>
<span data-ttu-id="2de1f-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="2de1f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2de1f-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="2de1f-130">Response</span></span>

<span data-ttu-id="2de1f-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2de1f-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2de1f-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2de1f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2de1f-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2de1f-133">Request</span></span>
<span data-ttu-id="2de1f-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2de1f-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="2de1f-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="2de1f-135">Response</span></span>
<span data-ttu-id="2de1f-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2de1f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
