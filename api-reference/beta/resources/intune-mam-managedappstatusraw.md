---
title: managedAppStatusRaw-Ressourcentyp
description: Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bfc7815e7f893294a72b88f67054702e1fb7347e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399262"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="8cd0e-103">managedAppStatusRaw-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="8cd0e-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="8cd0e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8cd0e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8cd0e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8cd0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8cd0e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8cd0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cd0e-107">Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="8cd0e-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="8cd0e-108">Erbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="8cd0e-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="8cd0e-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="8cd0e-109">Methods</span></span>
|<span data-ttu-id="8cd0e-110">Methode</span><span class="sxs-lookup"><span data-stu-id="8cd0e-110">Method</span></span>|<span data-ttu-id="8cd0e-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="8cd0e-111">Return Type</span></span>|<span data-ttu-id="8cd0e-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8cd0e-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8cd0e-113">managedAppStatusRaws auflisten</span><span class="sxs-lookup"><span data-stu-id="8cd0e-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="8cd0e-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="8cd0e-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="8cd0e-115">Auflisten von Eigenschaften und Beziehungen der [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="8cd0e-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="8cd0e-116">ManagedAppStatusRaw abrufen</span><span class="sxs-lookup"><span data-stu-id="8cd0e-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="8cd0e-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="8cd0e-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="8cd0e-118">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="8cd0e-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8cd0e-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8cd0e-119">Properties</span></span>
|<span data-ttu-id="8cd0e-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8cd0e-120">Property</span></span>|<span data-ttu-id="8cd0e-121">Typ</span><span class="sxs-lookup"><span data-stu-id="8cd0e-121">Type</span></span>|<span data-ttu-id="8cd0e-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8cd0e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cd0e-123">displayName</span><span class="sxs-lookup"><span data-stu-id="8cd0e-123">displayName</span></span>|<span data-ttu-id="8cd0e-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8cd0e-124">String</span></span>|<span data-ttu-id="8cd0e-125">Anzeigename des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="8cd0e-125">Friendly name of the status report.</span></span> <span data-ttu-id="8cd0e-126">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="8cd0e-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="8cd0e-127">id</span><span class="sxs-lookup"><span data-stu-id="8cd0e-127">id</span></span>|<span data-ttu-id="8cd0e-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8cd0e-128">String</span></span>|<span data-ttu-id="8cd0e-129">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="8cd0e-129">Key of the entity.</span></span> <span data-ttu-id="8cd0e-130">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="8cd0e-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="8cd0e-131">version</span><span class="sxs-lookup"><span data-stu-id="8cd0e-131">version</span></span>|<span data-ttu-id="8cd0e-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8cd0e-132">String</span></span>|<span data-ttu-id="8cd0e-133">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="8cd0e-133">Version of the entity.</span></span> <span data-ttu-id="8cd0e-134">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="8cd0e-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="8cd0e-135">content</span><span class="sxs-lookup"><span data-stu-id="8cd0e-135">content</span></span>|[<span data-ttu-id="8cd0e-136">Json</span><span class="sxs-lookup"><span data-stu-id="8cd0e-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="8cd0e-137">Inhalt des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="8cd0e-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cd0e-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8cd0e-138">Relationships</span></span>
<span data-ttu-id="8cd0e-139">Keine</span><span class="sxs-lookup"><span data-stu-id="8cd0e-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cd0e-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8cd0e-140">JSON Representation</span></span>
<span data-ttu-id="8cd0e-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8cd0e-141">Here is a JSON representation of the resource.</span></span>
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




