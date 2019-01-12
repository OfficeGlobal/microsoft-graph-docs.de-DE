---
title: Abrufen von dataPolicyOperation
description: Rufen Sie die Eigenschaften des DataPolicyOperation-Objekts ab.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5fff5d25ed83c6cfdf889c364630399acdeecb9e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951061"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="4a04b-103">Abrufen von dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="4a04b-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="4a04b-104">Rufen Sie die Eigenschaften des DataPolicyOperation-Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="4a04b-104">Retrieve the properties of the dataPolicyOperation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a04b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4a04b-105">Permissions</span></span>
<span data-ttu-id="4a04b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a04b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a04b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a04b-108">Permission type</span></span>      | <span data-ttu-id="4a04b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a04b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a04b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a04b-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="4a04b-111">User.Export.All und User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a04b-111">User.Export.All and User.Read.All</span></span>  |
|<span data-ttu-id="4a04b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a04b-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4a04b-113">Nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="4a04b-113">Not applicable</span></span>  |
|<span data-ttu-id="4a04b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a04b-114">Application</span></span> | <span data-ttu-id="4a04b-115">User.Export.All und User.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a04b-115">User.Export.All and User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4a04b-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a04b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4a04b-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a04b-117">Request headers</span></span>
| <span data-ttu-id="4a04b-118">Name</span><span class="sxs-lookup"><span data-stu-id="4a04b-118">Name</span></span>      |<span data-ttu-id="4a04b-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a04b-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4a04b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a04b-120">Authorization</span></span>  | <span data-ttu-id="4a04b-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="4a04b-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a04b-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a04b-122">Request body</span></span>
<span data-ttu-id="4a04b-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4a04b-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4a04b-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a04b-124">Response</span></span>
<span data-ttu-id="4a04b-125">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortobjekt Code und [DataPolicyOperation](../resources/datapolicyoperation.md) im Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4a04b-125">If successful, this method returns a `200 OK` response code and [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4a04b-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a04b-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a04b-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a04b-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/beta/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="4a04b-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a04b-128">Response</span></span>
<span data-ttu-id="4a04b-p102">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4a04b-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dataPolicyOperation"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 212

{
  "completedDateTime": "datetime-value",
  "id": "id-value",
  "status": "status-value",
  "storageLocation": "storageLocation-value",
  "userId": "userId-value",
  "submittedDateTime": "datetime-value",
  "progress": "progress-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get dataPolicyOperation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
