---
title: Archiv-team
description: 'Archivieren Sie das angegebene Team. '
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: c7ac186eeb937b1dda0b1df4878260e61fe30b18
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016639"
---
# <a name="archive-team"></a><span data-ttu-id="45ee3-103">Archiv-team</span><span class="sxs-lookup"><span data-stu-id="45ee3-103">Archive team</span></span>



<span data-ttu-id="45ee3-104">Archivieren Sie das angegebene [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="45ee3-104">Archive the specified [team](../resources/team.md).</span></span> <span data-ttu-id="45ee3-105">Wenn ein Team archiviert wird, können Benutzer nicht mehr senden wie Nachrichten auf einem beliebigen Kanal im Team, bearbeiten das Team Name, Beschreibung oder andere Einstellungen oder im Allgemeinen die meisten Änderungen an das Team vornehmen.</span><span class="sxs-lookup"><span data-stu-id="45ee3-105">When a team is archived, users can no longer send or like messages on any channel in the team, edit the team's name, description, or other settings, or in general make most changes to the team.</span></span>
<span data-ttu-id="45ee3-106">Mitgliedschaftsänderungen an das Team weiterhin zugelassen werden.</span><span class="sxs-lookup"><span data-stu-id="45ee3-106">Membership changes to the team continue to be allowed.</span></span>

<span data-ttu-id="45ee3-107">Archivierung ist ein asynchroner Vorgang.</span><span class="sxs-lookup"><span data-stu-id="45ee3-107">Archiving is an async operation.</span></span> <span data-ttu-id="45ee3-108">Nach Abschluss des Vorgangs Async erfolgreich, die nach einer Antwort vom diese API auftreten können, ist ein Team archiviert.</span><span class="sxs-lookup"><span data-stu-id="45ee3-108">A team is archived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

<span data-ttu-id="45ee3-109">Zum Archivieren von Team benötigen die Teams und der [Gruppe](../resources/group.md) Besitzer.</span><span class="sxs-lookup"><span data-stu-id="45ee3-109">In order to archive team, the team and [group](../resources/group.md) must have an owner.</span></span>

<span data-ttu-id="45ee3-110">Um ein Team aus den archivierten Zustand wiederherzustellen, verwenden Sie die API zu [Öffnen](team-unarchive.md).</span><span class="sxs-lookup"><span data-stu-id="45ee3-110">To restore a team from its archived state, use the API to [unarchive](team-unarchive.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="45ee3-111">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="45ee3-111">Permissions</span></span>
<span data-ttu-id="45ee3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45ee3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45ee3-114">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="45ee3-114">Permission type</span></span>      | <span data-ttu-id="45ee3-115">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="45ee3-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45ee3-116">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="45ee3-116">Delegated (work or school account)</span></span> | <span data-ttu-id="45ee3-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45ee3-117">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="45ee3-118">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="45ee3-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45ee3-119">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="45ee3-119">Not supported.</span></span>    |
|<span data-ttu-id="45ee3-120">Anwendung</span><span class="sxs-lookup"><span data-stu-id="45ee3-120">Application</span></span> | <span data-ttu-id="45ee3-121">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45ee3-121">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="45ee3-122">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="45ee3-122">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="45ee3-123">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="45ee3-123">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="45ee3-124">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="45ee3-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/archive
```
## <a name="request-headers"></a><span data-ttu-id="45ee3-125">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="45ee3-125">Request headers</span></span>
| <span data-ttu-id="45ee3-126">Header</span><span class="sxs-lookup"><span data-stu-id="45ee3-126">Header</span></span>       | <span data-ttu-id="45ee3-127">Wert</span><span class="sxs-lookup"><span data-stu-id="45ee3-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="45ee3-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="45ee3-128">Authorization</span></span>  | <span data-ttu-id="45ee3-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="45ee3-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="45ee3-131">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="45ee3-131">Request body</span></span>
<span data-ttu-id="45ee3-132">In der Anforderung kann _optional_ umfassen die `shouldSetSpoSiteReadOnlyForMembers` Parameter in einem JSON body, wie folgt.</span><span class="sxs-lookup"><span data-stu-id="45ee3-132">In the request, you may _optionally_ include the `shouldSetSpoSiteReadOnlyForMembers` parameter in a JSON body, as follows.</span></span>
```JSON
{
    "shouldSetSpoSiteReadOnlyForMembers": true
}
```
<span data-ttu-id="45ee3-133">Dieser optionale Parameter definiert, ob Festlegen von Berechtigungen für Teammitglieder den Schreibschutz für die Sharepoint Online-Website mit dem Team verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="45ee3-133">This optional parameter defines whether to set permissions for team members to read-only on the Sharepoint Online site associated with the team.</span></span> <span data-ttu-id="45ee3-134">Festlegen der Steuerelementvorlage auf False oder im Textkörper auslassen führt vollständig in diesem Schritt wird übersprungen.</span><span class="sxs-lookup"><span data-stu-id="45ee3-134">Setting it to false or omitting the body altogether will result in this step being skipped.</span></span>

## <a name="response"></a><span data-ttu-id="45ee3-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="45ee3-135">Response</span></span>

<span data-ttu-id="45ee3-136">Wenn die Archivierung erfolgreich gestartet wurde, gibt diese Methode einen `202 Accepted` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="45ee3-136">If archiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="45ee3-137">Die Antwort enthält außerdem eine `Location` Kopf, der den Speicherort der die [TeamsAsyncOperation](../resources/teamsasyncoperation.md) enthält, die zum Behandeln des Teams Archivierung erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="45ee3-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle archiving of the team.</span></span> <span data-ttu-id="45ee3-138">Überprüfen Sie den Status des Vorgangs Archivierung, indem er eine GET-Anforderung an diesen Speicherort.</span><span class="sxs-lookup"><span data-stu-id="45ee3-138">Check the status of the archiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="45ee3-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="45ee3-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="45ee3-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="45ee3-140">Request</span></span>
<span data-ttu-id="45ee3-141">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="45ee3-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "archive_team"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/archive
```
#### <a name="response"></a><span data-ttu-id="45ee3-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="45ee3-142">Response</span></span>
<span data-ttu-id="45ee3-143">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="45ee3-143">The following is an example of a response.</span></span>
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
