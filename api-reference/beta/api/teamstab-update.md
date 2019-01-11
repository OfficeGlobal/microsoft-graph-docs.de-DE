---
title: Registerkarte "Aktualisieren"
description: Aktualisieren Sie die Eigenschaften der angegebenen Registerkarte.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: c17381432465ae318d86a818922d161ab46e762f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815064"
---
# <a name="update-tab"></a><span data-ttu-id="c4489-103">Registerkarte "Aktualisieren"</span><span class="sxs-lookup"><span data-stu-id="c4489-103">Update tab</span></span>

> <span data-ttu-id="c4489-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="c4489-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4489-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="c4489-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4489-106">Aktualisieren Sie die Eigenschaften der angegebenen [Registerkarte](../resources/teamstab.md). Dies kann so konfigurieren Sie den Inhalt der Registerkarte verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="c4489-106">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4489-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="c4489-107">Permissions</span></span>
<span data-ttu-id="c4489-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4489-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c4489-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="c4489-110">Permission type</span></span>      | <span data-ttu-id="c4489-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="c4489-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4489-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="c4489-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c4489-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4489-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4489-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="c4489-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4489-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="c4489-115">Not supported.</span></span>    |
|<span data-ttu-id="c4489-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="c4489-116">Application</span></span>                            | <span data-ttu-id="c4489-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4489-117">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="c4489-118">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="c4489-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="c4489-119">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="c4489-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="c4489-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4489-120">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c4489-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="c4489-121">Request headers</span></span>
| <span data-ttu-id="c4489-122">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="c4489-122">Header</span></span>       | <span data-ttu-id="c4489-123">Wert</span><span class="sxs-lookup"><span data-stu-id="c4489-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c4489-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4489-124">Authorization</span></span>  | <span data-ttu-id="c4489-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="c4489-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c4489-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c4489-127">Content-Type</span></span>  | <span data-ttu-id="c4489-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c4489-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4489-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="c4489-129">Request body</span></span>
<span data-ttu-id="c4489-130">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der [Tab](../resources/teamstab.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="c4489-130">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c4489-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4489-131">Response</span></span>

<span data-ttu-id="c4489-132">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c4489-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c4489-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="c4489-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c4489-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="c4489-134">Request</span></span>
<span data-ttu-id="c4489-135">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="c4489-135">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="c4489-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="c4489-136">Response</span></span>
```http
HTTP/1.1 200 Success
Content-type: application/json

{
  "id": "tabId",
  "name": "My Contoso Tab - updated",
  "teamsAppId": "06805b9e-77e3-4b93-ac81-525eb87513b8",
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

## <a name="see-also"></a><span data-ttu-id="c4489-137">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="c4489-137">See also</span></span>

[<span data-ttu-id="c4489-138">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="c4489-138">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
