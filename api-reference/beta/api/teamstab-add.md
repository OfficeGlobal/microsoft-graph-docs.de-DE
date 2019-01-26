---
title: Registerkarte Channel hinzufügen
description: 'Fügt (Pins) einer Registerkarte an den angegebenen Kanal innerhalb eines Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1de8cfe1d553a6e0f70653aa4fe1d978c8d92323
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29570932"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="1bb50-103">Registerkarte Channel hinzufügen</span><span class="sxs-lookup"><span data-stu-id="1bb50-103">Add tab to channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1bb50-104">Fügt (Pins) einer [Registerkarte](../resources/teamstab.md) an den angegebenen [DDE-Kanal](../resources/channel.md) in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="1bb50-104">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="1bb50-105">Die entsprechende app muss bereits [im Team installiert](../api/teamsappinstallation-add.md)sein.</span><span class="sxs-lookup"><span data-stu-id="1bb50-105">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="1bb50-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1bb50-106">Permissions</span></span>
<span data-ttu-id="1bb50-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1bb50-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1bb50-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1bb50-109">Permission type</span></span>      | <span data-ttu-id="1bb50-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1bb50-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1bb50-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1bb50-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1bb50-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bb50-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1bb50-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1bb50-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1bb50-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1bb50-114">Not supported.</span></span>    |
| <span data-ttu-id="1bb50-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1bb50-115">Application</span></span>                            | <span data-ttu-id="1bb50-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bb50-116">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="1bb50-117">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="1bb50-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="1bb50-118">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="1bb50-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="1bb50-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1bb50-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="1bb50-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1bb50-120">Request headers</span></span>
| <span data-ttu-id="1bb50-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1bb50-121">Header</span></span>       | <span data-ttu-id="1bb50-122">Wert</span><span class="sxs-lookup"><span data-stu-id="1bb50-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1bb50-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bb50-123">Authorization</span></span>  | <span data-ttu-id="1bb50-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1bb50-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1bb50-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1bb50-126">Request body</span></span>

<span data-ttu-id="1bb50-127">Ein [TeamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="1bb50-127">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="1bb50-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="1bb50-128">Response</span></span>

<span data-ttu-id="1bb50-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `201 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1bb50-129">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1bb50-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1bb50-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="1bb50-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1bb50-131">Request</span></span>

<span data-ttu-id="1bb50-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1bb50-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs
{
  "name": "My Contoso Tab",
  "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  }
}
```

#### <a name="response"></a><span data-ttu-id="1bb50-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="1bb50-133">Response</span></span>

<span data-ttu-id="1bb50-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1bb50-134">The following is an example of the response.</span></span> <span data-ttu-id="1bb50-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="1bb50-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1bb50-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1bb50-136">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "794f0e4e-4d10-4bb5-9079-3a465a629eff",
  "name": "My Contoso Tab",
  "configuration": {
    "entityId": "2DCA2E6C7A10415CAF6B8AB6661B3154",
    "contentUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/tabView",
    "websiteUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154",
    "removeUrl": "https://www.contoso.com/Orders/2DCA2E6C7A10415CAF6B8AB6661B3154/uninstallTab"
  },
  "sortOrderIndex": "20",
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="1bb50-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="1bb50-137">See also</span></span>

[<span data-ttu-id="1bb50-138">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="1bb50-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/teamstab-add.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
