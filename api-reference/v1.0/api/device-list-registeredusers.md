---
title: registeredUsers auflisten
description: Dient zum Abrufen einer Liste von Benutzern, die registrierte Benutzer des Geräts sind.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 58b691bbf71dde1aa6247cfa19164f8cc44b3674
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846389"
---
# <a name="list-registeredusers"></a><span data-ttu-id="1fa6b-103">registeredUsers auflisten</span><span class="sxs-lookup"><span data-stu-id="1fa6b-103">List registeredUsers</span></span>

<span data-ttu-id="1fa6b-104">Dient zum Abrufen einer Liste von Benutzern, die registrierte Benutzer des Geräts sind.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-104">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="1fa6b-105">Für mit der Cloud verknüpfte Geräte und registrierte persönliche Geräte werden registrierte Benutzer bei der Registrierung auf den gleichen Wert wie registrierte Besitzer festgelegt.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-105">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="1fa6b-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1fa6b-106">Permissions</span></span>
<span data-ttu-id="1fa6b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1fa6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1fa6b-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1fa6b-109">Permission type</span></span>      | <span data-ttu-id="1fa6b-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1fa6b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1fa6b-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1fa6b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1fa6b-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1fa6b-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1fa6b-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1fa6b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fa6b-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1fa6b-114">Not supported.</span></span>    |
|<span data-ttu-id="1fa6b-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1fa6b-115">Application</span></span> | <span data-ttu-id="1fa6b-116">Directory.Read.All oder Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1fa6b-116">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1fa6b-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1fa6b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1fa6b-118">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="1fa6b-118">Optional query parameters</span></span>
<span data-ttu-id="1fa6b-119">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1fa6b-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1fa6b-120">Request headers</span></span>
| <span data-ttu-id="1fa6b-121">Name</span><span class="sxs-lookup"><span data-stu-id="1fa6b-121">Name</span></span>       | <span data-ttu-id="1fa6b-122">Typ</span><span class="sxs-lookup"><span data-stu-id="1fa6b-122">Type</span></span> | <span data-ttu-id="1fa6b-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1fa6b-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1fa6b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fa6b-124">Authorization</span></span>  | <span data-ttu-id="1fa6b-125">string</span><span class="sxs-lookup"><span data-stu-id="1fa6b-125">string</span></span>  | <span data-ttu-id="1fa6b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1fa6b-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1fa6b-128">Request body</span></span>
<span data-ttu-id="1fa6b-129">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1fa6b-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="1fa6b-130">Response</span></span>

<span data-ttu-id="1fa6b-131">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1fa6b-132">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1fa6b-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1fa6b-133">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1fa6b-133">Request</span></span>
<span data-ttu-id="1fa6b-134">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="1fa6b-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="1fa6b-135">Response</span></span>
<span data-ttu-id="1fa6b-p103">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1fa6b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
