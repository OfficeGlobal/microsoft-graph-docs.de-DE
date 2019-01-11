---
title: directoryRoles auflisten
description: Mit dieser API können Sie alle Verzeichnisrollen abrufen, die in einem Mandanten aktiviert sind.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 03f81de99fadc8beb96f7f07361b6152689b680a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838122"
---
# <a name="list-directoryroles"></a><span data-ttu-id="a11cb-103">directoryRoles auflisten</span><span class="sxs-lookup"><span data-stu-id="a11cb-103">List directoryRoles</span></span>

> <span data-ttu-id="a11cb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a11cb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a11cb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a11cb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a11cb-106">Mit dieser API können Sie alle Verzeichnisrollen abrufen, die in einem Mandanten aktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="a11cb-106">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="a11cb-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a11cb-107">Permissions</span></span>
<span data-ttu-id="a11cb-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a11cb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a11cb-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a11cb-110">Permission type</span></span>      | <span data-ttu-id="a11cb-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a11cb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a11cb-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a11cb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a11cb-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a11cb-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a11cb-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a11cb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a11cb-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a11cb-115">Not supported.</span></span>    |
|<span data-ttu-id="a11cb-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a11cb-116">Application</span></span> | <span data-ttu-id="a11cb-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a11cb-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a11cb-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a11cb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a11cb-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="a11cb-119">Optional query parameters</span></span>
<span data-ttu-id="a11cb-120">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort werden von dieser Methode **nicht** unterstützt (d. h. „$filter“ wird nicht unterstützt).</span><span class="sxs-lookup"><span data-stu-id="a11cb-120">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a11cb-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a11cb-121">Request headers</span></span>
| <span data-ttu-id="a11cb-122">Name</span><span class="sxs-lookup"><span data-stu-id="a11cb-122">Name</span></span>       | <span data-ttu-id="a11cb-123">Typ</span><span class="sxs-lookup"><span data-stu-id="a11cb-123">Type</span></span> | <span data-ttu-id="a11cb-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a11cb-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a11cb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a11cb-125">Authorization</span></span>  | <span data-ttu-id="a11cb-126">string</span><span class="sxs-lookup"><span data-stu-id="a11cb-126">string</span></span>  | <span data-ttu-id="a11cb-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a11cb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a11cb-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a11cb-129">Request body</span></span>
<span data-ttu-id="a11cb-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="a11cb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a11cb-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a11cb-131">Response</span></span>

<span data-ttu-id="a11cb-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryRole](../resources/directoryrole.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a11cb-132">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a11cb-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a11cb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a11cb-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a11cb-134">Request</span></span>
<span data-ttu-id="a11cb-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="a11cb-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles
```
##### <a name="response"></a><span data-ttu-id="a11cb-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a11cb-136">Response</span></span>
<span data-ttu-id="a11cb-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a11cb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 187

{
  "value": [
    {
      "description": "description-value",
      "displayName": "displayName-value",
      "roleTemplateId": "roleTemplateId-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List directoryRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
