---
title: managedAppStatus-Ressourcentyp
description: Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3bc6982161e204a4f2e5cac38b62d351ab417482
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258863"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="51bb5-103">managedAppStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="51bb5-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="51bb5-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="51bb5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51bb5-105">Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="51bb5-105">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="51bb5-106">Methoden</span><span class="sxs-lookup"><span data-stu-id="51bb5-106">Methods</span></span>
|<span data-ttu-id="51bb5-107">Methode</span><span class="sxs-lookup"><span data-stu-id="51bb5-107">Method</span></span>|<span data-ttu-id="51bb5-108">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="51bb5-108">Return Type</span></span>|<span data-ttu-id="51bb5-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51bb5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="51bb5-110">managedAppStatuses auflisten</span><span class="sxs-lookup"><span data-stu-id="51bb5-110">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="51bb5-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="51bb5-111">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="51bb5-112">Auflisten von Eigenschaften und Beziehungen der [managedAppStatus](../resources/intune-mam-managedappstatus.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="51bb5-112">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="51bb5-113">managedAppStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="51bb5-113">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="51bb5-114">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="51bb5-114">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="51bb5-115">Lesen von Eigenschaften und Beziehungen des [managedAppStatus](../resources/intune-mam-managedappstatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="51bb5-115">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="51bb5-116">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="51bb5-116">Properties</span></span>
|<span data-ttu-id="51bb5-117">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="51bb5-117">Property</span></span>|<span data-ttu-id="51bb5-118">Typ</span><span class="sxs-lookup"><span data-stu-id="51bb5-118">Type</span></span>|<span data-ttu-id="51bb5-119">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51bb5-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51bb5-120">displayName</span><span class="sxs-lookup"><span data-stu-id="51bb5-120">displayName</span></span>|<span data-ttu-id="51bb5-121">String</span><span class="sxs-lookup"><span data-stu-id="51bb5-121">String</span></span>|<span data-ttu-id="51bb5-122">Anzeigename des Statusberichts</span><span class="sxs-lookup"><span data-stu-id="51bb5-122">Friendly name of the status report.</span></span>|
|<span data-ttu-id="51bb5-123">id</span><span class="sxs-lookup"><span data-stu-id="51bb5-123">id</span></span>|<span data-ttu-id="51bb5-124">string</span><span class="sxs-lookup"><span data-stu-id="51bb5-124">String</span></span>|<span data-ttu-id="51bb5-125">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="51bb5-125">Key of the entity.</span></span>|
|<span data-ttu-id="51bb5-126">Version</span><span class="sxs-lookup"><span data-stu-id="51bb5-126">version</span></span>|<span data-ttu-id="51bb5-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="51bb5-127">String</span></span>|<span data-ttu-id="51bb5-128">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="51bb5-128">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51bb5-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="51bb5-129">Relationships</span></span>
<span data-ttu-id="51bb5-130">Keine</span><span class="sxs-lookup"><span data-stu-id="51bb5-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51bb5-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="51bb5-131">JSON Representation</span></span>
<span data-ttu-id="51bb5-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="51bb5-132">Here is a JSON representation of the resource.</span></span>
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



