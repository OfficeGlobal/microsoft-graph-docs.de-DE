---
title: groupPolicyPresentation-Ressourcentyp
description: Die Basisentität für die Anzeige der zusätzlichen Optionen in einer Gruppenrichtlinien Definition.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d6abbcde241059a15969236b3ab7bcb0825d67d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166878"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="bc7be-103">groupPolicyPresentation-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="bc7be-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="bc7be-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bc7be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc7be-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="bc7be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc7be-106">Die Basisentität für die Anzeige der zusätzlichen Optionen in einer Gruppenrichtlinien Definition.</span><span class="sxs-lookup"><span data-stu-id="bc7be-106">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="bc7be-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="bc7be-107">Methods</span></span>
|<span data-ttu-id="bc7be-108">Methode</span><span class="sxs-lookup"><span data-stu-id="bc7be-108">Method</span></span>|<span data-ttu-id="bc7be-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="bc7be-109">Return Type</span></span>|<span data-ttu-id="bc7be-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc7be-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc7be-111">GroupPolicyPresentation abrufen</span><span class="sxs-lookup"><span data-stu-id="bc7be-111">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="bc7be-112">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="bc7be-112">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="bc7be-113">Lesen von Eigenschaften und Beziehungen des [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bc7be-113">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="bc7be-114">GroupPolicyPresentation aktualisieren</span><span class="sxs-lookup"><span data-stu-id="bc7be-114">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="bc7be-115">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="bc7be-115">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="bc7be-116">Aktualisieren der Eigenschaften eines [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="bc7be-116">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc7be-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bc7be-117">Properties</span></span>
|<span data-ttu-id="bc7be-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bc7be-118">Property</span></span>|<span data-ttu-id="bc7be-119">Typ</span><span class="sxs-lookup"><span data-stu-id="bc7be-119">Type</span></span>|<span data-ttu-id="bc7be-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc7be-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc7be-121">label</span><span class="sxs-lookup"><span data-stu-id="bc7be-121">label</span></span>|<span data-ttu-id="bc7be-122">String</span><span class="sxs-lookup"><span data-stu-id="bc7be-122">String</span></span>|<span data-ttu-id="bc7be-123">Lokalisierte Textbezeichnung für eine beliebige Präsentations Entität.</span><span class="sxs-lookup"><span data-stu-id="bc7be-123">Localized text label for any presentation entity.</span></span> <span data-ttu-id="bc7be-124">Der Standardwert ist Empty.</span><span class="sxs-lookup"><span data-stu-id="bc7be-124">The default value is empty.</span></span>|
|<span data-ttu-id="bc7be-125">id</span><span class="sxs-lookup"><span data-stu-id="bc7be-125">id</span></span>|<span data-ttu-id="bc7be-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="bc7be-126">String</span></span>|<span data-ttu-id="bc7be-127">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="bc7be-127">Key of the entity.</span></span>|
|<span data-ttu-id="bc7be-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bc7be-128">lastModifiedDateTime</span></span>|<span data-ttu-id="bc7be-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc7be-129">DateTimeOffset</span></span>|<span data-ttu-id="bc7be-130">Datum und Uhrzeit der letzten Änderung der Entität.</span><span class="sxs-lookup"><span data-stu-id="bc7be-130">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc7be-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bc7be-131">Relationships</span></span>
|<span data-ttu-id="bc7be-132">Beziehung</span><span class="sxs-lookup"><span data-stu-id="bc7be-132">Relationship</span></span>|<span data-ttu-id="bc7be-133">Typ</span><span class="sxs-lookup"><span data-stu-id="bc7be-133">Type</span></span>|<span data-ttu-id="bc7be-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bc7be-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc7be-135">definition</span><span class="sxs-lookup"><span data-stu-id="bc7be-135">definition</span></span>|[<span data-ttu-id="bc7be-136">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="bc7be-136">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="bc7be-137">Die der Präsentation zugeordnete Gruppenrichtlinien Definition.</span><span class="sxs-lookup"><span data-stu-id="bc7be-137">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc7be-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bc7be-138">JSON Representation</span></span>
<span data-ttu-id="bc7be-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bc7be-139">Here is a JSON representation of the resource.</span></span>
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




