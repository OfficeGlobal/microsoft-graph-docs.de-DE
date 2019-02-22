---
title: managedAppStatus-Ressourcentyp
description: Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cc9f6596e9d9361a8c211809bf0f621fe36bcd4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153158"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="537fd-103">managedAppStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="537fd-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="537fd-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="537fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="537fd-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="537fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="537fd-106">Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="537fd-106">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="537fd-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="537fd-107">Methods</span></span>
|<span data-ttu-id="537fd-108">Methode</span><span class="sxs-lookup"><span data-stu-id="537fd-108">Method</span></span>|<span data-ttu-id="537fd-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="537fd-109">Return Type</span></span>|<span data-ttu-id="537fd-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="537fd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="537fd-111">managedAppStatuses auflisten</span><span class="sxs-lookup"><span data-stu-id="537fd-111">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="537fd-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="537fd-112">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="537fd-113">Auflisten von Eigenschaften und Beziehungen der [managedAppStatus](../resources/intune-mam-managedappstatus.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="537fd-113">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="537fd-114">managedAppStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="537fd-114">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="537fd-115">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="537fd-115">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="537fd-116">Lesen von Eigenschaften und Beziehungen des [managedAppStatus](../resources/intune-mam-managedappstatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="537fd-116">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="537fd-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="537fd-117">Properties</span></span>
|<span data-ttu-id="537fd-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="537fd-118">Property</span></span>|<span data-ttu-id="537fd-119">Typ</span><span class="sxs-lookup"><span data-stu-id="537fd-119">Type</span></span>|<span data-ttu-id="537fd-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="537fd-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="537fd-121">displayName</span><span class="sxs-lookup"><span data-stu-id="537fd-121">displayName</span></span>|<span data-ttu-id="537fd-122">String</span><span class="sxs-lookup"><span data-stu-id="537fd-122">String</span></span>|<span data-ttu-id="537fd-123">Anzeigename des Statusberichts</span><span class="sxs-lookup"><span data-stu-id="537fd-123">Friendly name of the status report.</span></span>|
|<span data-ttu-id="537fd-124">id</span><span class="sxs-lookup"><span data-stu-id="537fd-124">id</span></span>|<span data-ttu-id="537fd-125">string</span><span class="sxs-lookup"><span data-stu-id="537fd-125">String</span></span>|<span data-ttu-id="537fd-126">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="537fd-126">Key of the entity.</span></span>|
|<span data-ttu-id="537fd-127">Version</span><span class="sxs-lookup"><span data-stu-id="537fd-127">version</span></span>|<span data-ttu-id="537fd-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="537fd-128">String</span></span>|<span data-ttu-id="537fd-129">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="537fd-129">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="537fd-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="537fd-130">Relationships</span></span>
<span data-ttu-id="537fd-131">Keine</span><span class="sxs-lookup"><span data-stu-id="537fd-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="537fd-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="537fd-132">JSON Representation</span></span>
<span data-ttu-id="537fd-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="537fd-133">Here is a JSON representation of the resource.</span></span>
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




