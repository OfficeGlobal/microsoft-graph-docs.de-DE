---
title: managedAppStatus-Ressourcentyp
description: Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac7e2c727bce9da64e9262e3e3165a0bcc024623
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923712"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="4b058-103">managedAppStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="4b058-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="4b058-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4b058-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4b058-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4b058-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b058-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4b058-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b058-107">Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="4b058-107">Represents app protection and configuration status for the organization.</span></span>
## <a name="methods"></a><span data-ttu-id="4b058-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="4b058-108">Methods</span></span>
|<span data-ttu-id="4b058-109">Methode</span><span class="sxs-lookup"><span data-stu-id="4b058-109">Method</span></span>|<span data-ttu-id="4b058-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="4b058-110">Return Type</span></span>|<span data-ttu-id="4b058-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b058-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4b058-112">managedAppStatuses auflisten</span><span class="sxs-lookup"><span data-stu-id="4b058-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="4b058-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="4b058-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="4b058-114">Auflisten von Eigenschaften und Beziehungen der [managedAppStatus](../resources/intune-mam-managedappstatus.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="4b058-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="4b058-115">managedAppStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="4b058-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="4b058-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="4b058-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="4b058-117">Lesen von Eigenschaften und Beziehungen des [managedAppStatus](../resources/intune-mam-managedappstatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="4b058-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b058-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="4b058-118">Properties</span></span>
|<span data-ttu-id="4b058-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="4b058-119">Property</span></span>|<span data-ttu-id="4b058-120">Typ</span><span class="sxs-lookup"><span data-stu-id="4b058-120">Type</span></span>|<span data-ttu-id="4b058-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4b058-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b058-122">displayName</span><span class="sxs-lookup"><span data-stu-id="4b058-122">displayName</span></span>|<span data-ttu-id="4b058-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b058-123">String</span></span>|<span data-ttu-id="4b058-124">Anzeigename des Statusberichts</span><span class="sxs-lookup"><span data-stu-id="4b058-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="4b058-125">id</span><span class="sxs-lookup"><span data-stu-id="4b058-125">id</span></span>|<span data-ttu-id="4b058-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b058-126">String</span></span>|<span data-ttu-id="4b058-127">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="4b058-127">Key of the entity.</span></span>|
|<span data-ttu-id="4b058-128">Version</span><span class="sxs-lookup"><span data-stu-id="4b058-128">version</span></span>|<span data-ttu-id="4b058-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="4b058-129">String</span></span>|<span data-ttu-id="4b058-130">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="4b058-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b058-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="4b058-131">Relationships</span></span>
<span data-ttu-id="4b058-132">Keine</span><span class="sxs-lookup"><span data-stu-id="4b058-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b058-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="4b058-133">JSON Representation</span></span>
<span data-ttu-id="4b058-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="4b058-134">Here is a JSON representation of the resource.</span></span>
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





