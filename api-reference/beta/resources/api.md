---
title: API-Ressourcentyp
description: Gibt die Einstellungen für eine-API-Webanwendung.
localization_priority: Normal
ms.openlocfilehash: 50c21c31fec7434514408e1a214c6edf2b838c98
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845207"
---
# <a name="api-resource-type"></a><span data-ttu-id="f17a9-103">API-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f17a9-103">api resource type</span></span>

> <span data-ttu-id="f17a9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f17a9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f17a9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f17a9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f17a9-106">Gibt die Einstellungen für eine-API-Webanwendung.</span><span class="sxs-lookup"><span data-stu-id="f17a9-106">Specifies settings for a Web API application.</span></span>

## <a name="properties"></a><span data-ttu-id="f17a9-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f17a9-107">Properties</span></span>

| <span data-ttu-id="f17a9-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f17a9-108">Property</span></span> | <span data-ttu-id="f17a9-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f17a9-109">Type</span></span> | <span data-ttu-id="f17a9-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f17a9-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f17a9-111">requestedAccessTokenVersion</span><span class="sxs-lookup"><span data-stu-id="f17a9-111">requestedAccessTokenVersion</span></span>|<span data-ttu-id="f17a9-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f17a9-112">Int32</span></span>| <span data-ttu-id="f17a9-113">Gibt die Version der akzeptierten Access token für die aktuelle API-Ressource.</span><span class="sxs-lookup"><span data-stu-id="f17a9-113">Specifies the accepted access token version for the current API resource.</span></span> <span data-ttu-id="f17a9-114">Mögliche Werte sind 1 oder 2.</span><span class="sxs-lookup"><span data-stu-id="f17a9-114">Possible values are 1 or 2.</span></span>  |
|<span data-ttu-id="f17a9-115">oauth2PermissionScopes</span><span class="sxs-lookup"><span data-stu-id="f17a9-115">oauth2PermissionScopes</span></span>|<span data-ttu-id="f17a9-116">[PermissionScope](permissionscope.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="f17a9-116">[permissionScope](permissionscope.md) collection</span></span>| <span data-ttu-id="f17a9-117">Die Auflistung von OAuth 2.0-berechtigungsbereiche, die im Web-API (Ressource) Anwendung Clientanwendungen verfügbar macht.</span><span class="sxs-lookup"><span data-stu-id="f17a9-117">The collection of OAuth 2.0 permission scopes that the web API (resource) application exposes to client applications.</span></span> <span data-ttu-id="f17a9-118">Diese berechtigungsbereiche können während der Zustimmung Clientanwendungen gewährt werden.</span><span class="sxs-lookup"><span data-stu-id="f17a9-118">These permission scopes may be granted to client applications during consent.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f17a9-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f17a9-119">JSON representation</span></span>
<span data-ttu-id="f17a9-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f17a9-120">Here is a JSON representation of the resource.</span></span>

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
