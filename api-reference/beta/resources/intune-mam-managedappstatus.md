---
title: managedAppStatus-Ressourcentyp
description: Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7625543106b1ccf019df9622c1b0f37d40232f0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415565"
---
# <a name="managedappstatus-resource-type"></a><span data-ttu-id="ee34f-103">managedAppStatus-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="ee34f-103">managedAppStatus resource type</span></span>

> <span data-ttu-id="ee34f-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="ee34f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee34f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ee34f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee34f-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ee34f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee34f-107">Stellt den App-Schutz und den Konfigurationsstatus für die Organisation dar.</span><span class="sxs-lookup"><span data-stu-id="ee34f-107">Represents app protection and configuration status for the organization.</span></span>

## <a name="methods"></a><span data-ttu-id="ee34f-108">Methoden</span><span class="sxs-lookup"><span data-stu-id="ee34f-108">Methods</span></span>
|<span data-ttu-id="ee34f-109">Methode</span><span class="sxs-lookup"><span data-stu-id="ee34f-109">Method</span></span>|<span data-ttu-id="ee34f-110">Rückgabetyp</span><span class="sxs-lookup"><span data-stu-id="ee34f-110">Return Type</span></span>|<span data-ttu-id="ee34f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee34f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ee34f-112">managedAppStatuses auflisten</span><span class="sxs-lookup"><span data-stu-id="ee34f-112">List managedAppStatuses</span></span>](../api/intune-mam-managedappstatus-list.md)|<span data-ttu-id="ee34f-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md)-Sammlung</span><span class="sxs-lookup"><span data-stu-id="ee34f-113">[managedAppStatus](../resources/intune-mam-managedappstatus.md) collection</span></span>|<span data-ttu-id="ee34f-114">Auflisten von Eigenschaften und Beziehungen der [managedAppStatus](../resources/intune-mam-managedappstatus.md)-Objekte.</span><span class="sxs-lookup"><span data-stu-id="ee34f-114">List properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) objects.</span></span>|
|[<span data-ttu-id="ee34f-115">managedAppStatus abrufen</span><span class="sxs-lookup"><span data-stu-id="ee34f-115">Get managedAppStatus</span></span>](../api/intune-mam-managedappstatus-get.md)|[<span data-ttu-id="ee34f-116">managedAppStatus</span><span class="sxs-lookup"><span data-stu-id="ee34f-116">managedAppStatus</span></span>](../resources/intune-mam-managedappstatus.md)|<span data-ttu-id="ee34f-117">Lesen von Eigenschaften und Beziehungen des [managedAppStatus](../resources/intune-mam-managedappstatus.md)-Objekts.</span><span class="sxs-lookup"><span data-stu-id="ee34f-117">Read properties and relationships of the [managedAppStatus](../resources/intune-mam-managedappstatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ee34f-118">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="ee34f-118">Properties</span></span>
|<span data-ttu-id="ee34f-119">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ee34f-119">Property</span></span>|<span data-ttu-id="ee34f-120">Typ</span><span class="sxs-lookup"><span data-stu-id="ee34f-120">Type</span></span>|<span data-ttu-id="ee34f-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ee34f-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee34f-122">displayName</span><span class="sxs-lookup"><span data-stu-id="ee34f-122">displayName</span></span>|<span data-ttu-id="ee34f-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee34f-123">String</span></span>|<span data-ttu-id="ee34f-124">Anzeigename des Statusberichts</span><span class="sxs-lookup"><span data-stu-id="ee34f-124">Friendly name of the status report.</span></span>|
|<span data-ttu-id="ee34f-125">id</span><span class="sxs-lookup"><span data-stu-id="ee34f-125">id</span></span>|<span data-ttu-id="ee34f-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee34f-126">String</span></span>|<span data-ttu-id="ee34f-127">Schlüssel der Entität</span><span class="sxs-lookup"><span data-stu-id="ee34f-127">Key of the entity.</span></span>|
|<span data-ttu-id="ee34f-128">Version</span><span class="sxs-lookup"><span data-stu-id="ee34f-128">version</span></span>|<span data-ttu-id="ee34f-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="ee34f-129">String</span></span>|<span data-ttu-id="ee34f-130">Version der Entität</span><span class="sxs-lookup"><span data-stu-id="ee34f-130">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee34f-131">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="ee34f-131">Relationships</span></span>
<span data-ttu-id="ee34f-132">Keine</span><span class="sxs-lookup"><span data-stu-id="ee34f-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee34f-133">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="ee34f-133">JSON Representation</span></span>
<span data-ttu-id="ee34f-134">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="ee34f-134">Here is a JSON representation of the resource.</span></span>
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




