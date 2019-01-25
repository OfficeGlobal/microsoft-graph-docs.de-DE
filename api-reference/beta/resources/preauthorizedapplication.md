---
title: Ressourcentyp preAuthorizedApplication
description: Stellt eine Anwendung und die angeforderten Berechtigungen für implizite Zustimmung dar. Erfordert ein Administrator Zustimmung an die Anwendung bereitgestellt haben. PreAuthorizedApplications erfordern keinen den Benutzer, die angeforderten Berechtigungen zuzustimmen. In PreAuthorizedApplications aufgelisteten Berechtigungen erfordern keine Zustimmung des Benutzers. Keine weiteren angeforderten Berechtigungen nicht in PreAuthorizedApplications aufgeführten erfordern jedoch Zustimmung des Benutzers.
localization_priority: Normal
ms.openlocfilehash: 22945589341066f4609d47773cb04426774648fd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524548"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="4c865-107">Ressourcentyp preAuthorizedApplication</span><span class="sxs-lookup"><span data-stu-id="4c865-107">preAuthorizedApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c865-108">Stellt eine Anwendung und die angeforderten Berechtigungen für implizite Zustimmung dar.</span><span class="sxs-lookup"><span data-stu-id="4c865-108">Represents an application and requested permissions for implicit consent.</span></span> <span data-ttu-id="4c865-109">Erfordert ein Administrator Zustimmung an die Anwendung bereitgestellt haben.</span><span class="sxs-lookup"><span data-stu-id="4c865-109">Requires an admin to have provided consent to the application.</span></span> <span data-ttu-id="4c865-110">PreAuthorizedApplications erfordern keinen den Benutzer, die angeforderten Berechtigungen zuzustimmen.</span><span class="sxs-lookup"><span data-stu-id="4c865-110">preAuthorizedApplications do not require the user to consent to the requested permissions.</span></span> <span data-ttu-id="4c865-111">In PreAuthorizedApplications aufgelisteten Berechtigungen erfordern keine Zustimmung des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="4c865-111">Permissions listed in preAuthorizedApplications do not require user consent.</span></span> <span data-ttu-id="4c865-112">Keine weiteren angeforderten Berechtigungen nicht in PreAuthorizedApplications aufgeführten erfordern jedoch Zustimmung des Benutzers.</span><span class="sxs-lookup"><span data-stu-id="4c865-112">However, any additional requested permissions not listed in preAuthorizedApplications require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="4c865-113">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4c865-113">Properties</span></span>

| <span data-ttu-id="4c865-114">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4c865-114">Property</span></span> | <span data-ttu-id="4c865-115">Typ</span><span class="sxs-lookup"><span data-stu-id="4c865-115">Type</span></span> | <span data-ttu-id="4c865-116">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4c865-116">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="4c865-117">appId</span><span class="sxs-lookup"><span data-stu-id="4c865-117">appId</span></span>|<span data-ttu-id="4c865-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4c865-118">String</span></span>| <span data-ttu-id="4c865-119">Der eindeutige Bezeichner für die Anwendung.</span><span class="sxs-lookup"><span data-stu-id="4c865-119">The unique identifier for the application.</span></span> |
|<span data-ttu-id="4c865-120">permissionIds</span><span class="sxs-lookup"><span data-stu-id="4c865-120">permissionIds</span></span>|<span data-ttu-id="4c865-121">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="4c865-121">String collection</span></span>| <span data-ttu-id="4c865-122">Der eindeutige Bezeichner für die [PublishedPermissionScope](permissionscope.md) oder [AppRole](approle.md) die Anwendung erfordert.</span><span class="sxs-lookup"><span data-stu-id="4c865-122">The unique identifier for either the [publishedPermissionScope](permissionscope.md) or [appRole](approle.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4c865-123">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4c865-123">JSON representation</span></span>
<span data-ttu-id="4c865-124">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4c865-124">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/preauthorizedapplication.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
