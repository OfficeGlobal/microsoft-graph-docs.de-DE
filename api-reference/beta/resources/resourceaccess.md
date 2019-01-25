---
title: Ressourcentyp resourceAccess
description: Gibt ein Berechtigungsbereich OAuth 2.0 oder eine app-Rolle, die eine Anwendung funktioniert. Die **ResourceAccess** -Eigenschaft vom Typ RequiredResourceAccess ist eine Auflistung von **ResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: 1e741aa49e56b304c265a5fd701fdac37feb29dd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519024"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="de206-104">Ressourcentyp resourceAccess</span><span class="sxs-lookup"><span data-stu-id="de206-104">resourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de206-105">Gibt ein Berechtigungsbereich OAuth 2.0 oder eine app-Rolle, die eine Anwendung funktioniert.</span><span class="sxs-lookup"><span data-stu-id="de206-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="de206-106">Die **ResourceAccess** -Eigenschaft vom Typ [RequiredResourceAccess](requiredresourceaccess.md) ist eine Auflistung von **ResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="de206-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="de206-107">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="de206-107">JSON representation</span></span>

<span data-ttu-id="de206-108">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="de206-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="de206-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="de206-109">Properties</span></span>
| <span data-ttu-id="de206-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="de206-110">Property</span></span>     | <span data-ttu-id="de206-111">Typ</span><span class="sxs-lookup"><span data-stu-id="de206-111">Type</span></span>   |<span data-ttu-id="de206-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="de206-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de206-113">id</span><span class="sxs-lookup"><span data-stu-id="de206-113">id</span></span>|<span data-ttu-id="de206-114">Guid</span><span class="sxs-lookup"><span data-stu-id="de206-114">Guid</span></span>|<span data-ttu-id="de206-115">Der eindeutige Bezeichner für eine der [oAuth2Permission](oauth2permission.md) oder [AppRole](approle.md) -Instanzen, die die Anwendung für die Ressource verfügbar macht.</span><span class="sxs-lookup"><span data-stu-id="de206-115">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="de206-116">type</span><span class="sxs-lookup"><span data-stu-id="de206-116">type</span></span>|<span data-ttu-id="de206-117">String</span><span class="sxs-lookup"><span data-stu-id="de206-117">String</span></span>|<span data-ttu-id="de206-118">Gibt an, ob die **Id** -Eigenschaft ein [oAuth2Permission](oauth2permission.md) oder ein [AppRole](approle.md)verweist.</span><span class="sxs-lookup"><span data-stu-id="de206-118">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="de206-119">Mögliche Werte sind "Bereich" oder "Rolle".</span><span class="sxs-lookup"><span data-stu-id="de206-119">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
