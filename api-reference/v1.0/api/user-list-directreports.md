---
title: directReports auflisten
description: Dient zum Abrufen des direkten Vorgesetzten des Benutzers. Gibt die Benutzer und Kontakte zurück, für die dieser Benutzer als Vorgesetzter zugewiesen ist.
localization_priority: Priority
ms.openlocfilehash: 1a654daf4483e274255c5bdf44c7ad26009177a3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823359"
---
# <a name="list-directreports"></a><span data-ttu-id="556fe-104">directReports auflisten</span><span class="sxs-lookup"><span data-stu-id="556fe-104">List directReports</span></span>

<span data-ttu-id="556fe-p102">Dient zum Abrufen des direkten Vorgesetzten des Benutzers. Gibt die Benutzer und Kontakte zurück, für die dieser Benutzer als Vorgesetzter zugewiesen ist.</span><span class="sxs-lookup"><span data-stu-id="556fe-p102">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="556fe-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="556fe-107">Permissions</span></span>
<span data-ttu-id="556fe-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="556fe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="556fe-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="556fe-110">Permission type</span></span>      | <span data-ttu-id="556fe-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="556fe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="556fe-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="556fe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="556fe-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="556fe-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="556fe-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="556fe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="556fe-115">User.Read, User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="556fe-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="556fe-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="556fe-116">Application</span></span> | <span data-ttu-id="556fe-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="556fe-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="556fe-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="556fe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="556fe-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="556fe-119">Optional query parameters</span></span>
<span data-ttu-id="556fe-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="556fe-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="556fe-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="556fe-121">Request headers</span></span>
| <span data-ttu-id="556fe-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="556fe-122">Header</span></span>       | <span data-ttu-id="556fe-123">Wert</span><span class="sxs-lookup"><span data-stu-id="556fe-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="556fe-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="556fe-124">Authorization</span></span>  | <span data-ttu-id="556fe-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="556fe-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="556fe-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="556fe-127">Content-Type</span></span>   | <span data-ttu-id="556fe-128">application/json</span><span class="sxs-lookup"><span data-stu-id="556fe-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="556fe-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="556fe-129">Request body</span></span>
<span data-ttu-id="556fe-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="556fe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="556fe-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="556fe-131">Response</span></span>

<span data-ttu-id="556fe-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="556fe-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="556fe-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="556fe-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="556fe-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="556fe-134">Request</span></span>
<span data-ttu-id="556fe-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="556fe-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/directReports
```
##### <a name="response"></a><span data-ttu-id="556fe-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="556fe-136">Response</span></span>
<span data-ttu-id="556fe-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="556fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
