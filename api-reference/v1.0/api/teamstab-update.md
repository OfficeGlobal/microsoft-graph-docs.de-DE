---
title: Registerkarte "Aktualisieren"
description: Aktualisieren Sie die Eigenschaften der angegebenen Registerkarte.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: fcfbf2e0b3ce44e91f709645108abe90ea781f0d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573620"
---
# <a name="update-tab"></a><span data-ttu-id="8a903-103">Registerkarte "Aktualisieren"</span><span class="sxs-lookup"><span data-stu-id="8a903-103">Update tab</span></span>



<span data-ttu-id="8a903-104">Aktualisieren Sie die Eigenschaften der angegebenen [Registerkarte](../resources/teamstab.md). Dies kann so konfigurieren Sie den Inhalt der Registerkarte verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="8a903-104">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="8a903-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8a903-105">Permissions</span></span>
<span data-ttu-id="8a903-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="8a903-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="8a903-108">Permission type</span></span>      | <span data-ttu-id="8a903-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="8a903-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8a903-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="8a903-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8a903-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a903-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8a903-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="8a903-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8a903-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="8a903-113">Not supported.</span></span>    |
|<span data-ttu-id="8a903-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="8a903-114">Application</span></span>                            | <span data-ttu-id="8a903-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a903-115">Group.ReadWrite.All</span></span>                         |

> <span data-ttu-id="8a903-116">**Hinweis**: Diese API unterstützt Administratorberechtigungen.</span><span class="sxs-lookup"><span data-stu-id="8a903-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8a903-117">Globale Administratoren und Microsoft-Teams Dienstadministratoren können Teams zugreifen, denen sie nicht Mitglied sind.</span><span class="sxs-lookup"><span data-stu-id="8a903-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8a903-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a903-118">HTTP request</span></span>

```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8a903-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="8a903-119">Request headers</span></span>
| <span data-ttu-id="8a903-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="8a903-120">Header</span></span>       | <span data-ttu-id="8a903-121">Wert</span><span class="sxs-lookup"><span data-stu-id="8a903-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8a903-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8a903-122">Authorization</span></span>  | <span data-ttu-id="8a903-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8a903-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8a903-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8a903-125">Content-Type</span></span>  | <span data-ttu-id="8a903-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a903-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8a903-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="8a903-127">Request body</span></span>
<span data-ttu-id="8a903-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der [Tab](../resources/teamstab.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="8a903-128">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8a903-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a903-129">Response</span></span>

<span data-ttu-id="8a903-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="8a903-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8a903-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="8a903-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="8a903-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="8a903-132">Request</span></span>
<span data-ttu-id="8a903-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="8a903-133">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="8a903-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="8a903-134">Response</span></span>
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
  "webUrl": "https://teams.microsoft.com/l/channel/19%3ac2e36757ee744c569e70b385e6dd79b6%40thread.skype/tab%3a%3afd736d46-51ed-4c0b-9b23-e67ca354bb24?label=my%20%contoso%to%tab"
}
```

## <a name="see-also"></a><span data-ttu-id="8a903-135">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="8a903-135">See also</span></span>

[<span data-ttu-id="8a903-136">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="8a903-136">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
