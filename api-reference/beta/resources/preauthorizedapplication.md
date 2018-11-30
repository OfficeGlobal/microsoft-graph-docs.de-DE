---
title: Ressourcentyp preAuthorizedApplication
description: Stellt eine Anwendung und die angeforderten Berechtigungen für implizite Zustimmung dar. Erfordert ein Administrator Zustimmung an die Anwendung bereitgestellt haben. PreAuthorizedApplications erfordern keinen den Benutzer, die angeforderten Berechtigungen zuzustimmen. In PreAuthorizedApplications aufgelisteten Berechtigungen erfordern keine Zustimmung des Benutzers. Keine weiteren angeforderten Berechtigungen nicht in PreAuthorizedApplications aufgeführten erfordern jedoch Zustimmung des Benutzers.
ms.openlocfilehash: d299aefcac541407e0e42d0b0933e903afa3e84d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065760"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="a8bd1-107">Ressourcentyp preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="a8bd1-107">preAuthorizedApplication resource type</span></span>

> <span data-ttu-id="a8bd1-108">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="a8bd1-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a8bd1-109">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a8bd1-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a8bd1-110">Stellt eine Anwendung und die angeforderten Berechtigungen für implizite Zustimmung dar.</span><span class="sxs-lookup"><span data-stu-id="a8bd1-110">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="a8bd1-111">Erfordert ein Administrator Zustimmung an die Anwendung bereitgestellt haben.</span><span class="sxs-lookup"><span data-stu-id="a8bd1-111">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="a8bd1-112">PreAuthorizedApplications erfordern keinen den Benutzer, die angeforderten Berechtigungen zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="a8bd1-112">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="a8bd1-113">In PreAuthorizedApplications aufgelisteten Berechtigungen erfordern keine Zustimmung des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="a8bd1-113">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="a8bd1-114">Keine weiteren angeforderten Berechtigungen nicht in PreAuthorizedApplications aufgeführten erfordern jedoch Zustimmung des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="a8bd1-114">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="a8bd1-115">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a8bd1-115">Properties</span></span>

| <span data-ttu-id="a8bd1-116">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a8bd1-116">Property</span></span> | <span data-ttu-id="a8bd1-117">Typ</span><span class="sxs-lookup"><span data-stu-id="a8bd1-117">Type</span></span> | <span data-ttu-id="a8bd1-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a8bd1-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a8bd1-119">appId</span><span class="sxs-lookup"><span data-stu-id="a8bd1-119">appId</span></span>|<span data-ttu-id="a8bd1-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a8bd1-120">String</span></span>| <span data-ttu-id="a8bd1-121">Der eindeutige Bezeichner für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="a8bd1-121">The unique identifier for the application.</span></span> |
|<span data-ttu-id="a8bd1-122">permissionIds</span><span class="sxs-lookup"><span data-stu-id="a8bd1-122">permissionIds</span></span>|<span data-ttu-id="a8bd1-123">Collection von Objekten des Typs „String“</span><span class="sxs-lookup"><span data-stu-id="a8bd1-123">String collection</span></span>| <span data-ttu-id="a8bd1-124">Der eindeutige Bezeichner für die [PublishedPermissionScope](permissionscope.md) oder [AppRole](approle.md) die Anwendung erfordert.</span><span class="sxs-lookup"><span data-stu-id="a8bd1-124">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a8bd1-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a8bd1-125">JSON representation</span></span>
<span data-ttu-id="a8bd1-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a8bd1-126">Here is a JSON representation of the resource.</span></span>

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