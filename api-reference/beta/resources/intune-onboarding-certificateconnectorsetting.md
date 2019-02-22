---
title: certificateConnectorSetting-Ressourcentyp
description: Zertifikat-konnektoreinstellungen.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09f4baf9ddd8be630c432fcec5d7df71c442bbe2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168306"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="f63e8-103">certificateConnectorSetting-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f63e8-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="f63e8-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f63e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f63e8-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="f63e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f63e8-106">Zertifikat-konnektoreinstellungen.</span><span class="sxs-lookup"><span data-stu-id="f63e8-106">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="f63e8-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f63e8-107">Properties</span></span>
|<span data-ttu-id="f63e8-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f63e8-108">Property</span></span>|<span data-ttu-id="f63e8-109">Typ</span><span class="sxs-lookup"><span data-stu-id="f63e8-109">Type</span></span>|<span data-ttu-id="f63e8-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f63e8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f63e8-111">status</span><span class="sxs-lookup"><span data-stu-id="f63e8-111">status</span></span>|<span data-ttu-id="f63e8-112">Int32</span><span class="sxs-lookup"><span data-stu-id="f63e8-112">Int32</span></span>|<span data-ttu-id="f63e8-113">Zertifikat-Connectorstatus</span><span class="sxs-lookup"><span data-stu-id="f63e8-113">Certificate connector status</span></span>|
|<span data-ttu-id="f63e8-114">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="f63e8-114">certExpiryTime</span></span>|<span data-ttu-id="f63e8-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f63e8-115">DateTimeOffset</span></span>|<span data-ttu-id="f63e8-116">Dauer des Zertifikats Ablaufs</span><span class="sxs-lookup"><span data-stu-id="f63e8-116">Certificate expire time</span></span>|
|<span data-ttu-id="f63e8-117">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="f63e8-117">enrollmentError</span></span>|<span data-ttu-id="f63e8-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f63e8-118">String</span></span>|<span data-ttu-id="f63e8-119">Zertifikat-Connector-Registrierungsfehler</span><span class="sxs-lookup"><span data-stu-id="f63e8-119">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="f63e8-120">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="f63e8-120">lastConnectorConnectionTime</span></span>|<span data-ttu-id="f63e8-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f63e8-121">DateTimeOffset</span></span>|<span data-ttu-id="f63e8-122">Letzter Zeitpunkt der Verbindung mit dem Zertifikat-Konnektor</span><span class="sxs-lookup"><span data-stu-id="f63e8-122">Last time certificate connector connected</span></span>|
|<span data-ttu-id="f63e8-123">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="f63e8-123">connectorVersion</span></span>|<span data-ttu-id="f63e8-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f63e8-124">String</span></span>|<span data-ttu-id="f63e8-125">Version von Certificate Connector</span><span class="sxs-lookup"><span data-stu-id="f63e8-125">Version of certificate connector</span></span>|
|<span data-ttu-id="f63e8-126">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="f63e8-126">lastUploadVersion</span></span>|<span data-ttu-id="f63e8-127">Int64</span><span class="sxs-lookup"><span data-stu-id="f63e8-127">Int64</span></span>|<span data-ttu-id="f63e8-128">Version des zuletzt hochgeladenen Zertifikats-Konnektors</span><span class="sxs-lookup"><span data-stu-id="f63e8-128">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="f63e8-129">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f63e8-129">Relationships</span></span>
<span data-ttu-id="f63e8-130">Keine</span><span class="sxs-lookup"><span data-stu-id="f63e8-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f63e8-131">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f63e8-131">JSON Representation</span></span>
<span data-ttu-id="f63e8-132">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f63e8-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```




