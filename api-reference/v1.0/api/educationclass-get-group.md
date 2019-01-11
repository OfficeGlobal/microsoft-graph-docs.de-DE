---
title: Gruppe abrufen
description: Abrufen der Office 365-**Gruppe**, die dieser **educationClass** entspricht.
localization_priority: Normal
ms.openlocfilehash: da7e179802739f39465cfb462c92c527ecac3d7c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825347"
---
# <a name="get-group"></a><span data-ttu-id="4abdf-103">Gruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="4abdf-103">Get group</span></span>

<span data-ttu-id="4abdf-104">Abrufen der Office 365-**Gruppe**, die dieser **educationClass** entspricht.</span><span class="sxs-lookup"><span data-stu-id="4abdf-104">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="4abdf-105">**Hinweis:** Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Schulen.</span><span class="sxs-lookup"><span data-stu-id="4abdf-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="4abdf-106">Verwenden Sie in diesem Fall die Ressource `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="4abdf-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="4abdf-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4abdf-107">Permissions</span></span>
<span data-ttu-id="4abdf-108">Zum Aufrufen dieser API ist eine Kombination von Berechtigungen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4abdf-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="4abdf-109">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4abdf-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4abdf-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4abdf-110">Permission type</span></span>      | <span data-ttu-id="4abdf-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4abdf-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4abdf-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4abdf-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="4abdf-113">Eine von EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write sowie Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4abdf-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="4abdf-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4abdf-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4abdf-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4abdf-115">Not supported.</span></span>  |
|<span data-ttu-id="4abdf-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4abdf-116">Application</span></span> | <span data-ttu-id="4abdf-117">EduRoster.Read.All, EduRoster.ReadWrite.All und Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4abdf-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="4abdf-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4abdf-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="4abdf-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4abdf-119">Request headers</span></span>
| <span data-ttu-id="4abdf-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4abdf-120">Header</span></span>       | <span data-ttu-id="4abdf-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4abdf-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4abdf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4abdf-122">Authorization</span></span>  | <span data-ttu-id="4abdf-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4abdf-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4abdf-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4abdf-125">Request body</span></span>
<span data-ttu-id="4abdf-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4abdf-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4abdf-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="4abdf-127">Response</span></span>
<span data-ttu-id="4abdf-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4abdf-128">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4abdf-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4abdf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4abdf-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4abdf-130">Request</span></span>
<span data-ttu-id="4abdf-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4abdf-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/{class-id}/group
```
##### <a name="response"></a><span data-ttu-id="4abdf-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="4abdf-132">Response</span></span>
<span data-ttu-id="4abdf-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="4abdf-133">The following is an example of the response.</span></span> 

><span data-ttu-id="4abdf-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4abdf-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
