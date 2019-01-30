---
title: Ressourcentyp governancePermission
description: 'Stellt die Berechtigung, die ein GovernanceSubject hat für eine bestimmte GovernanceResource dar.  '
localization_priority: Normal
ms.openlocfilehash: 255cd4c25a957a40e5e5ac765ed446f516c51607
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643783"
---
# <a name="governancepermission-resource-type"></a><span data-ttu-id="055fb-103">Ressourcentyp governancePermission</span><span class="sxs-lookup"><span data-stu-id="055fb-103">governancePermission resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="055fb-104">Stellt die Berechtigung, die ein [GovernanceSubject](../resources/governancesubject.md) hat für eine bestimmte [GovernanceResource](../resources/governanceresource.md)dar.</span><span class="sxs-lookup"><span data-stu-id="055fb-104">Represents the access permission that a [governanceSubject](../resources/governancesubject.md) has to a specific [governanceResource](../resources/governanceresource.md).</span></span>  


## <a name="properties"></a><span data-ttu-id="055fb-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="055fb-105">Properties</span></span>
| <span data-ttu-id="055fb-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="055fb-106">Property</span></span>     | <span data-ttu-id="055fb-107">Typ</span><span class="sxs-lookup"><span data-stu-id="055fb-107">Type</span></span>   |<span data-ttu-id="055fb-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="055fb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="055fb-109">accessLevel</span><span class="sxs-lookup"><span data-stu-id="055fb-109">accessLevel</span></span>|<span data-ttu-id="055fb-110">String</span><span class="sxs-lookup"><span data-stu-id="055fb-110">String</span></span>|<span data-ttu-id="055fb-111">Die Zugriffsebene.</span><span class="sxs-lookup"><span data-stu-id="055fb-111">The access level.</span></span> <span data-ttu-id="055fb-112">Gültige Werte: ``None``, ``UserRead``, ``AdminRead``, und ``AdminReadWrite``.</span><span class="sxs-lookup"><span data-stu-id="055fb-112">Valid values: ``None``, ``UserRead``, ``AdminRead``, and ``AdminReadWrite``.</span></span>|
|<span data-ttu-id="055fb-113">isActive</span><span class="sxs-lookup"><span data-stu-id="055fb-113">isActive</span></span>|<span data-ttu-id="055fb-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="055fb-114">Boolean</span></span>|<span data-ttu-id="055fb-115">Gibt an, ob der anfordernden Person hat aktiven rollenzuweisung für die Zugriffsebene.</span><span class="sxs-lookup"><span data-stu-id="055fb-115">Indicate if the the requestor has any active role assignment for the access level.</span></span>|
|<span data-ttu-id="055fb-116">isEligible</span><span class="sxs-lookup"><span data-stu-id="055fb-116">isEligible</span></span>|<span data-ttu-id="055fb-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="055fb-117">Boolean</span></span>|<span data-ttu-id="055fb-118">Geben Sie an, ob der Requestor alle qualifizierten rollenzuweisung für die Zugriffsebene hat.</span><span class="sxs-lookup"><span data-stu-id="055fb-118">Indicate if the requestor has any eligible role assignment for the access level.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="055fb-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="055fb-119">JSON representation</span></span>

<span data-ttu-id="055fb-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="055fb-120">Here is a JSON representation of the resource.</span></span>

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancepermission.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
