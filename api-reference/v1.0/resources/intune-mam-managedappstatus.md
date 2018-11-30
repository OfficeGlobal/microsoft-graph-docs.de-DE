---
title: managedAppStatus-Ressourcentyp
description: Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.
ms.openlocfilehash: d25770468341e1f62e96273c6c925d322b385c89
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018381"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="9ad26-103">managedAppStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="9ad26-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="9ad26-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9ad26-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ad26-105">Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="9ad26-105">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="9ad26-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="9ad26-106">Methods</span></span>
|<span data-ttu-id="9ad26-107">Methode</span><span class="sxs-lookup"><span data-stu-id="9ad26-107">Method</span></span>|<span data-ttu-id="9ad26-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="9ad26-108">Return Type</span></span>|<span data-ttu-id="9ad26-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ad26-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ad26-110">managedAppStatuses auflisten</span><span class="sxs-lookup"><span data-stu-id="9ad26-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="9ad26-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="9ad26-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="9ad26-112">Auflisten von Eigenschaften und Beziehungen der [managedAppStatus](../resources/intune-mam-managedappstatus.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="9ad26-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="9ad26-113">managedAppStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="9ad26-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="9ad26-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="9ad26-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="9ad26-115">Lesen von Eigenschaften und Beziehungen des [managedAppStatus](../resources/intune-mam-managedappstatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="9ad26-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ad26-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="9ad26-116">Properties</span></span>
|<span data-ttu-id="9ad26-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="9ad26-117">Property</span></span>|<span data-ttu-id="9ad26-118">Typ</span><span class="sxs-lookup"><span data-stu-id="9ad26-118">Type</span></span>|<span data-ttu-id="9ad26-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9ad26-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ad26-120">displayName</span><span class="sxs-lookup"><span data-stu-id="9ad26-120">displayName</span></span>|<span data-ttu-id="9ad26-121">String</span><span class="sxs-lookup"><span data-stu-id="9ad26-121">String</span></span>|<span data-ttu-id="9ad26-122">Anzeigename des Statusberichts</span><span class="sxs-lookup"><span data-stu-id="9ad26-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="9ad26-123">id</span><span class="sxs-lookup"><span data-stu-id="9ad26-123">id</span></span>|<span data-ttu-id="9ad26-124">String</span><span class="sxs-lookup"><span data-stu-id="9ad26-124">String</span></span>|<span data-ttu-id="9ad26-125">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="9ad26-125">Key of the entity.</span></span>|
|<span data-ttu-id="9ad26-126">Version</span><span class="sxs-lookup"><span data-stu-id="9ad26-126">version</span></span>|<span data-ttu-id="9ad26-127">String</span><span class="sxs-lookup"><span data-stu-id="9ad26-127">String</span></span>|<span data-ttu-id="9ad26-128">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="9ad26-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ad26-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="9ad26-129">Relationships</span></span>
<span data-ttu-id="9ad26-130">Keine</span><span class="sxs-lookup"><span data-stu-id="9ad26-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ad26-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="9ad26-131">JSON Representation</span></span>
<span data-ttu-id="9ad26-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="9ad26-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```


