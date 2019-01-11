---
title: managedAppStatusRaw-Ressourcentyp
description: Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 975f43d064718b8457b40be707a54a0ea0eb69f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884014"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="df972-103">managedAppStatusRaw-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="df972-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="df972-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="df972-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df972-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="df972-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df972-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="df972-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df972-107">Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="df972-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="df972-108">Erbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="df972-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="df972-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="df972-109">Methods</span></span>
|<span data-ttu-id="df972-110">Methode</span><span class="sxs-lookup"><span data-stu-id="df972-110">Method</span></span>|<span data-ttu-id="df972-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="df972-111">Return Type</span></span>|<span data-ttu-id="df972-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df972-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="df972-113">managedAppStatusRaws auflisten</span><span class="sxs-lookup"><span data-stu-id="df972-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="df972-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="df972-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="df972-115">Auflisten von Eigenschaften und Beziehungen der [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="df972-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="df972-116">ManagedAppStatusRaw abrufen</span><span class="sxs-lookup"><span data-stu-id="df972-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="df972-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="df972-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="df972-118">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="df972-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="df972-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="df972-119">Properties</span></span>
|<span data-ttu-id="df972-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="df972-120">Property</span></span>|<span data-ttu-id="df972-121">Typ</span><span class="sxs-lookup"><span data-stu-id="df972-121">Type</span></span>|<span data-ttu-id="df972-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="df972-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df972-123">displayName</span><span class="sxs-lookup"><span data-stu-id="df972-123">displayName</span></span>|<span data-ttu-id="df972-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df972-124">String</span></span>|<span data-ttu-id="df972-125">Anzeigename des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="df972-125">Friendly name of the status report.</span></span> <span data-ttu-id="df972-126">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="df972-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="df972-127">id</span><span class="sxs-lookup"><span data-stu-id="df972-127">id</span></span>|<span data-ttu-id="df972-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df972-128">String</span></span>|<span data-ttu-id="df972-129">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="df972-129">Key of the entity.</span></span> <span data-ttu-id="df972-130">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="df972-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="df972-131">version</span><span class="sxs-lookup"><span data-stu-id="df972-131">version</span></span>|<span data-ttu-id="df972-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="df972-132">String</span></span>|<span data-ttu-id="df972-133">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="df972-133">Version of the entity.</span></span> <span data-ttu-id="df972-134">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="df972-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="df972-135">content</span><span class="sxs-lookup"><span data-stu-id="df972-135">content</span></span>|[<span data-ttu-id="df972-136">Json</span><span class="sxs-lookup"><span data-stu-id="df972-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="df972-137">Inhalt des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="df972-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df972-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="df972-138">Relationships</span></span>
<span data-ttu-id="df972-139">Keine</span><span class="sxs-lookup"><span data-stu-id="df972-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="df972-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="df972-140">JSON Representation</span></span>
<span data-ttu-id="df972-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="df972-141">Here is a JSON representation of the resource.</span></span>
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





