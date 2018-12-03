---
title: Archiv-team
description: 'Archivieren Sie das angegebene Team. '
ms.openlocfilehash: 70a7015229784ffda78dc9020a0f847d68027d22
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058416"
---
# <a name="archive-team"></a><span data-ttu-id="7b0db-103">Archiv-team</span><span class="sxs-lookup"><span data-stu-id="7b0db-103">Archive team</span></span>

> <span data-ttu-id="7b0db-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7b0db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b0db-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7b0db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b0db-106">Archivieren Sie das angegebene [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7b0db-106">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="7b0db-107">Wenn ein Team archiviert wird, können Benutzer nicht mehr senden wie Nachrichten auf einem beliebigen Kanal im Team, bearbeiten das Team Name, Beschreibung oder andere Einstellungen oder im Allgemeinen die meisten Änderungen an das Team vornehmen.</span><span class="sxs-lookup"><span data-stu-id="7b0db-107">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="7b0db-108">Mitgliedschaftsänderungen an das Team weiterhin zugelassen werden.</span><span class="sxs-lookup"><span data-stu-id="7b0db-108">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="7b0db-109">Archivierung ist ein asynchroner Vorgang.</span><span class="sxs-lookup"><span data-stu-id="7b0db-109">Archiving is an async operation.</span></span> <span data-ttu-id="7b0db-110">Nach Abschluss des Vorgangs Async erfolgreich, die nach einer Antwort vom diese API auftreten können, ist ein Team archiviert.</span><span class="sxs-lookup"><span data-stu-id="7b0db-110">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="7b0db-111">Zum Archivieren von Team benötigen die Teams und der [Gruppe](../resources/group.md) Besitzer.</span><span class="sxs-lookup"><span data-stu-id="7b0db-111">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="7b0db-112">Um ein Team aus den archivierten Zustand wiederherzustellen, verwenden Sie die API zu [Öffnen](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="7b0db-112">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7b0db-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7b0db-113">Permissions</span></span>
<span data-ttu-id="7b0db-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7b0db-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7b0db-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7b0db-116">Permission type</span></span>      | <span data-ttu-id="7b0db-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7b0db-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7b0db-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7b0db-118">Delegated (work or school account)</span></span> | <span data-ttu-id="7b0db-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b0db-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7b0db-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7b0db-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7b0db-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7b0db-121">Not supported.</span></span>    |
|<span data-ttu-id="7b0db-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7b0db-122">Application</span></span> | <span data-ttu-id="7b0db-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7b0db-123">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="7b0db-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b0db-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="7b0db-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7b0db-125">Request headers</span></span>
| <span data-ttu-id="7b0db-126">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7b0db-126">Header</span></span>       | <span data-ttu-id="7b0db-127">Wert</span><span class="sxs-lookup"><span data-stu-id="7b0db-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7b0db-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b0db-128">Authorization</span></span>  | <span data-ttu-id="7b0db-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7b0db-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7b0db-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7b0db-131">Request body</span></span>
<span data-ttu-id="7b0db-132">In der Anforderung kann _optional_ umfassen die `shouldSetSpoSiteReadOnlyForMembers` Parameter in einem JSON body, wie folgt.</span><span class="sxs-lookup"><span data-stu-id="7b0db-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="7b0db-133">Dieser optionale Parameter definiert, ob Festlegen von Berechtigungen für Teammitglieder den Schreibschutz für die Sharepoint Online-Website mit dem Team verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="7b0db-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="7b0db-134">Festlegen der Steuerelementvorlage auf False oder im Textkörper auslassen führt vollständig in diesem Schritt wird übersprungen.</span><span class="sxs-lookup"><span data-stu-id="7b0db-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="7b0db-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b0db-135">Response</span></span>

<span data-ttu-id="7b0db-136">Wenn die Archivierung erfolgreich gestartet wurde, gibt diese Methode einen `202 Accepted` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="7b0db-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="7b0db-137">Die Antwort enthält außerdem eine `Location` Kopf, der den Speicherort der die [TeamsAsyncOperation](../resources/teamsasyncoperation.md) enthält, die zum Behandeln des Teams Archivierung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="7b0db-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="7b0db-138">Überprüfen Sie den Status des Vorgangs Archivierung, indem er eine GET-Anforderung an diesen Speicherort.</span><span class="sxs-lookup"><span data-stu-id="7b0db-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="7b0db-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7b0db-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7b0db-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7b0db-140">Request</span></span>
<span data-ttu-id="7b0db-141">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7b0db-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="7b0db-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="7b0db-142">Response</span></span>
<span data-ttu-id="7b0db-143">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="7b0db-143">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```
<!-- uuid: e848414b-4669-4484-ac36-1504c58a3fb8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Archive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
