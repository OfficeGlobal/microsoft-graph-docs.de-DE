---
title: managedAppStatusRaw-Ressourcentyp
description: Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c89b36f7b9587a99d280de789dcaa753442591e9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253498"
---
# <a name="managedappstatusraw-resource-type"></a><span data-ttu-id="d50fb-103">managedAppStatusRaw-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d50fb-103">managedAppStatusRaw resource type</span></span>

> <span data-ttu-id="d50fb-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d50fb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d50fb-105">Stellt einen nicht typisierten Statusbericht über App-Schutz und -Konfiguration der Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="d50fb-105">Represents an un-typed status report about organizations app protection and configuration.</span></span>


<span data-ttu-id="d50fb-106">Erbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="d50fb-106">Inherits from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d50fb-107">Methoden</span><span class="sxs-lookup"><span data-stu-id="d50fb-107">Methods</span></span>
|<span data-ttu-id="d50fb-108">Methode</span><span class="sxs-lookup"><span data-stu-id="d50fb-108">Method</span></span>|<span data-ttu-id="d50fb-109">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="d50fb-109">Return Type</span></span>|<span data-ttu-id="d50fb-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d50fb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d50fb-111">managedAppStatusRaws auflisten</span><span class="sxs-lookup"><span data-stu-id="d50fb-111">List managedAppStatusRaws</span></span>](../api/intune-mam-managedappstatusraw-list.md)|<span data-ttu-id="d50fb-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="d50fb-112">[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) collection</span></span>|<span data-ttu-id="d50fb-113">Auflisten von Eigenschaften und Beziehungen der [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="d50fb-113">List properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) objects.</span></span>|
|[<span data-ttu-id="d50fb-114">ManagedAppStatusRaw abrufen</span><span class="sxs-lookup"><span data-stu-id="d50fb-114">Get managedAppStatusRaw</span></span>](../api/intune-mam-managedappstatusraw-get.md)|[<span data-ttu-id="d50fb-115">managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="d50fb-115">managedAppStatusRaw</span></span>](../resources/intune-mam-managedappstatusraw.md)|<span data-ttu-id="d50fb-116">Diese Methode liest die Eigenschaften und Beziehungen von Objekten des Typs [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).</span><span class="sxs-lookup"><span data-stu-id="d50fb-116">Read properties and relationships of the [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d50fb-117">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d50fb-117">Properties</span></span>
|<span data-ttu-id="d50fb-118">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d50fb-118">Property</span></span>|<span data-ttu-id="d50fb-119">Typ</span><span class="sxs-lookup"><span data-stu-id="d50fb-119">Type</span></span>|<span data-ttu-id="d50fb-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d50fb-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d50fb-121">displayName</span><span class="sxs-lookup"><span data-stu-id="d50fb-121">displayName</span></span>|<span data-ttu-id="d50fb-122">String</span><span class="sxs-lookup"><span data-stu-id="d50fb-122">String</span></span>|<span data-ttu-id="d50fb-123">Anzeigename des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="d50fb-123">Friendly name of the status report.</span></span> <span data-ttu-id="d50fb-124">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="d50fb-124">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="d50fb-125">id</span><span class="sxs-lookup"><span data-stu-id="d50fb-125">id</span></span>|<span data-ttu-id="d50fb-126">string</span><span class="sxs-lookup"><span data-stu-id="d50fb-126">String</span></span>|<span data-ttu-id="d50fb-127">Schlüssel der Entität.</span><span class="sxs-lookup"><span data-stu-id="d50fb-127">Key of the entity.</span></span> <span data-ttu-id="d50fb-128">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="d50fb-128">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="d50fb-129">version</span><span class="sxs-lookup"><span data-stu-id="d50fb-129">version</span></span>|<span data-ttu-id="d50fb-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d50fb-130">String</span></span>|<span data-ttu-id="d50fb-131">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="d50fb-131">Version of the entity.</span></span> <span data-ttu-id="d50fb-132">Geerbt von [managedAppStatus](../resources/intune-mam-managedappstatus.md).</span><span class="sxs-lookup"><span data-stu-id="d50fb-132">Inherited from [managedAppStatus](../resources/intune-mam-managedappstatus.md)</span></span>|
|<span data-ttu-id="d50fb-133">content</span><span class="sxs-lookup"><span data-stu-id="d50fb-133">content</span></span>|[<span data-ttu-id="d50fb-134">Json</span><span class="sxs-lookup"><span data-stu-id="d50fb-134">Json</span></span>](../resources/intune-mam-json.md)|<span data-ttu-id="d50fb-135">Inhalt des Statusberichts.</span><span class="sxs-lookup"><span data-stu-id="d50fb-135">Status report content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d50fb-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d50fb-136">Relationships</span></span>
<span data-ttu-id="d50fb-137">Keine</span><span class="sxs-lookup"><span data-stu-id="d50fb-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d50fb-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d50fb-138">JSON Representation</span></span>
<span data-ttu-id="d50fb-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d50fb-139">Here is a JSON representation of the resource.</span></span>
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



