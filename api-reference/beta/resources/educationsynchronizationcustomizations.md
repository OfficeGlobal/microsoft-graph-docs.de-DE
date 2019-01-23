---
title: Ressourcentyp educationSynchronizationCustomizations
description: Enthält die Liste der Entitäten, Synchronisierung und ihre Anpassungen an, sofern vorhanden.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 18b37276730286650e3fd75ad57a6b16e7917a04
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425960"
---
# <a name="educationsynchronizationcustomizations-resource-type"></a><span data-ttu-id="5531f-103">Ressourcentyp educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="5531f-103">educationSynchronizationCustomizations resource type</span></span>

> <span data-ttu-id="5531f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können geändert werden.</span><span class="sxs-lookup"><span data-stu-id="5531f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5531f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="5531f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5531f-106">Enthält die Liste der Entitäten, Synchronisierung und ihre [Anpassungen](educationsynchronizationcustomization.md), sofern vorhanden.</span><span class="sxs-lookup"><span data-stu-id="5531f-106">Contains the list of entities to sync and their [customizations](educationsynchronizationcustomization.md), if any.</span></span>

> <span data-ttu-id="5531f-107">**Hinweis:** Anpassung von Eigenschaften für die Synchronisierung gilt nicht für die **StudentEnrollment** und **TeacherRoster** -Entitäten.</span><span class="sxs-lookup"><span data-stu-id="5531f-107">**Note:** Customization of properties to sync does not apply to the **studentEnrollment** and **teacherRoster** entities.</span></span>

<span data-ttu-id="5531f-108">Diese Ressource ist Mitglied der folgenden Datenanbieter:</span><span class="sxs-lookup"><span data-stu-id="5531f-108">This resource is member of the following data providers:</span></span>

* [<span data-ttu-id="5531f-109">educationCsvDataProvider</span><span class="sxs-lookup"><span data-stu-id="5531f-109">educationCsvDataProvider</span></span>](educationcsvdataprovider.md)
* [<span data-ttu-id="5531f-110">educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="5531f-110">educationPowerSchoolDataProvider</span></span>](educationpowerschooldataprovider.md)

## <a name="properties"></a><span data-ttu-id="5531f-111">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="5531f-111">Properties</span></span>

| <span data-ttu-id="5531f-112">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="5531f-112">Property</span></span> | <span data-ttu-id="5531f-113">Typ</span><span class="sxs-lookup"><span data-stu-id="5531f-113">Type</span></span> | <span data-ttu-id="5531f-114">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="5531f-114">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="5531f-115">**School**</span><span class="sxs-lookup"><span data-stu-id="5531f-115">**school**</span></span> | [<span data-ttu-id="5531f-116">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="5531f-116">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="5531f-117">Anpassung für eine Schule Entität.</span><span class="sxs-lookup"><span data-stu-id="5531f-117">Customization for a school entity.</span></span>        |
| <span data-ttu-id="5531f-118">**section**</span><span class="sxs-lookup"><span data-stu-id="5531f-118">**section**</span></span> | [<span data-ttu-id="5531f-119">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="5531f-119">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="5531f-120">Anpassung für eine Entität im Abschnitt.</span><span class="sxs-lookup"><span data-stu-id="5531f-120">Customization for a section entity.</span></span>         |
| <span data-ttu-id="5531f-121">**student**</span><span class="sxs-lookup"><span data-stu-id="5531f-121">**student**</span></span> | [<span data-ttu-id="5531f-122">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="5531f-122">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="5531f-123">Anpassung für eine Student-Entität.</span><span class="sxs-lookup"><span data-stu-id="5531f-123">Customization for a student entity.</span></span>         |
| <span data-ttu-id="5531f-124">**teacher**</span><span class="sxs-lookup"><span data-stu-id="5531f-124">**teacher**</span></span> | [<span data-ttu-id="5531f-125">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="5531f-125">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="5531f-126">Anpassung für eine Entität Lehrer.</span><span class="sxs-lookup"><span data-stu-id="5531f-126">Customization for a teacher entity.</span></span>         |
| <span data-ttu-id="5531f-127">**studentEnrollment**</span><span class="sxs-lookup"><span data-stu-id="5531f-127">**studentEnrollment**</span></span> | [<span data-ttu-id="5531f-128">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="5531f-128">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |  <span data-ttu-id="5531f-129">Anpassung für die Student-Registrierung.</span><span class="sxs-lookup"><span data-stu-id="5531f-129">Customization for student enrollment.</span></span>           |
| <span data-ttu-id="5531f-130">**teacherRoster**</span><span class="sxs-lookup"><span data-stu-id="5531f-130">**teacherRoster**</span></span> | [<span data-ttu-id="5531f-131">educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="5531f-131">educationSynchronizationCustomization</span></span>](educationsynchronizationcustomization.md) |       <span data-ttu-id="5531f-132">Anpassung für eine Teilnehmerliste Lehrer.</span><span class="sxs-lookup"><span data-stu-id="5531f-132">Customization for a teacher roster.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="5531f-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="5531f-133">JSON representation</span></span>
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
