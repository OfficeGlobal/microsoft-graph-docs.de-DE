---
title: Registerkarte "Aktualisieren"
description: Aktualisieren Sie die Eigenschaften der angegebenen Registerkarte.
ms.openlocfilehash: fb2346fbadcb9794e05f8bb583596536a5710052
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019187"
---
# <a name="update-tab"></a><span data-ttu-id="2dfa8-103">Registerkarte "Aktualisieren"</span><span class="sxs-lookup"><span data-stu-id="2dfa8-103">Update tab</span></span>



<span data-ttu-id="2dfa8-104">Aktualisieren Sie die Eigenschaften der angegebenen [Registerkarte](../resources/teamstab.md). Dies kann so konfigurieren Sie den Inhalt der Registerkarte verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="2dfa8-104">Update the properties of the specified [tab](../resources/teamstab.md). This can be used to configure the content of the tab.</span></span>

## <a name="permissions"></a><span data-ttu-id="2dfa8-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2dfa8-105">Permissions</span></span>
<span data-ttu-id="2dfa8-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2dfa8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="2dfa8-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2dfa8-108">Permission type</span></span>      | <span data-ttu-id="2dfa8-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2dfa8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dfa8-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2dfa8-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2dfa8-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dfa8-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2dfa8-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2dfa8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2dfa8-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2dfa8-113">Not supported.</span></span>    |
|<span data-ttu-id="2dfa8-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="2dfa8-114">Application</span></span>                            | <span data-ttu-id="2dfa8-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dfa8-115">Group.ReadWrite.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="2dfa8-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2dfa8-116">HTTP request</span></span>
```http
PATCH /teams/{id}/channels/{id}/tabs/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2dfa8-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2dfa8-117">Request headers</span></span>
| <span data-ttu-id="2dfa8-118">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="2dfa8-118">Header</span></span>       | <span data-ttu-id="2dfa8-119">Wert</span><span class="sxs-lookup"><span data-stu-id="2dfa8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2dfa8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2dfa8-120">Authorization</span></span>  | <span data-ttu-id="2dfa8-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2dfa8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2dfa8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2dfa8-123">Content-Type</span></span>  | <span data-ttu-id="2dfa8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2dfa8-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2dfa8-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2dfa8-125">Request body</span></span>
<span data-ttu-id="2dfa8-126">Geben Sie im Textkörper Anforderung eine JSON-Darstellung der [Tab](../resources/teamstab.md) -Objekt.</span><span class="sxs-lookup"><span data-stu-id="2dfa8-126">In the request body, supply a JSON representation of [tab](../resources/teamstab.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2dfa8-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="2dfa8-127">Response</span></span>

<span data-ttu-id="2dfa8-128">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2dfa8-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2dfa8-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2dfa8-129">Example</span></span>
#### <a name="request"></a><span data-ttu-id="2dfa8-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2dfa8-130">Request</span></span>
<span data-ttu-id="2dfa8-131">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2dfa8-131">The following is an example of the request.</span></span>
```http
PATCH https://graph.microsoft.com/beta/teams/{id}/channels/{id}/tabs/{id}
Content-type: application/json
Content-length: 211

{
  "name": "My Contoso Tab - updated"
}
```
#### <a name="response"></a><span data-ttu-id="2dfa8-132">Antwort</span><span class="sxs-lookup"><span data-stu-id="2dfa8-132">Response</span></span>
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

## <a name="see-also"></a><span data-ttu-id="2dfa8-133">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="2dfa8-133">See also</span></span>

[<span data-ttu-id="2dfa8-134">Konfigurieren der integrierten Registerkartentypen</span><span class="sxs-lookup"><span data-stu-id="2dfa8-134">Configuring the built-in tab types</span></span>](/graph/teams-configuring-builtin-tabs)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tab in channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
