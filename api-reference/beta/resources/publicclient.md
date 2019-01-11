---
title: Ressourcentyp publicClient
description: Gibt die Einstellungen für nicht Web App oder Web-Api. (Mobile oder anderen öffentlichen Client wie eine installierte Anwendung, die auf einem Desktopgerät ausgeführt)
localization_priority: Normal
ms.openlocfilehash: c466c91f90ac8adc2bf3806fa212e0b01e6d2507
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864197"
---
# <a name="publicclient-resource-type"></a><span data-ttu-id="99c6d-104">Ressourcentyp publicClient</span><span class="sxs-lookup"><span data-stu-id="99c6d-104">publicClient resource type</span></span>

> <span data-ttu-id="99c6d-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="99c6d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99c6d-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="99c6d-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="99c6d-107">Gibt die Einstellungen für nicht Web App oder Web-Api.</span><span class="sxs-lookup"><span data-stu-id="99c6d-107">Specifies settings for non Web App or Web Api.</span></span> <span data-ttu-id="99c6d-108">(Mobile oder anderen öffentlichen Client wie eine installierte Anwendung, die auf einem Desktopgerät ausgeführt)</span><span class="sxs-lookup"><span data-stu-id="99c6d-108">(e.g. Mobile or other public client such as an installed application running on a desktop device)</span></span>

## <a name="properties"></a><span data-ttu-id="99c6d-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="99c6d-109">Properties</span></span>

| <span data-ttu-id="99c6d-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="99c6d-110">Property</span></span> | <span data-ttu-id="99c6d-111">Typ</span><span class="sxs-lookup"><span data-stu-id="99c6d-111">Type</span></span> | <span data-ttu-id="99c6d-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99c6d-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="99c6d-113">redirectUris</span><span class="sxs-lookup"><span data-stu-id="99c6d-113">redirectUris</span></span>|<span data-ttu-id="99c6d-114">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="99c6d-114">String collection</span></span>| <span data-ttu-id="99c6d-115">Gibt die URLs der Benutzertoken für die Anmeldung an gesendet werden, oder die Umleitung, URIs, dass OAuth 2.0 Autorisierungscodes und Zugriffstoken gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="99c6d-115">Specifies the URLs that user tokens are sent to for sign in, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="99c6d-116">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="99c6d-116">JSON representation</span></span>
<span data-ttu-id="99c6d-117">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="99c6d-117">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "installedClient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
