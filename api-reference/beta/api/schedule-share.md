---
title: 'Zeitplan: Freigeben'
description: Teilen Sie einen Zeit Planzeitraum mit Schedule-Elementen.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: eaa2eae082c2b50f39b4a3ac2547ca5b0135381f
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657721"
---
# <a name="schedule-share"></a><span data-ttu-id="7910d-103">Zeitplan: Freigeben</span><span class="sxs-lookup"><span data-stu-id="7910d-103">schedule: share</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7910d-104">Teilen Sie einen Zeit [Plan](../resources/schedule.md) Zeitraum mit Schedule-Elementen.</span><span class="sxs-lookup"><span data-stu-id="7910d-104">Share a [schedule](../resources/schedule.md) time range with schedule members.</span></span>
<span data-ttu-id="7910d-105">Erstellen Sie die Auflistungen von [Shift](../resources/shift.md) -und [timeOff](../resources/timeoff.md) -Elementen im angegebenen Zeitintervall [](../resources/schedule.md) des Zeitplans, die von den angegebenen Teammitgliedern angezeigt werden, einschließlich Mitarbeiter und Manager.</span><span class="sxs-lookup"><span data-stu-id="7910d-105">Make the collections of [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) items in the specified time range of the [schedule](../resources/schedule.md) viewable by the specified team members, including employees and managers.</span></span>
<span data-ttu-id="7910d-106">Jede [Shift](../resources/shift.md) -und [timeOff](../resources/timeoff.md) -Instanz in einem [Zeitplan](../resources/schedule.md) unterstützt eine Entwurfsversion und eine freigegebene Version des Elements.</span><span class="sxs-lookup"><span data-stu-id="7910d-106">Each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in a [schedule](../resources/schedule.md) supports a draft version and a shared version of the item.</span></span> <span data-ttu-id="7910d-107">Die Entwurfsversion kann nur von Managern angezeigt werden, und die freigegebene Version kann von Mitarbeitern und Managern angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="7910d-107">The draft version is viewable by only managers, and the shared version is viewable by employees and managers.</span></span> <span data-ttu-id="7910d-108">Für jede [Shift](../resources/shift.md) -und [timeOff](../resources/timeoff.md) -Instanz im angegebenen Zeitintervall aktualisiert die Freigabe Aktion die freigegebene Version aus der Entwurfsversion, sodass Mitarbeiter neben Managern auch die aktuellen Informationen zu dem Element anzeigen können.</span><span class="sxs-lookup"><span data-stu-id="7910d-108">For each [shift](../resources/shift.md) and [timeOff](../resources/timeoff.md) instance in the specified time range, the share action updates the shared version from the draft version, so that in addition to managers, employees can also view the most current information about the item.</span></span> <span data-ttu-id="7910d-109">Der Parameter **notifyTeam** gibt weiter an, welche Mitarbeiter das Element anzeigen können.</span><span class="sxs-lookup"><span data-stu-id="7910d-109">The **notifyTeam** parameter further specifies which employees can view the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="7910d-110">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7910d-110">Permissions</span></span>

<span data-ttu-id="7910d-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7910d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7910d-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7910d-113">Permission type</span></span>      | <span data-ttu-id="7910d-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7910d-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7910d-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7910d-115">Delegated (work or school account)</span></span> | <span data-ttu-id="7910d-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7910d-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7910d-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7910d-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7910d-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7910d-118">Not supported.</span></span>    |
|<span data-ttu-id="7910d-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7910d-119">Application</span></span> | <span data-ttu-id="7910d-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7910d-120">Not supported.</span></span> |

> <span data-ttu-id="7910d-121">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="7910d-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7910d-122">Globale Administratoren können auf Gruppen zugreifen, von denen Sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="7910d-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7910d-123">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7910d-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/share
```

## <a name="request-headers"></a><span data-ttu-id="7910d-124">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7910d-124">Request headers</span></span>

| <span data-ttu-id="7910d-125">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7910d-125">Header</span></span>       | <span data-ttu-id="7910d-126">Wert</span><span class="sxs-lookup"><span data-stu-id="7910d-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7910d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="7910d-127">Authorization</span></span>  | <span data-ttu-id="7910d-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7910d-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7910d-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7910d-130">Content-Type</span></span>  | <span data-ttu-id="7910d-131">application/json</span><span class="sxs-lookup"><span data-stu-id="7910d-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7910d-132">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7910d-132">Request body</span></span>

<span data-ttu-id="7910d-133">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="7910d-133">In the request body, provide a JSON object with the following parameters.</span></span>

|<span data-ttu-id="7910d-134">Parameter</span><span class="sxs-lookup"><span data-stu-id="7910d-134">Parameter</span></span>                   |<span data-ttu-id="7910d-135">Typ</span><span class="sxs-lookup"><span data-stu-id="7910d-135">Type</span></span>           |<span data-ttu-id="7910d-136">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7910d-136">Description</span></span>  |
|-----------------------|-------------------|--------------|
| <span data-ttu-id="7910d-137">notifyTeam</span><span class="sxs-lookup"><span data-stu-id="7910d-137">notifyTeam</span></span>            |`Boolean`             |<span data-ttu-id="7910d-138">Gibt an, ob das gesamte Team eine sichtbare Benachrichtigung über diese Aktion erhalten soll, oder nur Mitarbeiter, denen eine Schicht zugewiesen wurde, die freigegeben wurde.</span><span class="sxs-lookup"><span data-stu-id="7910d-138">Indicates whether the entire team should get a visible notification of this action, or only employees that have a shift assigned to them that was shared.</span></span> <span data-ttu-id="7910d-139">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7910d-139">Required.</span></span>       |
| <span data-ttu-id="7910d-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7910d-140">startDateTime</span></span>         |`DateTimeOffset`   |<span data-ttu-id="7910d-141">Die Startzeit für die Freigabe von Schichten im Zeitplan.</span><span class="sxs-lookup"><span data-stu-id="7910d-141">The start time to share shifts on the schedule from.</span></span> <span data-ttu-id="7910d-142">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7910d-142">Required.</span></span>   |
| <span data-ttu-id="7910d-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7910d-143">endDateTime</span></span>           |`DateTimeOffset`   | <span data-ttu-id="7910d-144">Die Endzeit für die Freigabe von Schichten für den Zeitplan bis.</span><span class="sxs-lookup"><span data-stu-id="7910d-144">The end time to share shifts on the schedule until.</span></span>   |

## <a name="response"></a><span data-ttu-id="7910d-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="7910d-145">Response</span></span>

<span data-ttu-id="7910d-p107">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben. Im Antworttext wird nichts zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7910d-p107">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7910d-148">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7910d-148">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7910d-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7910d-149">Request</span></span>

<span data-ttu-id="7910d-150">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7910d-150">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-share"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/share
Content-type: application/json

{
  "notifyTeam": true,
  "startDateTime": "2018-10-08T00:00:00.000Z",
  "endDateTime": "2018-10-15T00:00:00.000Z"
}
```

#### <a name="response"></a><span data-ttu-id="7910d-151">Antwort</span><span class="sxs-lookup"><span data-stu-id="7910d-151">Response</span></span>

<span data-ttu-id="7910d-152">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7910d-152">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Shares a time-range of the schedule with the schedule members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-share.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
