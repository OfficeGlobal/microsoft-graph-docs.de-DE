---
title: Abrufen der Teilnehmer
description: Rufen Sie die Eigenschaften und die Beziehungen eines **Teilnehmers** -Objekts ab.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: bdcf52f844ea000458d35aa211e7c32a5c6566e5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837695"
---
# <a name="get-participant"></a><span data-ttu-id="4a787-103">Abrufen der Teilnehmer</span><span class="sxs-lookup"><span data-stu-id="4a787-103">Get participant</span></span>

> <span data-ttu-id="4a787-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4a787-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a787-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4a787-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4a787-106">Rufen Sie die Eigenschaften und die Beziehungen eines **Teilnehmers** -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="4a787-106">Retrieve the properties and relationships of a **participant** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a787-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4a787-107">Permissions</span></span>
<span data-ttu-id="4a787-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a787-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4a787-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4a787-110">Permission type</span></span> | <span data-ttu-id="4a787-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4a787-111">Permissions (from least to most privileged)</span></span> |
| :-------------- | :------------------------------------------ |
| <span data-ttu-id="4a787-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4a787-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="4a787-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a787-113">Not Supported</span></span>        |
| <span data-ttu-id="4a787-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4a787-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a787-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4a787-115">Not Supported</span></span>        |
| <span data-ttu-id="4a787-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4a787-116">Application</span></span>     | <span data-ttu-id="4a787-117">Keine</span><span class="sxs-lookup"><span data-stu-id="4a787-117">None</span></span>                                        |

## <a name="http-request"></a><span data-ttu-id="4a787-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a787-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /app/calls/{id}/participants/{id}
GET /applications/{id}/calls/{id}/participants/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4a787-119">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="4a787-119">Optional query parameters</span></span>
<span data-ttu-id="4a787-120">Diese Methode unterstützt die [OData-Abfrage-Parameter](/graph/query-parameters) , mit denen die Antwort anpassen.</span><span class="sxs-lookup"><span data-stu-id="4a787-120">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4a787-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4a787-121">Request headers</span></span>
| <span data-ttu-id="4a787-122">Name</span><span class="sxs-lookup"><span data-stu-id="4a787-122">Name</span></span>          | <span data-ttu-id="4a787-123">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a787-123">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4a787-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a787-124">Authorization</span></span> | <span data-ttu-id="4a787-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4a787-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a787-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4a787-127">Request body</span></span>
<span data-ttu-id="4a787-128">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="4a787-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a787-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a787-129">Response</span></span>
<span data-ttu-id="4a787-130">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und eines [Teilnehmers](../resources/participant.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="4a787-130">If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a787-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4a787-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4a787-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4a787-132">Request</span></span>
<span data-ttu-id="4a787-133">Das folgende Beispiel zeigt die Antwort.</span><span class="sxs-lookup"><span data-stu-id="4a787-133">The following example shows the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get-participant"
}-->
```http
GET https://graph.microsoft.com/beta/app/calls/{id}/participants/{id}
```

##### <a name="response"></a><span data-ttu-id="4a787-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4a787-134">Response</span></span>

> <span data-ttu-id="4a787-p104">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="4a787-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Get participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
