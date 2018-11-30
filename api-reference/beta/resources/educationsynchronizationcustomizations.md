---
title: Ressourcentyp educationSynchronizationCustomizations
description: Enthält die Liste der Entitäten, Synchronisierung und ihre Anpassungen an, sofern vorhanden.
ms.openlocfilehash: d694c5ea1136d38e11ff3f1aca0ad0fde34b9d02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062407"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="15102-103">Ressourcentyp educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="15102-103">educationSynchronizationCustomizations resource type</span></span>

> <span data-ttu-id="15102-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="15102-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15102-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="15102-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="15102-106">Enthält die Liste der Entitäten, Synchronisierung und ihre [Anpassungen](educationsynchronizationcustomization.md), sofern vorhanden.</span><span class="sxs-lookup"><span data-stu-id="15102-106">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="15102-107">**Hinweis:** Anpassung von Eigenschaften für die Synchronisierung gilt nicht für die **StudentEnrollment** und **TeacherRoster** -Entitäten.</span><span class="sxs-lookup"><span data-stu-id="15102-107">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="15102-108">Diese Ressource ist Mitglied der folgenden Datenanbieter:</span><span class="sxs-lookup"><span data-stu-id="15102-108">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="15102-109">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="15102-109">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="15102-110">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="15102-110">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="15102-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="15102-111">Properties</span></span>

| <span data-ttu-id="15102-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="15102-112">Property</span></span> | <span data-ttu-id="15102-113">Typ</span><span class="sxs-lookup"><span data-stu-id="15102-113">Type</span></span> | <span data-ttu-id="15102-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15102-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="15102-115">**School**</span><span class="sxs-lookup"><span data-stu-id="15102-115">**school**</span></span> | [<span data-ttu-id="15102-116">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="15102-116">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="15102-117">Anpassung für eine Schule Entität.</span><span class="sxs-lookup"><span data-stu-id="15102-117">Customization for a school entity.</span></span>        |
| <span data-ttu-id="15102-118">**section**</span><span class="sxs-lookup"><span data-stu-id="15102-118">**section**</span></span> | [<span data-ttu-id="15102-119">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="15102-119">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="15102-120">Anpassung für eine Entität im Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="15102-120">Customization for a section entity.</span></span>         |
| <span data-ttu-id="15102-121">**student**</span><span class="sxs-lookup"><span data-stu-id="15102-121">**student**</span></span> | [<span data-ttu-id="15102-122">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="15102-122">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="15102-123">Anpassung für eine Student-Entität.</span><span class="sxs-lookup"><span data-stu-id="15102-123">Customization for a student entity.</span></span>         |
| <span data-ttu-id="15102-124">**teacher**</span><span class="sxs-lookup"><span data-stu-id="15102-124">**teacher**</span></span> | [<span data-ttu-id="15102-125">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="15102-125">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="15102-126">Anpassung für eine Entität Lehrer.</span><span class="sxs-lookup"><span data-stu-id="15102-126">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="15102-127">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="15102-127">**studentEnrollment**</span></span> | [<span data-ttu-id="15102-128">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="15102-128">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="15102-129">Anpassung für die Student-Registrierung.</span><span class="sxs-lookup"><span data-stu-id="15102-129">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="15102-130">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="15102-130">**teacherRoster**</span></span> | [<span data-ttu-id="15102-131">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="15102-131">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="15102-132">Anpassung für eine Teilnehmerliste Lehrer.</span><span class="sxs-lookup"><span data-stu-id="15102-132">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="15102-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="15102-133">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomizations"
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
