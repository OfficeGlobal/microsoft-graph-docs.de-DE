---
title: managedAppStatusRaw-Ressourcentyp
description: Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 19c00f6d6bc1eb642320f77d9b5dfcc2fe842b1e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856854"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="da0f1-103">managedAppStatusRaw-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="da0f1-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="da0f1-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="da0f1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da0f1-105">Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="da0f1-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="da0f1-106">Erbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="da0f1-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="da0f1-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="da0f1-107">Methods</span></span>
|<span data-ttu-id="da0f1-108">Methode</span><span class="sxs-lookup"><span data-stu-id="da0f1-108">Method</span></span>|<span data-ttu-id="da0f1-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="da0f1-109">Return Type</span></span>|<span data-ttu-id="da0f1-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da0f1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="da0f1-111">managedAppStatusRaws auflisten</span><span class="sxs-lookup"><span data-stu-id="da0f1-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="da0f1-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="da0f1-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="da0f1-113">Auflisten von Eigenschaften und Beziehungen der [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="da0f1-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="da0f1-114">ManagedAppStatusRaw abrufen</span><span class="sxs-lookup"><span data-stu-id="da0f1-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="da0f1-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="da0f1-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="da0f1-116">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="da0f1-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="da0f1-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="da0f1-117">Properties</span></span>
|<span data-ttu-id="da0f1-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da0f1-118">Property</span></span>|<span data-ttu-id="da0f1-119">Typ</span><span class="sxs-lookup"><span data-stu-id="da0f1-119">Type</span></span>|<span data-ttu-id="da0f1-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da0f1-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da0f1-121">displayName</span><span class="sxs-lookup"><span data-stu-id="da0f1-121">displayName</span></span>|<span data-ttu-id="da0f1-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da0f1-122">String</span></span>|<span data-ttu-id="da0f1-123">Anzeigename des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="da0f1-123">Friendly name of the status report.</span></span> <span data-ttu-id="da0f1-124">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="da0f1-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="da0f1-125">id</span><span class="sxs-lookup"><span data-stu-id="da0f1-125">id</span></span>|<span data-ttu-id="da0f1-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da0f1-126">String</span></span>|<span data-ttu-id="da0f1-127">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="da0f1-127">Key of the entity.</span></span> <span data-ttu-id="da0f1-128">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="da0f1-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="da0f1-129">version</span><span class="sxs-lookup"><span data-stu-id="da0f1-129">version</span></span>|<span data-ttu-id="da0f1-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da0f1-130">String</span></span>|<span data-ttu-id="da0f1-131">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="da0f1-131">Version of the entity.</span></span> <span data-ttu-id="da0f1-132">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="da0f1-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="da0f1-133">content</span><span class="sxs-lookup"><span data-stu-id="da0f1-133">content</span></span>|[<span data-ttu-id="da0f1-134">Json</span><span class="sxs-lookup"><span data-stu-id="da0f1-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="da0f1-135">Inhalt des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="da0f1-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da0f1-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="da0f1-136">Relationships</span></span>
<span data-ttu-id="da0f1-137">Keine</span><span class="sxs-lookup"><span data-stu-id="da0f1-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="da0f1-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="da0f1-138">JSON Representation</span></span>
<span data-ttu-id="da0f1-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="da0f1-139">Here is a JSON representation of the resource.</span></span>
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



