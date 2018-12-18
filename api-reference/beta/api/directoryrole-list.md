---
title: directoryRoles auflisten
description: Mit dieser API können Sie alle Verzeichnisrollen abrufen, die in einem Mandanten aktiviert sind.
author: lleonard-msft
ms.openlocfilehash: 102360728e31e7fbec10c165ab026432a5b71585
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350743"
---
# <a name="list-directoryroles"></a><span data-ttu-id="0028a-103">directoryRoles auflisten</span><span class="sxs-lookup"><span data-stu-id="0028a-103">List directoryRoles</span></span>

> <span data-ttu-id="0028a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0028a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0028a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0028a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0028a-106">Mit dieser API können Sie alle Verzeichnisrollen abrufen, die in einem Mandanten aktiviert sind.</span><span class="sxs-lookup"><span data-stu-id="0028a-106">List the directory roles that are activated in the tenant.</span></span>
## <a name="permissions"></a><span data-ttu-id="0028a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0028a-107">Permissions</span></span>
<span data-ttu-id="0028a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0028a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0028a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0028a-110">Permission type</span></span>      | <span data-ttu-id="0028a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0028a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0028a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0028a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0028a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0028a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0028a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0028a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0028a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0028a-115">Not supported.</span></span>    |
|<span data-ttu-id="0028a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0028a-116">Application</span></span> | <span data-ttu-id="0028a-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0028a-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0028a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0028a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0028a-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="0028a-119">Optional query parameters</span></span>
<span data-ttu-id="0028a-120">Die [OData-Abfrageparameter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) zur Anpassung der Antwort werden von dieser Methode **nicht** unterstützt (d. h. „$filter“ wird nicht unterstützt).</span><span class="sxs-lookup"><span data-stu-id="0028a-120">This method does **not** support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0028a-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0028a-121">Request headers</span></span>
| <span data-ttu-id="0028a-122">Name</span><span class="sxs-lookup"><span data-stu-id="0028a-122">Name</span></span>       | <span data-ttu-id="0028a-123">Typ</span><span class="sxs-lookup"><span data-stu-id="0028a-123">Type</span></span> | <span data-ttu-id="0028a-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0028a-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0028a-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0028a-125">Authorization</span></span>  | <span data-ttu-id="0028a-126">string</span><span class="sxs-lookup"><span data-stu-id="0028a-126">string</span></span>  | <span data-ttu-id="0028a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0028a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0028a-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0028a-129">Request body</span></span>
<span data-ttu-id="0028a-130">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0028a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0028a-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="0028a-131">Response</span></span>

<span data-ttu-id="0028a-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [directoryRole](../resources/directoryrole.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0028a-132">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/directoryrole.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0028a-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0028a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0028a-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0028a-134">Request</span></span>
<span data-ttu-id="0028a-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0028a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directoryroles"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles
```
##### <a name="response"></a><span data-ttu-id="0028a-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="0028a-136">Response</span></span>
<span data-ttu-id="0028a-p104">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0028a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
