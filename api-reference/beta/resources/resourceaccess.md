---
title: Ressourcentyp resourceAccess
description: Gibt ein Berechtigungsbereich OAuth 2.0 oder eine app-Rolle, die eine Anwendung funktioniert. Die **ResourceAccess** -Eigenschaft vom Typ RequiredResourceAccess ist eine Auflistung von **ResourceAccess**.
localization_priority: Normal
ms.openlocfilehash: f5389915897c3aab8b8277a45b54042bc861b290
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27862335"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="209b4-104">Ressourcentyp resourceAccess</span><span class="sxs-lookup"><span data-stu-id="209b4-104">resourceAccess resource type</span></span>

> <span data-ttu-id="209b4-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="209b4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="209b4-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="209b4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="209b4-107">Gibt ein Berechtigungsbereich OAuth 2.0 oder eine app-Rolle, die eine Anwendung funktioniert.</span><span class="sxs-lookup"><span data-stu-id="209b4-107">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="209b4-108">Die **ResourceAccess** -Eigenschaft vom Typ [RequiredResourceAccess](requiredresourceaccess.md) ist eine Auflistung von **ResourceAccess**.</span><span class="sxs-lookup"><span data-stu-id="209b4-108">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="209b4-109">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="209b4-109">JSON representation</span></span>

<span data-ttu-id="209b4-110">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="209b4-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="209b4-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="209b4-111">Properties</span></span>
| <span data-ttu-id="209b4-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="209b4-112">Property</span></span>     | <span data-ttu-id="209b4-113">Typ</span><span class="sxs-lookup"><span data-stu-id="209b4-113">Type</span></span>   |<span data-ttu-id="209b4-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="209b4-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="209b4-115">id</span><span class="sxs-lookup"><span data-stu-id="209b4-115">id</span></span>|<span data-ttu-id="209b4-116">Guid</span><span class="sxs-lookup"><span data-stu-id="209b4-116">Guid</span></span>|<span data-ttu-id="209b4-117">Der eindeutige Bezeichner für eine der [oAuth2Permission](oauth2permission.md) oder [AppRole](approle.md) -Instanzen, die die Anwendung für die Ressource verfügbar macht.</span><span class="sxs-lookup"><span data-stu-id="209b4-117">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="209b4-118">type</span><span class="sxs-lookup"><span data-stu-id="209b4-118">type</span></span>|<span data-ttu-id="209b4-119">String</span><span class="sxs-lookup"><span data-stu-id="209b4-119">String</span></span>|<span data-ttu-id="209b4-120">Gibt an, ob die **Id** -Eigenschaft ein [oAuth2Permission](oauth2permission.md) oder ein [AppRole](approle.md)verweist.</span><span class="sxs-lookup"><span data-stu-id="209b4-120">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="209b4-121">Mögliche Werte sind "Bereich" oder "Rolle".</span><span class="sxs-lookup"><span data-stu-id="209b4-121">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
