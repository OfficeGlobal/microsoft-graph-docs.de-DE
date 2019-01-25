---
title: Gruppe abrufen
description: Abrufen der Office 365-**Gruppe**, die dieser **educationClass** entspricht.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: bd5cac6b952f58c27a3f801db8679dfc48b16de3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518884"
---
# <a name="get-group"></a><span data-ttu-id="0e91c-103">Gruppe abrufen</span><span class="sxs-lookup"><span data-stu-id="0e91c-103">Get group</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e91c-104">Abrufen der Office 365-**Gruppe**, die dieser **educationClass** entspricht.</span><span class="sxs-lookup"><span data-stu-id="0e91c-104">Retrieve the Office 365 **group** that corresponds to this **educationClass**.</span></span>

><span data-ttu-id="0e91c-105">**Hinweis:** Wenn das delegierte Token verwendet wird, erhalten Mitglieder nur Informationen zu ihren eigenen Schulen.</span><span class="sxs-lookup"><span data-stu-id="0e91c-105">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="0e91c-106">Verwenden Sie in diesem Fall die Ressource `...beta/education/me/schools`.</span><span class="sxs-lookup"><span data-stu-id="0e91c-106">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e91c-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0e91c-107">Permissions</span></span>
<span data-ttu-id="0e91c-108">Zum Aufrufen dieser API ist eine Kombination von Berechtigungen erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e91c-108">A combination of permissions is required to call this API.</span></span> <span data-ttu-id="0e91c-109">Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie unter [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e91c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e91c-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e91c-110">Permission type</span></span>      | <span data-ttu-id="0e91c-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e91c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e91c-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e91c-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="0e91c-113">Eine von EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write sowie Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e91c-113">One from EduRoster.ReadBasic, EduRoster.Read, EduRoster.Write plus Directory.Read.All</span></span>|
|<span data-ttu-id="0e91c-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e91c-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0e91c-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e91c-115">Not supported.</span></span>  |
|<span data-ttu-id="0e91c-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e91c-116">Application</span></span> | <span data-ttu-id="0e91c-117">EduRoster.Read.All, EduRoster.ReadWrite.All und Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e91c-117">EduRoster.Read.All, EduRoster.ReadWrite.All plus Directory.Read.All</span></span>| 

## <a name="http-request"></a><span data-ttu-id="0e91c-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e91c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/group
```
## <a name="request-headers"></a><span data-ttu-id="0e91c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e91c-119">Request headers</span></span>
| <span data-ttu-id="0e91c-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="0e91c-120">Header</span></span>       | <span data-ttu-id="0e91c-121">Wert</span><span class="sxs-lookup"><span data-stu-id="0e91c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0e91c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e91c-122">Authorization</span></span>  | <span data-ttu-id="0e91c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e91c-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e91c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e91c-125">Request body</span></span>
<span data-ttu-id="0e91c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="0e91c-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0e91c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e91c-127">Response</span></span>
<span data-ttu-id="0e91c-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e91c-128">If successful, this method returns a `200 OK` response code and a [group](../resources/group.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0e91c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e91c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e91c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e91c-130">Request</span></span>
<span data-ttu-id="0e91c-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0e91c-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/2961761D-8094-4183-A9F6-8E36E966C7D9/group
```
##### <a name="response"></a><span data-ttu-id="0e91c-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e91c-132">Response</span></span>
<span data-ttu-id="0e91c-133">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0e91c-133">The following is an example of the response.</span></span> 

><span data-ttu-id="0e91c-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="0e91c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-get-group.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
