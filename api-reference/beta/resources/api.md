---
title: API-Ressourcentyp
description: Gibt die Einstellungen für eine-API-Webanwendung.
ms.openlocfilehash: b5b07ccb5a66027f9eb755754842f6e2e2ae708e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060464"
---
# <a name="api-resource-type"></a><span data-ttu-id="332f7-103">API-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="332f7-103">api resource type</span></span>

> <span data-ttu-id="332f7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="332f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="332f7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="332f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="332f7-106">Gibt die Einstellungen für eine-API-Webanwendung.</span><span class="sxs-lookup"><span data-stu-id="332f7-106">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="332f7-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="332f7-107">Properties</span></span>

| <span data-ttu-id="332f7-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="332f7-108">Property</span></span> | <span data-ttu-id="332f7-109">Typ</span><span class="sxs-lookup"><span data-stu-id="332f7-109">Type</span></span> | <span data-ttu-id="332f7-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="332f7-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="332f7-111">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="332f7-111">requestedAccessTokenVersion</span></span>|<span data-ttu-id="332f7-112">Int32</span><span class="sxs-lookup"><span data-stu-id="332f7-112">Int32</span></span>| <span data-ttu-id="332f7-113">Gibt die Version der akzeptierten Access token für die aktuelle API-Ressource.</span><span class="sxs-lookup"><span data-stu-id="332f7-113">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="332f7-114">Mögliche Werte sind 1 oder 2.</span><span class="sxs-lookup"><span data-stu-id="332f7-114">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="332f7-115">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="332f7-115">oauth2PermissionScopes</span></span>|<span data-ttu-id="332f7-116">[PermissionScope](permissionscope.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="332f7-116">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="332f7-117">Die Auflistung von OAuth 2.0-berechtigungsbereiche, die im Web-API (Ressource) Anwendung Clientanwendungen verfügbar macht.</span><span class="sxs-lookup"><span data-stu-id="332f7-117">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="332f7-118">Diese berechtigungsbereiche können während der Zustimmung Clientanwendungen gewährt werden.</span><span class="sxs-lookup"><span data-stu-id="332f7-118">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="332f7-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="332f7-119">JSON representation</span></span>
<span data-ttu-id="332f7-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="332f7-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.api"
}-->

```json
{
  "requestedAccessTokenVersion": 1,
  "oauth2PermissionScopes": [{"@odata.type": "microsoft.graph.permissionScope"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "api resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->