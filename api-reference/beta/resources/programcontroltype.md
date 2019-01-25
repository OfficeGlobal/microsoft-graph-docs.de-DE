---
title: Ressourcentyp programControlType
description: 'In Azure AD Access Feature überprüft, der Steuerelementtyp Programm wird verwendet, wenn Zuordnen eines Steuerelements an ein Programm, den Typ des Access-Überprüfung an das Steuerelement ist.  '
localization_priority: Normal
ms.openlocfilehash: 8b17a0f30fbdceb6b6da24d5cbe972223acb29b0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519703"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="9546e-103">Ressourcentyp programControlType</span><span class="sxs-lookup"><span data-stu-id="9546e-103">programControlType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9546e-104">In der Azure AD [Access überprüft](accessreviews-root.md) -Funktion wird der Programm Steuerelementtyp verwendet, wenn zuordnen ein Steuerelements an ein Programm, um den Typ des Access-Überprüfung anzugeben, die für das Steuerelement ist.</span><span class="sxs-lookup"><span data-stu-id="9546e-104">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="9546e-105">Die Programm-Steuerelement Typ-Objekte werden automatisch generiert, wenn die Onboards globaler Administrator den Mandanten so verwenden Sie das Access Feature überprüft.</span><span class="sxs-lookup"><span data-stu-id="9546e-105">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="9546e-106">Keine zusätzliche Programm Steuerungstypen können erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="9546e-106">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="9546e-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="9546e-107">Methods</span></span>

| <span data-ttu-id="9546e-108">Methode</span><span class="sxs-lookup"><span data-stu-id="9546e-108">Method</span></span>           | <span data-ttu-id="9546e-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9546e-109">Return Type</span></span>    |<span data-ttu-id="9546e-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9546e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9546e-111">Liste programControlTypes</span><span class="sxs-lookup"><span data-stu-id="9546e-111">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="9546e-112">[ProgramControlType](programcontroltype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="9546e-112">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="9546e-113">Programm Steuerelement Listentypen.</span><span class="sxs-lookup"><span data-stu-id="9546e-113">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="9546e-114">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9546e-114">Properties</span></span>
| <span data-ttu-id="9546e-115">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9546e-115">Property</span></span>     | <span data-ttu-id="9546e-116">Typ</span><span class="sxs-lookup"><span data-stu-id="9546e-116">Type</span></span>   |<span data-ttu-id="9546e-117">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9546e-117">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="9546e-118">Das Feature zugewiesenen Bezeichner des Typs Programm</span><span class="sxs-lookup"><span data-stu-id="9546e-118">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="9546e-119">Der Name des Typs Programm</span><span class="sxs-lookup"><span data-stu-id="9546e-119">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="9546e-120">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9546e-120">Relationships</span></span>

<span data-ttu-id="9546e-121">Keine.</span><span class="sxs-lookup"><span data-stu-id="9546e-121">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="9546e-122">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="9546e-122">See also</span></span>

| <span data-ttu-id="9546e-123">Methode</span><span class="sxs-lookup"><span data-stu-id="9546e-123">Method</span></span>           | <span data-ttu-id="9546e-124">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9546e-124">Return Type</span></span>    |<span data-ttu-id="9546e-125">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9546e-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9546e-126">Erstellen von programControl</span><span class="sxs-lookup"><span data-stu-id="9546e-126">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="9546e-127">programControl</span><span class="sxs-lookup"><span data-stu-id="9546e-127">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="9546e-128">Fügen Sie ein Programm ein ProgramControl hinzu.</span><span class="sxs-lookup"><span data-stu-id="9546e-128">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="9546e-129">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9546e-129">JSON representation</span></span>

<span data-ttu-id="9546e-130">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9546e-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/programcontroltype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
