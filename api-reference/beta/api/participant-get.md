---
title: Abrufen der Teilnehmer
description: Rufen Sie die Eigenschaften und die Beziehungen eines **Teilnehmers** -Objekts ab.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5b966b3fae9ea687fea22e01227e585d5d69d4cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507670"
---
# <a name="get-participant"></a><span data-ttu-id="4ab5d-103">Abrufen der Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="4ab5d-103">Get participant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4ab5d-104">Rufen Sie die Eigenschaften und die Beziehungen eines **Teilnehmers** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="4ab5d-104">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ab5d-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4ab5d-105">Permissions</span></span>
<span data-ttu-id="4ab5d-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ab5d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4ab5d-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4ab5d-108">Permission type</span></span> | <span data-ttu-id="4ab5d-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4ab5d-109">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="4ab5d-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4ab5d-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4ab5d-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ab5d-111">Not Supported</span></span>        |
| <span data-ttu-id="4ab5d-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4ab5d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ab5d-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ab5d-113">Not Supported</span></span>        |
| <span data-ttu-id="4ab5d-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ab5d-114">Application</span></span>     | <span data-ttu-id="4ab5d-115">Keine</span><span class="sxs-lookup"><span data-stu-id="4ab5d-115">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="4ab5d-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ab5d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /applications/{id}/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4ab5d-117">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4ab5d-117">Optional query parameters</span></span>
<span data-ttu-id="4ab5d-118">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="4ab5d-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4ab5d-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ab5d-119">Request headers</span></span>
| <span data-ttu-id="4ab5d-120">Name</span><span class="sxs-lookup"><span data-stu-id="4ab5d-120">Name</span></span>          | <span data-ttu-id="4ab5d-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ab5d-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4ab5d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ab5d-122">Authorization</span></span> | <span data-ttu-id="4ab5d-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4ab5d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ab5d-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ab5d-125">Request body</span></span>
<span data-ttu-id="4ab5d-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4ab5d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4ab5d-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ab5d-127">Response</span></span>
<span data-ttu-id="4ab5d-128">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [Teilnehmers](../resources/participant.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4ab5d-128">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ab5d-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ab5d-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4ab5d-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ab5d-130">Request</span></span>
<span data-ttu-id="4ab5d-131">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="4ab5d-131">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}
```

##### <a name="response"></a><span data-ttu-id="4ab5d-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ab5d-132">Response</span></span>

> <span data-ttu-id="4ab5d-p103">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4ab5d-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "info": {
    "identity": {
      "user": {
        "id": "550fae72-d251-43ec-868c-373732c2704f",
        "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
        "displayName": "Heidi Steen"
      }
    },
    "languageId": "languageId-value",
    "region": "region-value"
  },
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [
    {
      "sourceId": "1",
      "direction": "sendReceive",
      "label": "main-audio",
      "mediaType": "audio",
      "serverMuted": false
    }
  ],
  "metadata": "metadata-value",
  "recordingInfo": {
    "initiatedBy": {
      "identity": {
        "user": {
          "id": "550fae72-d251-43ec-868c-373732c2704f",
          "tenantId": "72f988bf-86f1-41af-91ab-2d7cd011db47",
          "displayName": "Heidi Steen"
        }
      },
      "languageId": "languageId-value",
      "region": "region-value"
    },
    "status": "recordingCapable"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/participant-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
