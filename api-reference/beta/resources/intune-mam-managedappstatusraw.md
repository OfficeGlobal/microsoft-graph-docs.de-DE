---
title: managedAppStatusRaw-Ressourcentyp
description: Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34c70a268c3940843759844c27de7f31bfab002e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30154194"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="95bc1-103">managedAppStatusRaw-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="95bc1-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="95bc1-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="95bc1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95bc1-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="95bc1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95bc1-106">Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="95bc1-106">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="95bc1-107">Erbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="95bc1-107">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="95bc1-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="95bc1-108">Methods</span></span>
|<span data-ttu-id="95bc1-109">Methode</span><span class="sxs-lookup"><span data-stu-id="95bc1-109">Method</span></span>|<span data-ttu-id="95bc1-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="95bc1-110">Return Type</span></span>|<span data-ttu-id="95bc1-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95bc1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="95bc1-112">managedAppStatusRaws auflisten</span><span class="sxs-lookup"><span data-stu-id="95bc1-112">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="95bc1-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="95bc1-113">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="95bc1-114">Auflisten von Eigenschaften und Beziehungen der [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="95bc1-114">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="95bc1-115">ManagedAppStatusRaw abrufen</span><span class="sxs-lookup"><span data-stu-id="95bc1-115">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="95bc1-116">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="95bc1-116">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="95bc1-117">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="95bc1-117">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="95bc1-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="95bc1-118">Properties</span></span>
|<span data-ttu-id="95bc1-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="95bc1-119">Property</span></span>|<span data-ttu-id="95bc1-120">Typ</span><span class="sxs-lookup"><span data-stu-id="95bc1-120">Type</span></span>|<span data-ttu-id="95bc1-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="95bc1-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95bc1-122">displayName</span><span class="sxs-lookup"><span data-stu-id="95bc1-122">displayName</span></span>|<span data-ttu-id="95bc1-123">String</span><span class="sxs-lookup"><span data-stu-id="95bc1-123">String</span></span>|<span data-ttu-id="95bc1-124">Anzeigename des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="95bc1-124">Friendly name of the status report.</span></span> <span data-ttu-id="95bc1-125">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="95bc1-125">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="95bc1-126">id</span><span class="sxs-lookup"><span data-stu-id="95bc1-126">id</span></span>|<span data-ttu-id="95bc1-127">string</span><span class="sxs-lookup"><span data-stu-id="95bc1-127">String</span></span>|<span data-ttu-id="95bc1-128">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="95bc1-128">Key of the entity.</span></span> <span data-ttu-id="95bc1-129">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="95bc1-129">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="95bc1-130">version</span><span class="sxs-lookup"><span data-stu-id="95bc1-130">version</span></span>|<span data-ttu-id="95bc1-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="95bc1-131">String</span></span>|<span data-ttu-id="95bc1-132">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="95bc1-132">Version of the entity.</span></span> <span data-ttu-id="95bc1-133">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="95bc1-133">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="95bc1-134">content</span><span class="sxs-lookup"><span data-stu-id="95bc1-134">content</span></span>|[<span data-ttu-id="95bc1-135">Json</span><span class="sxs-lookup"><span data-stu-id="95bc1-135">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="95bc1-136">Inhalt des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="95bc1-136">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95bc1-137">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="95bc1-137">Relationships</span></span>
<span data-ttu-id="95bc1-138">Keine</span><span class="sxs-lookup"><span data-stu-id="95bc1-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95bc1-139">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="95bc1-139">JSON Representation</span></span>
<span data-ttu-id="95bc1-140">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="95bc1-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```




