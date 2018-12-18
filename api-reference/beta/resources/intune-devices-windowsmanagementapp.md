---
title: Ressourcentyp windowsManagementApp
description: Windows Management-app-Entität.
author: tfitzmac
ms.openlocfilehash: 641538644dc313234e27b0f518a26d8a38c612b7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346424"
---
# <a name="windowsmanagementapp-resource-type"></a><span data-ttu-id="b1a45-103">Ressourcentyp windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="b1a45-103">windowsManagementApp resource type</span></span>

> <span data-ttu-id="b1a45-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b1a45-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1a45-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b1a45-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1a45-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b1a45-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1a45-107">Windows Management-app-Entität.</span><span class="sxs-lookup"><span data-stu-id="b1a45-107">Windows management app entity.</span></span>
## <a name="methods"></a><span data-ttu-id="b1a45-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="b1a45-108">Methods</span></span>
|<span data-ttu-id="b1a45-109">Methode</span><span class="sxs-lookup"><span data-stu-id="b1a45-109">Method</span></span>|<span data-ttu-id="b1a45-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="b1a45-110">Return Type</span></span>|<span data-ttu-id="b1a45-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1a45-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b1a45-112">Abrufen von windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="b1a45-112">Get windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-get.md)|[<span data-ttu-id="b1a45-113">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="b1a45-113">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="b1a45-114">Lesen Sie Eigenschaften und Beziehungen des [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b1a45-114">Read properties and relationships of the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|
|[<span data-ttu-id="b1a45-115">WindowsManagementApp aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b1a45-115">Update windowsManagementApp</span></span>](../api/intune-devices-windowsmanagementapp-update.md)|[<span data-ttu-id="b1a45-116">windowsManagementApp</span><span class="sxs-lookup"><span data-stu-id="b1a45-116">windowsManagementApp</span></span>](../resources/intune-devices-windowsmanagementapp.md)|<span data-ttu-id="b1a45-117">Aktualisieren Sie die Eigenschaften eines [WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="b1a45-117">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b1a45-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b1a45-118">Properties</span></span>
|<span data-ttu-id="b1a45-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b1a45-119">Property</span></span>|<span data-ttu-id="b1a45-120">Typ</span><span class="sxs-lookup"><span data-stu-id="b1a45-120">Type</span></span>|<span data-ttu-id="b1a45-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1a45-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1a45-122">id</span><span class="sxs-lookup"><span data-stu-id="b1a45-122">id</span></span>|<span data-ttu-id="b1a45-123">String</span><span class="sxs-lookup"><span data-stu-id="b1a45-123">String</span></span>|<span data-ttu-id="b1a45-124">Eindeutiger Bezeichner für die Windows Management-app</span><span class="sxs-lookup"><span data-stu-id="b1a45-124">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="b1a45-125">availableVersion</span><span class="sxs-lookup"><span data-stu-id="b1a45-125">availableVersion</span></span>|<span data-ttu-id="b1a45-126">String</span><span class="sxs-lookup"><span data-stu-id="b1a45-126">String</span></span>|<span data-ttu-id="b1a45-127">Windows Management app verfügbare Version.</span><span class="sxs-lookup"><span data-stu-id="b1a45-127">Windows management app available version.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1a45-128">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b1a45-128">Relationships</span></span>
|<span data-ttu-id="b1a45-129">Beziehung</span><span class="sxs-lookup"><span data-stu-id="b1a45-129">Relationship</span></span>|<span data-ttu-id="b1a45-130">Typ</span><span class="sxs-lookup"><span data-stu-id="b1a45-130">Type</span></span>|<span data-ttu-id="b1a45-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b1a45-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1a45-132">healthSummary</span><span class="sxs-lookup"><span data-stu-id="b1a45-132">healthSummary</span></span>|[<span data-ttu-id="b1a45-133">windowsManagementAppHealthSummary</span><span class="sxs-lookup"><span data-stu-id="b1a45-133">windowsManagementAppHealthSummary</span></span>](../resources/intune-devices-windowsmanagementapphealthsummary.md)|<span data-ttu-id="b1a45-134">Zusammenfassung für Windows Management app Integrität.</span><span class="sxs-lookup"><span data-stu-id="b1a45-134">Health summary for Windows management app.</span></span>|
|<span data-ttu-id="b1a45-135">healthStates</span><span class="sxs-lookup"><span data-stu-id="b1a45-135">healthStates</span></span>|<span data-ttu-id="b1a45-136">[WindowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="b1a45-136">[windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) collection</span></span>|<span data-ttu-id="b1a45-137">Die Liste der Zustände für installierten Windows Management-Anwendung.</span><span class="sxs-lookup"><span data-stu-id="b1a45-137">The list of health states for installed Windows management app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b1a45-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b1a45-138">JSON Representation</span></span>
<span data-ttu-id="b1a45-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b1a45-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "String (identifier)",
  "availableVersion": "String"
}
```





