---
title: registeredDevices auflisten
description: Mit dieser API können Sie eine Liste aller registrierten Geräte eines Benutzers abrufen.
localization_priority: Normal
ms.openlocfilehash: 2447a58e89fe6c94ab5b3cf6d23b2621f757709c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866367"
---
# <a name="list-registereddevices"></a><span data-ttu-id="c728d-103">registeredDevices auflisten</span><span class="sxs-lookup"><span data-stu-id="c728d-103">List registeredDevices</span></span>

> <span data-ttu-id="c728d-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c728d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c728d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c728d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c728d-106">Mit dieser API können Sie eine Liste aller registrierten Geräte eines Benutzers abrufen.</span><span class="sxs-lookup"><span data-stu-id="c728d-106">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="c728d-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c728d-107">Permissions</span></span>
<span data-ttu-id="c728d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c728d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c728d-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c728d-110">Permission type</span></span>      | <span data-ttu-id="c728d-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c728d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c728d-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c728d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c728d-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c728d-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c728d-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c728d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c728d-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c728d-115">Not supported.</span></span>    |
|<span data-ttu-id="c728d-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c728d-116">Application</span></span> | <span data-ttu-id="c728d-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c728d-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c728d-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c728d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c728d-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="c728d-119">Optional query parameters</span></span>
<span data-ttu-id="c728d-120">Diese Methode unterstützt die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="c728d-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c728d-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c728d-121">Request headers</span></span>
| <span data-ttu-id="c728d-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c728d-122">Header</span></span>       | <span data-ttu-id="c728d-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c728d-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c728d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c728d-124">Authorization</span></span>  | <span data-ttu-id="c728d-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c728d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c728d-127">Annehmen</span><span class="sxs-lookup"><span data-stu-id="c728d-127">Accept</span></span>  | <span data-ttu-id="c728d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c728d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c728d-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c728d-129">Request body</span></span>
<span data-ttu-id="c728d-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="c728d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c728d-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c728d-131">Response</span></span>

<span data-ttu-id="c728d-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryObject](../resources/directoryobject.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c728d-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c728d-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c728d-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c728d-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c728d-134">Request</span></span>
<span data-ttu-id="c728d-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c728d-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```http
GET https://graph.microsoft.com/beta/me/registeredDevices
```
##### <a name="response"></a><span data-ttu-id="c728d-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c728d-136">Response</span></span>
<span data-ttu-id="c728d-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c728d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
