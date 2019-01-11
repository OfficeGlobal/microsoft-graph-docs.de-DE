---
title: Ressourcentyp preAuthorizedApplication
description: Stellt eine Anwendung und die angeforderten Berechtigungen für implizite Zustimmung dar. Erfordert ein Administrator Zustimmung an die Anwendung bereitgestellt haben. PreAuthorizedApplications erfordern keinen den Benutzer, die angeforderten Berechtigungen zuzustimmen. In PreAuthorizedApplications aufgelisteten Berechtigungen erfordern keine Zustimmung des Benutzers. Keine weiteren angeforderten Berechtigungen nicht in PreAuthorizedApplications aufgeführten erfordern jedoch Zustimmung des Benutzers.
localization_priority: Normal
ms.openlocfilehash: fa26b8046b81db70300b8ff40abcbd2b84f3f0c8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832795"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="6026e-107">Ressourcentyp preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="6026e-107">preAuthorizedApplication resource type</span></span>

> <span data-ttu-id="6026e-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6026e-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6026e-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6026e-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6026e-110">Stellt eine Anwendung und die angeforderten Berechtigungen für implizite Zustimmung dar.</span><span class="sxs-lookup"><span data-stu-id="6026e-110">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="6026e-111">Erfordert ein Administrator Zustimmung an die Anwendung bereitgestellt haben.</span><span class="sxs-lookup"><span data-stu-id="6026e-111">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="6026e-112">PreAuthorizedApplications erfordern keinen den Benutzer, die angeforderten Berechtigungen zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="6026e-112">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="6026e-113">In PreAuthorizedApplications aufgelisteten Berechtigungen erfordern keine Zustimmung des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="6026e-113">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="6026e-114">Keine weiteren angeforderten Berechtigungen nicht in PreAuthorizedApplications aufgeführten erfordern jedoch Zustimmung des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="6026e-114">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="6026e-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6026e-115">Properties</span></span>

| <span data-ttu-id="6026e-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6026e-116">Property</span></span> | <span data-ttu-id="6026e-117">Typ</span><span class="sxs-lookup"><span data-stu-id="6026e-117">Type</span></span> | <span data-ttu-id="6026e-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6026e-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6026e-119">appId</span><span class="sxs-lookup"><span data-stu-id="6026e-119">appId</span></span>|<span data-ttu-id="6026e-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="6026e-120">String</span></span>| <span data-ttu-id="6026e-121">Der eindeutige Bezeichner für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="6026e-121">The unique identifier for the application.</span></span> |
|<span data-ttu-id="6026e-122">permissionIds</span><span class="sxs-lookup"><span data-stu-id="6026e-122">permissionIds</span></span>|<span data-ttu-id="6026e-123">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="6026e-123">String collection</span></span>| <span data-ttu-id="6026e-124">Der eindeutige Bezeichner für die [PublishedPermissionScope](permissionscope.md) oder [AppRole](approle.md) die Anwendung erfordert.</span><span class="sxs-lookup"><span data-stu-id="6026e-124">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6026e-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6026e-125">JSON representation</span></span>
<span data-ttu-id="6026e-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6026e-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
