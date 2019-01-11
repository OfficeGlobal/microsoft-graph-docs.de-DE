---
title: Ressourcentyp programControlType
description: 'In Azure AD Access Feature überprüft, der Steuerelementtyp Programm wird verwendet, wenn Zuordnen eines Steuerelements an ein Programm, den Typ des Access-Überprüfung an das Steuerelement ist.  '
localization_priority: Normal
ms.openlocfilehash: 0091c23fd5d537e7c1fd62051778e56b510a3dab
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808232"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="98417-103">Ressourcentyp programControlType</span><span class="sxs-lookup"><span data-stu-id="98417-103">programControlType resource type</span></span>

> <span data-ttu-id="98417-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="98417-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98417-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="98417-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98417-106">In der Azure AD [Access überprüft](accessreviews-root.md) -Funktion wird der Programm Steuerelementtyp verwendet, wenn zuordnen ein Steuerelements an ein Programm, um den Typ des Access-Überprüfung anzugeben, die für das Steuerelement ist.</span><span class="sxs-lookup"><span data-stu-id="98417-106">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="98417-107">Die Programm-Steuerelement Typ-Objekte werden automatisch generiert, wenn die Onboards globaler Administrator den Mandanten so verwenden Sie das Access Feature überprüft.</span><span class="sxs-lookup"><span data-stu-id="98417-107">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="98417-108">Keine zusätzliche Programm Steuerungstypen können erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="98417-108">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="98417-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="98417-109">Methods</span></span>

| <span data-ttu-id="98417-110">Methode</span><span class="sxs-lookup"><span data-stu-id="98417-110">Method</span></span>           | <span data-ttu-id="98417-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="98417-111">Return Type</span></span>    |<span data-ttu-id="98417-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98417-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98417-113">Liste programControlTypes</span><span class="sxs-lookup"><span data-stu-id="98417-113">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="98417-114">[ProgramControlType](programcontroltype.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="98417-114">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="98417-115">Programm Steuerelement Listentypen.</span><span class="sxs-lookup"><span data-stu-id="98417-115">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="98417-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="98417-116">Properties</span></span>
| <span data-ttu-id="98417-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="98417-117">Property</span></span>     | <span data-ttu-id="98417-118">Typ</span><span class="sxs-lookup"><span data-stu-id="98417-118">Type</span></span>   |<span data-ttu-id="98417-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98417-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="98417-120">Das Feature zugewiesenen Bezeichner des Typs Programm</span><span class="sxs-lookup"><span data-stu-id="98417-120">The feature-assigned identifier of the program control type</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="98417-121">Der Name des Typs Programm</span><span class="sxs-lookup"><span data-stu-id="98417-121">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="98417-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="98417-122">Relationships</span></span>

<span data-ttu-id="98417-123">Keine.</span><span class="sxs-lookup"><span data-stu-id="98417-123">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="98417-124">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="98417-124">See also</span></span>

| <span data-ttu-id="98417-125">Methode</span><span class="sxs-lookup"><span data-stu-id="98417-125">Method</span></span>           | <span data-ttu-id="98417-126">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="98417-126">Return Type</span></span>    |<span data-ttu-id="98417-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="98417-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98417-128">Erstellen von programControl</span><span class="sxs-lookup"><span data-stu-id="98417-128">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="98417-129">programControl</span><span class="sxs-lookup"><span data-stu-id="98417-129">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="98417-130">Fügen Sie ein Programm ein ProgramControl hinzu.</span><span class="sxs-lookup"><span data-stu-id="98417-130">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="98417-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="98417-131">JSON representation</span></span>

<span data-ttu-id="98417-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="98417-132">Here is a JSON representation of the resource.</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
