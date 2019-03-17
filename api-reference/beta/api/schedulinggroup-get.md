---
title: Get schedulinggroup
description: Rufen Sie die Eigenschaften und Beziehungen einer [schedulinggroup](../resources/schedulinggroup.md) anhand der ID ab.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 46131e90cac2a6f5a4e75409eefd6bbf2eda7888
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657574"
---
# <a name="get-schedulinggroup"></a><span data-ttu-id="8a62b-103">Get schedulinggroup</span><span class="sxs-lookup"><span data-stu-id="8a62b-103">Get schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a62b-104">Rufen Sie die Eigenschaften und Beziehungen einer [schedulinggroup](../resources/schedulinggroup.md) anhand der ID ab.</span><span class="sxs-lookup"><span data-stu-id="8a62b-104">Retrieve the properties and relationships of a [schedulingGroup](../resources/schedulinggroup.md) by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a62b-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8a62b-105">Permissions</span></span>

<span data-ttu-id="8a62b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a62b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a62b-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8a62b-108">Permission type</span></span>      | <span data-ttu-id="8a62b-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8a62b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a62b-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a62b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8a62b-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a62b-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a62b-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a62b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a62b-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a62b-113">Not supported.</span></span>    |
|<span data-ttu-id="8a62b-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a62b-114">Application</span></span> | <span data-ttu-id="8a62b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a62b-115">Not supported.</span></span> |

> <span data-ttu-id="8a62b-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="8a62b-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8a62b-117">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="8a62b-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8a62b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a62b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="8a62b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a62b-119">Request headers</span></span>

| <span data-ttu-id="8a62b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8a62b-120">Header</span></span>       | <span data-ttu-id="8a62b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8a62b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a62b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a62b-122">Authorization</span></span>  | <span data-ttu-id="8a62b-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a62b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8a62b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a62b-125">Content-Type</span></span>  | <span data-ttu-id="8a62b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a62b-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a62b-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8a62b-127">Request body</span></span>
<span data-ttu-id="8a62b-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="8a62b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8a62b-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a62b-129">Response</span></span>

<span data-ttu-id="8a62b-130">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [schedulinggroup](../resources/schedulinggroup.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="8a62b-130">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a62b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a62b-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8a62b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a62b-132">Request</span></span>

<span data-ttu-id="8a62b-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8a62b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-get-schedulinggroups"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

#### <a name="response"></a><span data-ttu-id="8a62b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a62b-134">Response</span></span>

<span data-ttu-id="8a62b-135">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="8a62b-135">The following is an example of the response.</span></span> 

><span data-ttu-id="8a62b-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="8a62b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a schedulingGroup by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-get-schedulinggroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
