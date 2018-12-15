---
title: Abrufen von dataPolicyOperation
description: Rufen Sie die Eigenschaften des DataPolicyOperation-Objekts ab.
ms.openlocfilehash: 8e5e4b6c10e086769fadcdd575cfd71339a5dcde
ms.sourcegitcommit: f3d479edf03935d0edbbc7668a65f7cde2a56c92
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2018
ms.locfileid: "27284112"
---
# <a name="get-datapolicyoperation"></a><span data-ttu-id="38759-103">Abrufen von dataPolicyOperation</span><span class="sxs-lookup"><span data-stu-id="38759-103">Get dataPolicyOperation</span></span>

<span data-ttu-id="38759-104">Rufen Sie die Eigenschaften eines **DataPolicyOperation** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="38759-104">Retrieve the properties of a **dataPolicyOperation** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="38759-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="38759-105">Permissions</span></span>
<span data-ttu-id="38759-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="38759-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38759-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="38759-108">Permission type</span></span>      | <span data-ttu-id="38759-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="38759-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38759-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="38759-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="38759-111">User.Export.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="38759-111">User.Export.All, User.Read.All</span></span>  |
|<span data-ttu-id="38759-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="38759-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="38759-113">Nicht zutreffend</span><span class="sxs-lookup"><span data-stu-id="38759-113">Not applicable</span></span>  |
|<span data-ttu-id="38759-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="38759-114">Application</span></span> | <span data-ttu-id="38759-115">User.Export.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="38759-115">User.Export.All, User.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="38759-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="38759-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /dataPolicyOperations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="38759-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="38759-117">Request headers</span></span>
| <span data-ttu-id="38759-118">Name</span><span class="sxs-lookup"><span data-stu-id="38759-118">Name</span></span>      |<span data-ttu-id="38759-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="38759-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="38759-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="38759-120">Authorization</span></span>  | <span data-ttu-id="38759-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="38759-121">Bearer {token}</span></span>|

## <a name="request-body"></a><span data-ttu-id="38759-122">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="38759-122">Request body</span></span>
<span data-ttu-id="38759-123">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="38759-123">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="38759-124">Antwort</span><span class="sxs-lookup"><span data-stu-id="38759-124">Response</span></span>
<span data-ttu-id="38759-125">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [DataPolicyOperation](../resources/datapolicyoperation.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="38759-125">If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38759-126">Beispiel</span><span class="sxs-lookup"><span data-stu-id="38759-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38759-127">Anforderung</span><span class="sxs-lookup"><span data-stu-id="38759-127">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}-->
```http
GET https://graph.microsoft.com/v1.0/dataPolicyOperations/{id}
```
##### <a name="response"></a><span data-ttu-id="38759-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="38759-128">Response</span></span>
><span data-ttu-id="38759-p102">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="38759-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
