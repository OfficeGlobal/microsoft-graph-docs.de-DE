---
title: Zeitplan abrufen
description: Ruft die Eigenschaften und Beziehungen eines **Schedule** -Objekts ab.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 84abbad582d346c106c751030b07c6337c939f48
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657588"
---
# <a name="get-schedule"></a><span data-ttu-id="175d2-103">Zeitplan abrufen</span><span class="sxs-lookup"><span data-stu-id="175d2-103">Get schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="175d2-104">Ruft die Eigenschaften und Beziehungen eines [Schedule](../resources/schedule.md) -Objekts ab.</span><span class="sxs-lookup"><span data-stu-id="175d2-104">Retrieve the properties and relationships of a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="175d2-105">Der Zeit Planerstellungsprozess entspricht der [API-Richtlinie für ressourcenbasierte Vorgänge mit langer Ausführungszeit (relo)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="175d2-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="175d2-106">Wenn die [Put-Methode](team-put-schedule.md)von Clients verwendet wird, wird der Zeitplan bei der Ausführung des Zeitplans aktualisiert. Andernfalls startet der Vorgang den Zeitplan für die bereitstellen im Hintergrund.</span><span class="sxs-lookup"><span data-stu-id="175d2-106">When clients use the [PUT method](team-put-schedule.md), if the schedule is provisioned, the operation updates the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="175d2-107">Während der Terminplanung können Clients die GET-Methode verwenden, um den Zeitplan abzurufen und die `provisionStatus` Eigenschaft für den aktuellen Status der proaktivierung zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="175d2-107">During schedule provisioning, clients can use the GET method to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="175d2-108">Wenn die Einrichtung fehlgeschlagen ist, können Clients zusätzliche Informationen von der `provisionStatusCode` -Eigenschaft abrufen.</span><span class="sxs-lookup"><span data-stu-id="175d2-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="175d2-109">Clients können auch die Konfiguration des Zeitplans überprüfen.</span><span class="sxs-lookup"><span data-stu-id="175d2-109">Clients can also inspect the configuration of the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="175d2-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="175d2-110">Permissions</span></span>

<span data-ttu-id="175d2-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="175d2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="175d2-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="175d2-113">Permission type</span></span>      | <span data-ttu-id="175d2-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="175d2-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="175d2-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="175d2-115">Delegated (work or school account)</span></span> | <span data-ttu-id="175d2-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="175d2-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="175d2-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="175d2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="175d2-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="175d2-118">Not supported.</span></span>    |
|<span data-ttu-id="175d2-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="175d2-119">Application</span></span> | <span data-ttu-id="175d2-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="175d2-120">Not supported.</span></span> |

> <span data-ttu-id="175d2-121">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="175d2-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="175d2-122">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="175d2-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="175d2-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="175d2-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="175d2-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="175d2-124">Request headers</span></span>

| <span data-ttu-id="175d2-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="175d2-125">Header</span></span>       | <span data-ttu-id="175d2-126">Wert</span><span class="sxs-lookup"><span data-stu-id="175d2-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="175d2-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="175d2-127">Authorization</span></span>  | <span data-ttu-id="175d2-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="175d2-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="175d2-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="175d2-130">Content-Type</span></span>  | <span data-ttu-id="175d2-131">application/json</span><span class="sxs-lookup"><span data-stu-id="175d2-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="175d2-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="175d2-132">Request body</span></span>
<span data-ttu-id="175d2-133">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="175d2-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="175d2-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="175d2-134">Response</span></span>

<span data-ttu-id="175d2-135">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [Schedule](../resources/schedule.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="175d2-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="175d2-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="175d2-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="175d2-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="175d2-137">Request</span></span>

<span data-ttu-id="175d2-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="175d2-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule
```

#### <a name="response"></a><span data-ttu-id="175d2-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="175d2-139">Response</span></span>

<span data-ttu-id="175d2-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="175d2-140">The following is an example of the response.</span></span> 

><span data-ttu-id="175d2-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="175d2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
