---
title: Gruppe abrufen
description: Abrufen der Office 365-**Gruppe**, die dieser **educationClass** entspricht.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: d467e36afe09ee37b51afcf25ed8f1917ed6ab16
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931699"
---
# <a name="get-group"></a><span data-ttu-id="4d12e-103">Gruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="4d12e-103">Get group</span></span>

<span data-ttu-id="4d12e-104">Abrufen der Office 365-**Gruppe**, die dieser **educationClass** entspricht.</span><span class="sxs-lookup"><span data-stu-id="4d12e-104">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="4d12e-105">**Hinweis:** Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Schulen.</span><span class="sxs-lookup"><span data-stu-id="4d12e-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="4d12e-106">Verwenden Sie in diesem Fall die Ressource `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="4d12e-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d12e-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4d12e-107">Permissions</span></span>
<span data-ttu-id="4d12e-108">Zum Aufrufen dieser API ist eine Kombination von Berechtigungen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d12e-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="4d12e-109">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d12e-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d12e-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4d12e-110">Permission type</span></span>      | <span data-ttu-id="4d12e-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4d12e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d12e-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4d12e-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="4d12e-113">Eine von EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write sowie Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d12e-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="4d12e-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4d12e-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4d12e-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4d12e-115">Not supported.</span></span>  |
|<span data-ttu-id="4d12e-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4d12e-116">Application</span></span> | <span data-ttu-id="4d12e-117">EduRoster.Read.All, EduRoster.ReadWrite.All und Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d12e-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="4d12e-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d12e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="4d12e-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4d12e-119">Request headers</span></span>
| <span data-ttu-id="4d12e-120">Header</span><span class="sxs-lookup"><span data-stu-id="4d12e-120">Header</span></span>       | <span data-ttu-id="4d12e-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4d12e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4d12e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d12e-122">Authorization</span></span>  | <span data-ttu-id="4d12e-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4d12e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4d12e-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4d12e-125">Request body</span></span>
<span data-ttu-id="4d12e-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4d12e-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4d12e-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d12e-127">Response</span></span>
<span data-ttu-id="4d12e-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4d12e-128">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d12e-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4d12e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d12e-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4d12e-130">Request</span></span>
<span data-ttu-id="4d12e-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4d12e-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/group
```
##### <a name="response"></a><span data-ttu-id="4d12e-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="4d12e-132">Response</span></span>
<span data-ttu-id="4d12e-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4d12e-133">The following is an example of the response.</span></span> 

><span data-ttu-id="4d12e-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4d12e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user",
  "isCollection": false
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: xxx

{
  "id": "id-value",
  "description": "description-value",
  "displayName": "displayName-value",
  "groupTypes": [
    "groupTypes-value"
  ],
  "mail": "mail-value",
  "mailEnabled": true,
  "mailNickname": "mailNickname-value",
  "onPremisesLastSyncDateTime": "onPremisesLastSyncDateTime-value",
  "onPremisesSecurityIdentifier": "onPremisesSecurityIdentifier-value",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": [
    "proxyAddresses-value"
   ],
   "securityEnabled": true,
   "visibility": "visibility-value"
}
```

<!-- uuid: 0087D9B3-1418-4C87-91C9-A18C6D93706B
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
