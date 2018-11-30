---
title: Registerkarte Channel hinzufügen
description: 'Fügt (Pins) einer Registerkarte an den angegebenen Kanal innerhalb eines Teams. '
ms.openlocfilehash: be246b0308be83e0b411fa89fe16034018756829
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059723"
---
# <a name="add-tab-to-channel"></a><span data-ttu-id="ace04-103">Registerkarte Channel hinzufügen</span><span class="sxs-lookup"><span data-stu-id="ace04-103">Add tab to channel</span></span>

> <span data-ttu-id="ace04-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="ace04-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ace04-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ace04-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ace04-106">Fügt (Pins) einer [Registerkarte](../resources/teamstab.md) an den angegebenen [DDE-Kanal](../resources/channel.md) in einem [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ace04-106">Adds (pins) a [tab](../resources/teamstab.md) to the specified [channel](../resources/channel.md) within a [team](../resources/team.md).</span></span> <span data-ttu-id="ace04-107">Die entsprechende app muss bereits [im Team installiert](../api/teamsappinstallation-add.md)sein.</span><span class="sxs-lookup"><span data-stu-id="ace04-107">The corresponding app must already be [installed in the team](../api/teamsappinstallation-add.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ace04-108">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ace04-108">Permissions</span></span>
<span data-ttu-id="ace04-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ace04-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ace04-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ace04-111">Permission type</span></span>      | <span data-ttu-id="ace04-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ace04-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ace04-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ace04-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ace04-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ace04-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ace04-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ace04-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ace04-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ace04-116">Not supported.</span></span>    |
| <span data-ttu-id="ace04-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ace04-117">Application</span></span>                            | <span data-ttu-id="ace04-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ace04-118">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="ace04-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ace04-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels/{id}/tabs
```

## <a name="request-headers"></a><span data-ttu-id="ace04-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ace04-120">Request headers</span></span>
| <span data-ttu-id="ace04-121">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="ace04-121">Header</span></span>       | <span data-ttu-id="ace04-122">Wert</span><span class="sxs-lookup"><span data-stu-id="ace04-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ace04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ace04-123">Authorization</span></span>  | <span data-ttu-id="ace04-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ace04-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ace04-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ace04-126">Request body</span></span>

<span data-ttu-id="ace04-127">Ein [TeamsTab](../resources/teamstab.md).</span><span class="sxs-lookup"><span data-stu-id="ace04-127">A [teamsTab](../resources/teamstab.md).</span></span>

## <a name="response"></a><span data-ttu-id="ace04-128">Antwort</span><span class="sxs-lookup"><span data-stu-id="ace04-128">Response</span></span>

<span data-ttu-id="ace04-129">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `201 OK` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ace04-129">If successful, this method returns a `201 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ace04-130">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ace04-130">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ace04-131">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ace04-131">Request</span></span>

<span data-ttu-id="ace04-132">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="ace04-132">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="ace04-133">Antwort</span><span class="sxs-lookup"><span data-stu-id="ace04-133">Response</span></span>

<span data-ttu-id="ace04-134">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ace04-134">The following is an example of the response.</span></span> <span data-ttu-id="ace04-135">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ace04-135">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="ace04-136">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ace04-136">All of the properties will be returned from an actual call.</span></span>
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
  "sortOrderIndex": 20,
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="ace04-137">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="ace04-137">See also</span></span>

[<span data-ttu-id="ace04-138">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="ace04-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Add tab to channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->