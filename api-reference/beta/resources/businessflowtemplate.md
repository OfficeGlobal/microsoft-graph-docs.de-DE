---
title: Ressourcentyp businessFlowTemplate
description: In Azure AD Access Feature, überprüft die `businesFlowTemplate` stellt eine Azure AD Business Flow-Vorlage. Der Bezeichner der Vorlage, beispielsweise zum Überprüfen der Gast Mitglieder einer Gruppe ist vom Anrufer bereitgestellt wird, wenn eine Überprüfung Access erstellen.
localization_priority: Normal
ms.openlocfilehash: 567a7f499e2fb493f3ca519e312e69fb43fe3b79
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529579"
---
# <a name="businessflowtemplate-resource-type"></a><span data-ttu-id="da353-104">Ressourcentyp businessFlowTemplate</span><span class="sxs-lookup"><span data-stu-id="da353-104">businessFlowTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da353-105">In der Azure AD [Access überprüft](accessreviews-root.md) -Funktion die `businesFlowTemplate` stellt eine Azure AD Business Flow-Vorlage.</span><span class="sxs-lookup"><span data-stu-id="da353-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the `businesFlowTemplate` represents an Azure AD business flow template.</span></span> <span data-ttu-id="da353-106">Der Bezeichner der Vorlage, beispielsweise zum Überprüfen der Gast Mitglieder einer Gruppe ist vom Anrufer bereitgestellt wird, wenn eine Überprüfung Access erstellen.</span><span class="sxs-lookup"><span data-stu-id="da353-106">The identifier of a template, such as to review guest members of a group, is supplied by the caller when creating an access review.</span></span>

<span data-ttu-id="da353-107">Der Fluss Vorlage Geschäftsobjekte sind automatisch generiert, wenn die Onboards globaler Administrator den Mandanten so verwenden Sie das Access Feature überprüft.</span><span class="sxs-lookup"><span data-stu-id="da353-107">The business flow template objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="da353-108">Keine zusätzliche Business Fluss Vorlagen können erstellt werden.</span><span class="sxs-lookup"><span data-stu-id="da353-108">No additional business flow templates can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="da353-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="da353-109">Methods</span></span>

| <span data-ttu-id="da353-110">Methode</span><span class="sxs-lookup"><span data-stu-id="da353-110">Method</span></span>           | <span data-ttu-id="da353-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="da353-111">Return Type</span></span>    |<span data-ttu-id="da353-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da353-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da353-113">Liste businessFlowTemplates</span><span class="sxs-lookup"><span data-stu-id="da353-113">List businessFlowTemplates</span></span>](../api/businessflowtemplate-list.md) | <span data-ttu-id="da353-114">[BusinessFlowTemplate](businessflowtemplate.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="da353-114">[businessFlowTemplate](businessflowtemplate.md) collection</span></span>| <span data-ttu-id="da353-115">Rufen Sie die Vorlagen für Unternehmen Fluss Bewertungen Zugriff auf entsprechende.</span><span class="sxs-lookup"><span data-stu-id="da353-115">Get the business flow templates appropriate to access reviews.</span></span>|

## <a name="properties"></a><span data-ttu-id="da353-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="da353-116">Properties</span></span>
| <span data-ttu-id="da353-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da353-117">Property</span></span>     | <span data-ttu-id="da353-118">Typ</span><span class="sxs-lookup"><span data-stu-id="da353-118">Type</span></span>   |<span data-ttu-id="da353-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da353-119">Description</span></span>|
|:---------------|:--------|:----------|
| `id`                     |`String`                | <span data-ttu-id="da353-120">Das Feature zugewiesene Bezeichner der Vorlage Fluss business</span><span class="sxs-lookup"><span data-stu-id="da353-120">The feature-assigned identifier of the business flow template</span></span>                                      |
| `displayName`            |`String`                | <span data-ttu-id="da353-121">Der Name der Vorlage Fluss business</span><span class="sxs-lookup"><span data-stu-id="da353-121">The name of the business flow template</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="da353-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="da353-122">Relationships</span></span>

<span data-ttu-id="da353-123">Keine.</span><span class="sxs-lookup"><span data-stu-id="da353-123">None.</span></span>

## <a name="see-also"></a><span data-ttu-id="da353-124">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="da353-124">See also</span></span>

| <span data-ttu-id="da353-125">Methode</span><span class="sxs-lookup"><span data-stu-id="da353-125">Method</span></span>           | <span data-ttu-id="da353-126">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="da353-126">Return Type</span></span>    |<span data-ttu-id="da353-127">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da353-127">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="da353-128">Erstellen von accessReview</span><span class="sxs-lookup"><span data-stu-id="da353-128">Create accessReview</span></span>](../api/accessreview-create.md) | [<span data-ttu-id="da353-129">accessReview</span><span class="sxs-lookup"><span data-stu-id="da353-129">accessReview</span></span>](accessreview.md) |   <span data-ttu-id="da353-130">Erstellen Sie eine neue AccessReview.</span><span class="sxs-lookup"><span data-stu-id="da353-130">Create a new accessReview.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="da353-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="da353-131">JSON representation</span></span>

<span data-ttu-id="da353-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="da353-132">Here is a JSON representation of the resource.</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "businessFlowTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/businessflowtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
