---
title: Abrufen von dataPolicyOperation
description: Rufen Sie die Eigenschaften des DataPolicyOperation-Objekts ab.
localization_priority: Normal
ms.openlocfilehash: a06b2b119683a75516b0d51f955565276249be41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860361"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="033d3-103">Abrufen von dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="033d3-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="033d3-104">Rufen Sie die Eigenschaften eines **DataPolicyOperation** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="033d3-104">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="033d3-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="033d3-105">Permissions</span></span>
<span data-ttu-id="033d3-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="033d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="033d3-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="033d3-108">Permission type</span></span>      | <span data-ttu-id="033d3-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="033d3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="033d3-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="033d3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="033d3-111">User.Export.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="033d3-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="033d3-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="033d3-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="033d3-113">Nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="033d3-113">Not applicable</span></span>  |
|<span data-ttu-id="033d3-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="033d3-114">Application</span></span> | <span data-ttu-id="033d3-115">User.Export.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="033d3-115">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="033d3-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="033d3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="033d3-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="033d3-117">Request headers</span></span>
| <span data-ttu-id="033d3-118">Name</span><span class="sxs-lookup"><span data-stu-id="033d3-118">Name</span></span>      |<span data-ttu-id="033d3-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="033d3-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="033d3-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="033d3-120">Authorization</span></span>  | <span data-ttu-id="033d3-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="033d3-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="033d3-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="033d3-122">Request body</span></span>
<span data-ttu-id="033d3-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="033d3-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="033d3-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="033d3-124">Response</span></span>
<span data-ttu-id="033d3-125">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [DataPolicyOperation](../resources/datapolicyoperation.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="033d3-125">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="033d3-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="033d3-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="033d3-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="033d3-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="033d3-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="033d3-128">Response</span></span>
><span data-ttu-id="033d3-p102">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="033d3-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "progress": "double-value"
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
