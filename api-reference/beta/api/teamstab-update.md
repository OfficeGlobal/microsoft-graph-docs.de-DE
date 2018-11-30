---
title: Registerkarte "Aktualisieren"
description: Aktualisieren Sie die Eigenschaften der angegebenen Registerkarte.
ms.openlocfilehash: 6943e9ea4ff602b3fcd4dc8ac899d55cee120ecc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059727"
---
# <a name="update-tab"></a><span data-ttu-id="4e8d0-103">Registerkarte "Aktualisieren"</span><span class="sxs-lookup"><span data-stu-id="4e8d0-103">Update tab</span></span>

> <span data-ttu-id="4e8d0-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4e8d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e8d0-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4e8d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e8d0-106">Aktualisieren Sie die Eigenschaften der angegebenen [Registerkarte](../resources/teamstab.md). Dies kann so konfigurieren Sie den Inhalt der Registerkarte verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="4e8d0-106">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e8d0-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4e8d0-107">Permissions</span></span>
<span data-ttu-id="4e8d0-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e8d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4e8d0-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4e8d0-110">Permission type</span></span>      | <span data-ttu-id="4e8d0-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4e8d0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e8d0-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4e8d0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4e8d0-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e8d0-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4e8d0-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4e8d0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e8d0-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4e8d0-115">Not supported.</span></span>    |
|<span data-ttu-id="4e8d0-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4e8d0-116">Application</span></span>                            | <span data-ttu-id="4e8d0-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e8d0-117">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="4e8d0-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e8d0-118">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4e8d0-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4e8d0-119">Request headers</span></span>
| <span data-ttu-id="4e8d0-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="4e8d0-120">Header</span></span>       | <span data-ttu-id="4e8d0-121">Wert</span><span class="sxs-lookup"><span data-stu-id="4e8d0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4e8d0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e8d0-122">Authorization</span></span>  | <span data-ttu-id="4e8d0-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4e8d0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4e8d0-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e8d0-125">Content-Type</span></span>  | <span data-ttu-id="4e8d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e8d0-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4e8d0-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4e8d0-127">Request body</span></span>
<span data-ttu-id="4e8d0-128">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der [Tab](../resources/teamstab.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="4e8d0-128">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4e8d0-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e8d0-129">Response</span></span>

<span data-ttu-id="4e8d0-130">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4e8d0-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4e8d0-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4e8d0-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4e8d0-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4e8d0-132">Request</span></span>
<span data-ttu-id="4e8d0-133">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4e8d0-133">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="4e8d0-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="4e8d0-134">Response</span></span>
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

## <a name="see-also"></a><span data-ttu-id="4e8d0-135">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="4e8d0-135">See also</span></span>

[<span data-ttu-id="4e8d0-136">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="4e8d0-136">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
