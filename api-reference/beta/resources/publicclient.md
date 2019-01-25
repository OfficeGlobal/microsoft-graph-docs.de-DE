---
title: Ressourcentyp publicClient
description: Gibt die Einstellungen für nicht Web App oder Web-Api. (Mobile oder anderen öffentlichen Client wie eine installierte Anwendung, die auf einem Desktopgerät ausgeführt)
localization_priority: Normal
ms.openlocfilehash: ff1d77709293a7167868451671e1660196c9a4db
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525962"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="a1309-104">Ressourcentyp publicClient</span><span class="sxs-lookup"><span data-stu-id="a1309-104">publicClient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1309-105">Gibt die Einstellungen für nicht Web App oder Web-Api.</span><span class="sxs-lookup"><span data-stu-id="a1309-105">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="a1309-106">(Mobile oder anderen öffentlichen Client wie eine installierte Anwendung, die auf einem Desktopgerät ausgeführt)</span><span class="sxs-lookup"><span data-stu-id="a1309-106">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="a1309-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a1309-107">Properties</span></span>

| <span data-ttu-id="a1309-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a1309-108">Property</span></span> | <span data-ttu-id="a1309-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a1309-109">Type</span></span> | <span data-ttu-id="a1309-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a1309-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a1309-111">redirectUris</span><span class="sxs-lookup"><span data-stu-id="a1309-111">redirectUris</span></span>|<span data-ttu-id="a1309-112">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="a1309-112">String collection</span></span>| <span data-ttu-id="a1309-113">Gibt die URLs der Benutzertoken für die Anmeldung an gesendet werden, oder die Umleitung, URIs, dass OAuth 2.0 Autorisierungscodes und Zugriffstoken gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="a1309-113">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a1309-114">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a1309-114">JSON representation</span></span>
<span data-ttu-id="a1309-115">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a1309-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.installedClient"
}-->

```json
{
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/publicclient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
