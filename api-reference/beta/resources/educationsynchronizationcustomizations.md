---
title: Ressourcentyp educationSynchronizationCustomizations
description: Enthält die Liste der Entitäten, Synchronisierung und ihre Anpassungen an, sofern vorhanden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9e513e64afb1478ca7b5cc5d53f1964d16d9928b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523253"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="6de77-103">Ressourcentyp educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="6de77-103">educationSynchronizationCustomizations resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6de77-104">Enthält die Liste der Entitäten, Synchronisierung und ihre [Anpassungen](educationsynchronizationcustomization.md), sofern vorhanden.</span><span class="sxs-lookup"><span data-stu-id="6de77-104">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="6de77-105">**Hinweis:** Anpassung von Eigenschaften für die Synchronisierung gilt nicht für die **StudentEnrollment** und **TeacherRoster** -Entitäten.</span><span class="sxs-lookup"><span data-stu-id="6de77-105">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="6de77-106">Diese Ressource ist Mitglied der folgenden Datenanbieter:</span><span class="sxs-lookup"><span data-stu-id="6de77-106">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="6de77-107">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="6de77-107">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="6de77-108">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="6de77-108">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="6de77-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6de77-109">Properties</span></span>

| <span data-ttu-id="6de77-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6de77-110">Property</span></span> | <span data-ttu-id="6de77-111">Typ</span><span class="sxs-lookup"><span data-stu-id="6de77-111">Type</span></span> | <span data-ttu-id="6de77-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6de77-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="6de77-113">**School**</span><span class="sxs-lookup"><span data-stu-id="6de77-113">**school**</span></span> | [<span data-ttu-id="6de77-114">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="6de77-114">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="6de77-115">Anpassung für eine Schule Entität.</span><span class="sxs-lookup"><span data-stu-id="6de77-115">Customization for a school entity.</span></span>        |
| <span data-ttu-id="6de77-116">**section**</span><span class="sxs-lookup"><span data-stu-id="6de77-116">**section**</span></span> | [<span data-ttu-id="6de77-117">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="6de77-117">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="6de77-118">Anpassung für eine Entität im Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="6de77-118">Customization for a section entity.</span></span>         |
| <span data-ttu-id="6de77-119">student</span><span class="sxs-lookup"><span data-stu-id="6de77-119">**student**</span></span> | [<span data-ttu-id="6de77-120">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="6de77-120">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="6de77-121">Anpassung für eine Student-Entität.</span><span class="sxs-lookup"><span data-stu-id="6de77-121">Customization for a student entity.</span></span>         |
| <span data-ttu-id="6de77-122">teacher</span><span class="sxs-lookup"><span data-stu-id="6de77-122">**teacher**</span></span> | [<span data-ttu-id="6de77-123">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="6de77-123">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="6de77-124">Anpassung für eine Entität Lehrer.</span><span class="sxs-lookup"><span data-stu-id="6de77-124">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="6de77-125">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="6de77-125">**studentEnrollment**</span></span> | [<span data-ttu-id="6de77-126">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="6de77-126">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="6de77-127">Anpassung für die Student-Registrierung.</span><span class="sxs-lookup"><span data-stu-id="6de77-127">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="6de77-128">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="6de77-128">**teacherRoster**</span></span> | [<span data-ttu-id="6de77-129">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="6de77-129">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="6de77-130">Anpassung für eine Teilnehmerliste Lehrer.</span><span class="sxs-lookup"><span data-stu-id="6de77-130">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="6de77-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6de77-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
}-->

```json
{
  "school": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "section": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "student": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacher": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "studentEnrollment": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"},
  "teacherRoster": {"@odata.type": "microsoft.graph.educationSynchronizationCustomization"}
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomizations.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
