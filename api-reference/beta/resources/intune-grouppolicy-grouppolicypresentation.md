---
title: Ressourcentyp groupPolicyPresentation
description: Die Basis Entität für die Präsentation Anzeigen aller die zusätzlichen Optionen in einer Gruppendefinition für die Richtlinie.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 736b599eaf310bc63530daa45ffa1aee7ede4c3f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430219"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="0e898-103">Ressourcentyp groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="0e898-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="0e898-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0e898-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0e898-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0e898-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e898-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e898-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e898-107">Die Basis Entität für die Präsentation Anzeigen aller die zusätzlichen Optionen in einer Gruppendefinition für die Richtlinie.</span><span class="sxs-lookup"><span data-stu-id="0e898-107">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="0e898-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="0e898-108">Methods</span></span>
|<span data-ttu-id="0e898-109">Methode</span><span class="sxs-lookup"><span data-stu-id="0e898-109">Method</span></span>|<span data-ttu-id="0e898-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="0e898-110">Return Type</span></span>|<span data-ttu-id="0e898-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e898-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0e898-112">Abrufen von groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="0e898-112">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="0e898-113">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="0e898-113">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="0e898-114">Lesen Sie Eigenschaften und Beziehungen des [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e898-114">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="0e898-115">GroupPolicyPresentation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0e898-115">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="0e898-116">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="0e898-116">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="0e898-117">Aktualisieren Sie die Eigenschaften eines [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="0e898-117">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e898-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0e898-118">Properties</span></span>
|<span data-ttu-id="0e898-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0e898-119">Property</span></span>|<span data-ttu-id="0e898-120">Typ</span><span class="sxs-lookup"><span data-stu-id="0e898-120">Type</span></span>|<span data-ttu-id="0e898-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e898-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e898-122">label</span><span class="sxs-lookup"><span data-stu-id="0e898-122">label</span></span>|<span data-ttu-id="0e898-123">String</span><span class="sxs-lookup"><span data-stu-id="0e898-123">String</span></span>|<span data-ttu-id="0e898-124">Lokalisierte Beschriftung für jede Entität Präsentation.</span><span class="sxs-lookup"><span data-stu-id="0e898-124">Localized text label for any presentation entity.</span></span> <span data-ttu-id="0e898-125">Der Standardwert ist leer.</span><span class="sxs-lookup"><span data-stu-id="0e898-125">The default value is empty.</span></span>|
|<span data-ttu-id="0e898-126">id</span><span class="sxs-lookup"><span data-stu-id="0e898-126">id</span></span>|<span data-ttu-id="0e898-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e898-127">String</span></span>|<span data-ttu-id="0e898-128">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="0e898-128">Key of the entity.</span></span>|
|<span data-ttu-id="0e898-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e898-129">lastModifiedDateTime</span></span>|<span data-ttu-id="0e898-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e898-130">DateTimeOffset</span></span>|<span data-ttu-id="0e898-131">Datum und Uhrzeit der letzten Änderung die Entität.</span><span class="sxs-lookup"><span data-stu-id="0e898-131">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e898-132">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0e898-132">Relationships</span></span>
|<span data-ttu-id="0e898-133">Beziehung</span><span class="sxs-lookup"><span data-stu-id="0e898-133">Relationship</span></span>|<span data-ttu-id="0e898-134">Typ</span><span class="sxs-lookup"><span data-stu-id="0e898-134">Type</span></span>|<span data-ttu-id="0e898-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e898-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e898-136">definition</span><span class="sxs-lookup"><span data-stu-id="0e898-136">definition</span></span>|[<span data-ttu-id="0e898-137">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="0e898-137">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="0e898-138">Die Gruppe Richtliniendefinition mit der Präsentation verknüpft ist.</span><span class="sxs-lookup"><span data-stu-id="0e898-138">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e898-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0e898-139">JSON Representation</span></span>
<span data-ttu-id="0e898-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0e898-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




