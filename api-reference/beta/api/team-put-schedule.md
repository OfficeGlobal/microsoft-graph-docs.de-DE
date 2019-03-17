---
title: Erstellen oder Ersetzen eines Zeitplans
description: Erstellen oder Ersetzen eines **Schedule** -Objekts.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ddae7a348d4150e8ef36974fecfe6b2c276b7f1d
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657483"
---
# <a name="create-or-replace-schedule"></a><span data-ttu-id="d8140-103">Erstellen oder Ersetzen eines Zeitplans</span><span class="sxs-lookup"><span data-stu-id="d8140-103">Create or replace schedule</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8140-104">Erstellen oder Ersetzen eines [Schedule](../resources/schedule.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="d8140-104">Create or replace a [schedule](../resources/schedule.md) object.</span></span>

<span data-ttu-id="d8140-105">Der Zeit Planerstellungsprozess entspricht der [API-Richtlinie für ressourcenbasierte Vorgänge mit langer Ausführungszeit (relo)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span><span class="sxs-lookup"><span data-stu-id="d8140-105">The schedule creation process conforms to the [One API guideline for resource based long running operations (RELO)](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo).</span></span>
<span data-ttu-id="d8140-106">Wenn Clients die PUT-Methode verwenden, wird der Zeitplan durch den Vorgang ersetzt, wenn der Zeitplan vorgesehen ist. Andernfalls startet der Vorgang den Zeitplan für die bereitstellen im Hintergrund.</span><span class="sxs-lookup"><span data-stu-id="d8140-106">When clients use the PUT method, if the schedule is provisioned, the operation replaces the schedule; otherwise, the operation starts the schedule provisioning process in the background.</span></span>

<span data-ttu-id="d8140-107">Während der Terminplanung können Clients die [Get-Methode](schedule-get.md) verwenden, um den Zeitplan abzurufen und die `provisionStatus` Eigenschaft für den aktuellen Status der proaktivierung zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="d8140-107">During schedule provisioning, clients can use the [GET method](schedule-get.md) to get the schedule and look at the `provisionStatus` property for the current state of the provisioning.</span></span> <span data-ttu-id="d8140-108">Wenn die Einrichtung fehlgeschlagen ist, können Clients zusätzliche Informationen von der `provisionStatusCode` -Eigenschaft abrufen.</span><span class="sxs-lookup"><span data-stu-id="d8140-108">If the provisioning failed, clients can get additional information from the `provisionStatusCode` property.</span></span>

<span data-ttu-id="d8140-109">Clients können auch die Konfiguration des Zeitplans überprüfen.</span><span class="sxs-lookup"><span data-stu-id="d8140-109">Clients can also inspect the configuration of the schedule.</span></span>


## <a name="permissions"></a><span data-ttu-id="d8140-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d8140-110">Permissions</span></span>

<span data-ttu-id="d8140-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8140-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8140-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d8140-113">Permission type</span></span>      | <span data-ttu-id="d8140-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d8140-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8140-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d8140-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d8140-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8140-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8140-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d8140-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8140-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d8140-118">Not supported.</span></span>    |
|<span data-ttu-id="d8140-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d8140-119">Application</span></span> | <span data-ttu-id="d8140-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d8140-120">Not supported.</span></span> |

> <span data-ttu-id="d8140-121">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="d8140-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d8140-122">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="d8140-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d8140-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d8140-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule
```

## <a name="request-headers"></a><span data-ttu-id="d8140-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d8140-124">Request headers</span></span>

| <span data-ttu-id="d8140-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d8140-125">Header</span></span>       | <span data-ttu-id="d8140-126">Wert</span><span class="sxs-lookup"><span data-stu-id="d8140-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d8140-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8140-127">Authorization</span></span>  | <span data-ttu-id="d8140-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d8140-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d8140-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8140-130">Content-Type</span></span>  | <span data-ttu-id="d8140-131">application/json</span><span class="sxs-lookup"><span data-stu-id="d8140-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d8140-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d8140-132">Request body</span></span>

<span data-ttu-id="d8140-133">Geben Sie im Anforderungstext eine JSON-Darstellung eines [Schedule](../resources/schedule.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="d8140-133">In the request body, supply a JSON representation of a [schedule](../resources/schedule.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d8140-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="d8140-134">Response</span></span>

<span data-ttu-id="d8140-135">Bei erfolgreicher Ausführung gibt diese Methode den `200 OK` Antwortcode und ein [Schedule](../resources/schedule.md) -Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="d8140-135">If successful, this method returns a `200 OK` response code and a [schedule](../resources/schedule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8140-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d8140-136">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d8140-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d8140-137">Request</span></span>

<span data-ttu-id="d8140-138">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d8140-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "team-put-schedule"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule
Content-type: application/json

{
  "enabled": true,
  "timeZone": "America/Chicago"
}
```

#### <a name="response"></a><span data-ttu-id="d8140-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="d8140-139">Response</span></span>

<span data-ttu-id="d8140-140">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d8140-140">The following is an example of the response.</span></span> 

><span data-ttu-id="d8140-p106">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="d8140-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Creates or replaces the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/team-put-schedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
