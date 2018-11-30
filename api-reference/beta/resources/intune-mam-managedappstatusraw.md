---
title: managedAppStatusRaw-Ressourcentyp
description: Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.
ms.openlocfilehash: ba2f398e54e27cb079dd575530d46a7bf287722d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058449"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="52d4b-103">managedAppStatusRaw-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="52d4b-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="52d4b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="52d4b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52d4b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="52d4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52d4b-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="52d4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52d4b-107">Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="52d4b-107">Represents an un-typed status report about organizations app protection and configuration.</span></span>

<span data-ttu-id="52d4b-108">Erbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="52d4b-108">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="52d4b-109">Methoden</span><span class="sxs-lookup"><span data-stu-id="52d4b-109">Methods</span></span>
|<span data-ttu-id="52d4b-110">Methode</span><span class="sxs-lookup"><span data-stu-id="52d4b-110">Method</span></span>|<span data-ttu-id="52d4b-111">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="52d4b-111">Return Type</span></span>|<span data-ttu-id="52d4b-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52d4b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="52d4b-113">managedAppStatusRaws auflisten</span><span class="sxs-lookup"><span data-stu-id="52d4b-113">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="52d4b-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="52d4b-114">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="52d4b-115">Auflisten von Eigenschaften und Beziehungen der [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="52d4b-115">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="52d4b-116">ManagedAppStatusRaw abrufen</span><span class="sxs-lookup"><span data-stu-id="52d4b-116">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="52d4b-117">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="52d4b-117">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="52d4b-118">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="52d4b-118">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="52d4b-119">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="52d4b-119">Properties</span></span>
|<span data-ttu-id="52d4b-120">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="52d4b-120">Property</span></span>|<span data-ttu-id="52d4b-121">Typ</span><span class="sxs-lookup"><span data-stu-id="52d4b-121">Type</span></span>|<span data-ttu-id="52d4b-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52d4b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52d4b-123">displayName</span><span class="sxs-lookup"><span data-stu-id="52d4b-123">displayName</span></span>|<span data-ttu-id="52d4b-124">String</span><span class="sxs-lookup"><span data-stu-id="52d4b-124">String</span></span>|<span data-ttu-id="52d4b-125">Anzeigename des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="52d4b-125">Friendly name of the status report.</span></span> <span data-ttu-id="52d4b-126">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="52d4b-126">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="52d4b-127">id</span><span class="sxs-lookup"><span data-stu-id="52d4b-127">id</span></span>|<span data-ttu-id="52d4b-128">String</span><span class="sxs-lookup"><span data-stu-id="52d4b-128">String</span></span>|<span data-ttu-id="52d4b-129">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="52d4b-129">Key of the entity.</span></span> <span data-ttu-id="52d4b-130">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="52d4b-130">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="52d4b-131">version</span><span class="sxs-lookup"><span data-stu-id="52d4b-131">version</span></span>|<span data-ttu-id="52d4b-132">String</span><span class="sxs-lookup"><span data-stu-id="52d4b-132">String</span></span>|<span data-ttu-id="52d4b-133">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="52d4b-133">Version of the entity.</span></span> <span data-ttu-id="52d4b-134">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="52d4b-134">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="52d4b-135">content</span><span class="sxs-lookup"><span data-stu-id="52d4b-135">content</span></span>|[<span data-ttu-id="52d4b-136">Json</span><span class="sxs-lookup"><span data-stu-id="52d4b-136">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="52d4b-137">Inhalt des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="52d4b-137">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52d4b-138">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="52d4b-138">Relationships</span></span>
<span data-ttu-id="52d4b-139">Keine</span><span class="sxs-lookup"><span data-stu-id="52d4b-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="52d4b-140">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="52d4b-140">JSON Representation</span></span>
<span data-ttu-id="52d4b-141">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="52d4b-141">Here is a JSON representation of the resource.</span></span>
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





