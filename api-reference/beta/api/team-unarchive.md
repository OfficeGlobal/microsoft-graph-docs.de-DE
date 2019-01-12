---
title: Entpackt team
description: Wiederherstellen eines archivierten Teams. Dadurch wird die Möglichkeit zum Senden von Nachrichten und das Team Verhältnismäßigkeitsprinzips Mandanten und Team-Einstellungen Bearbeiten des Benutzers wiederhergestellt. Teams sind mithilfe des Archivs API archiviert.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: b5c64c9c04c7c3cc3549721747c27361680bd03a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977668"
---
# <a name="unarchive-team"></a><span data-ttu-id="3109c-105">Entpackt team</span><span class="sxs-lookup"><span data-stu-id="3109c-105">Unarchive team</span></span>

> <span data-ttu-id="3109c-106">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="3109c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3109c-107">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3109c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3109c-108">Wiederherstellen eines archivierten [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="3109c-108">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="3109c-109">Dadurch wird die Möglichkeit zum Senden von Nachrichten und das Team Verhältnismäßigkeitsprinzips Mandanten und Team-Einstellungen Bearbeiten des Benutzers wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="3109c-109">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="3109c-110">Teams sind mit dem [Archiv](team-archive.md) API archiviert.</span><span class="sxs-lookup"><span data-stu-id="3109c-110">Teams are archived using the [archive](team-archive.md) API.</span></span>

<span data-ttu-id="3109c-111">Unarchiving ist ein asynchroner Vorgang.</span><span class="sxs-lookup"><span data-stu-id="3109c-111">Unarchiving is an async operation.</span></span> <span data-ttu-id="3109c-112">Ein Team ist nicht archivierte, sobald der asynchrone Vorgang erfolgreich abgeschlossen wurde die nach einer Antwort vom diese API auftreten können.</span><span class="sxs-lookup"><span data-stu-id="3109c-112">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="3109c-113">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="3109c-113">Permissions</span></span>
<span data-ttu-id="3109c-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3109c-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3109c-116">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="3109c-116">Permission type</span></span>      | <span data-ttu-id="3109c-117">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="3109c-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3109c-118">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="3109c-118">Delegated (work or school account)</span></span> | <span data-ttu-id="3109c-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3109c-119">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3109c-120">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="3109c-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3109c-121">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="3109c-121">Not supported.</span></span>    |
|<span data-ttu-id="3109c-122">Anwendung</span><span class="sxs-lookup"><span data-stu-id="3109c-122">Application</span></span> | <span data-ttu-id="3109c-123">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3109c-123">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="3109c-124">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="3109c-124">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3109c-125">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="3109c-125">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3109c-126">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="3109c-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="3109c-127">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="3109c-127">Request headers</span></span>
| <span data-ttu-id="3109c-128">Header</span><span class="sxs-lookup"><span data-stu-id="3109c-128">Header</span></span>       | <span data-ttu-id="3109c-129">Wert</span><span class="sxs-lookup"><span data-stu-id="3109c-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3109c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="3109c-130">Authorization</span></span>  | <span data-ttu-id="3109c-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="3109c-p107">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3109c-133">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="3109c-133">Request body</span></span>
<span data-ttu-id="3109c-134">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="3109c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3109c-135">Antwort</span><span class="sxs-lookup"><span data-stu-id="3109c-135">Response</span></span>

<span data-ttu-id="3109c-136">Wenn unarchiving erfolgreich gestartet wurde, gibt diese Methode einen `202 Accepted` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="3109c-136">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="3109c-137">Die Antwort enthält außerdem eine `Location` Kopf, der den Speicherort der die [TeamsAsyncOperation](../resources/teamsasyncoperation.md) enthält, die zur Verarbeitung von unarchiving des Teams erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="3109c-137">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="3109c-138">Überprüfen Sie den Status des Vorgangs unarchiving, indem er eine GET-Anforderung an diesen Speicherort.</span><span class="sxs-lookup"><span data-stu-id="3109c-138">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="3109c-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="3109c-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="3109c-140">Anforderung</span><span class="sxs-lookup"><span data-stu-id="3109c-140">Request</span></span>
<span data-ttu-id="3109c-141">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="3109c-141">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="3109c-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="3109c-142">Response</span></span>
<span data-ttu-id="3109c-143">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="3109c-143">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
