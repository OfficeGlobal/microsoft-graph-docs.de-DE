---
title: Ressourcentyp businessFlowTemplate
description: In Azure AD Access Feature, überprüft die `businesFlowTemplate` stellt eine Azure AD Business Flow-Vorlage. Der Bezeichner der Vorlage, beispielsweise zum Überprüfen der Gast Mitglieder einer Gruppe ist vom Anrufer bereitgestellt wird, wenn eine Überprüfung Access erstellen.
ms.openlocfilehash: 8faf1a1381f5cdcf4bfaab78adc7a6554479b427
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27064878"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="b3ee7-104">Ressourcentyp businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="b3ee7-104">businessFlowTemplate resource type</span></span>

> <span data-ttu-id="b3ee7-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b3ee7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3ee7-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b3ee7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3ee7-107">In der Azure AD [Access überprüft](accessreviews-root.md) -Funktion die `businesFlowTemplate` stellt eine Azure AD Business Flow-Vorlage.</span><span class="sxs-lookup"><span data-stu-id="b3ee7-107">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="b3ee7-108">Der Bezeichner der Vorlage, beispielsweise zum Überprüfen der Gast Mitglieder einer Gruppe ist vom Anrufer bereitgestellt wird, wenn eine Überprüfung Access erstellen.</span><span class="sxs-lookup"><span data-stu-id="b3ee7-108">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="b3ee7-109">Der Fluss Vorlage Geschäftsobjekte sind automatisch generiert, wenn die Onboards globaler Administrator den Mandanten so verwenden Sie das Access Feature überprüft.</span><span class="sxs-lookup"><span data-stu-id="b3ee7-109">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="b3ee7-110">Keine zusätzliche Business Fluss Vorlagen können erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="b3ee7-110">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="b3ee7-111">Methoden</span><span class="sxs-lookup"><span data-stu-id="b3ee7-111">Methods</span></span>

| <span data-ttu-id="b3ee7-112">Methode</span><span class="sxs-lookup"><span data-stu-id="b3ee7-112">Method</span></span>           | <span data-ttu-id="b3ee7-113">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b3ee7-113">Return Type</span></span>    |<span data-ttu-id="b3ee7-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3ee7-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b3ee7-115">Liste businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="b3ee7-115">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="b3ee7-116">[BusinessFlowTemplate](businessflowtemplate.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b3ee7-116">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="b3ee7-117">Rufen Sie die Vorlagen für Unternehmen Fluss Bewertungen Zugriff auf entsprechende.</span><span class="sxs-lookup"><span data-stu-id="b3ee7-117">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="b3ee7-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b3ee7-118">Properties</span></span>
| <span data-ttu-id="b3ee7-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b3ee7-119">Property</span></span>     | <span data-ttu-id="b3ee7-120">Typ</span><span class="sxs-lookup"><span data-stu-id="b3ee7-120">Type</span></span>   |<span data-ttu-id="b3ee7-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3ee7-121">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="b3ee7-122">Das Feature zugewiesene Bezeichner der Vorlage Fluss business</span><span class="sxs-lookup"><span data-stu-id="b3ee7-122">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="b3ee7-123">Der Name der Vorlage Fluss business</span><span class="sxs-lookup"><span data-stu-id="b3ee7-123">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="b3ee7-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b3ee7-124">Relationships</span></span>

<span data-ttu-id="b3ee7-125">Keine.</span><span class="sxs-lookup"><span data-stu-id="b3ee7-125">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="b3ee7-126">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="b3ee7-126">See also</span></span>

| <span data-ttu-id="b3ee7-127">Methode</span><span class="sxs-lookup"><span data-stu-id="b3ee7-127">Method</span></span>           | <span data-ttu-id="b3ee7-128">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b3ee7-128">Return Type</span></span>    |<span data-ttu-id="b3ee7-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b3ee7-129">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b3ee7-130">Erstellen von accessReview</span><span class="sxs-lookup"><span data-stu-id="b3ee7-130">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="b3ee7-131">accessReview</span><span class="sxs-lookup"><span data-stu-id="b3ee7-131">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="b3ee7-132">Erstellen Sie eine neue AccessReview.</span><span class="sxs-lookup"><span data-stu-id="b3ee7-132">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="b3ee7-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b3ee7-133">JSON representation</span></span>

<span data-ttu-id="b3ee7-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b3ee7-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.businessFlowTemplate"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
