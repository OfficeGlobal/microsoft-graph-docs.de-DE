---
title: Ressourcentyp certificateConnectorSetting
description: Connector-Einstellungen für Zertifikate.
author: tfitzmac
ms.openlocfilehash: 8c993634eb4f41e16643ae3f40be74ecc3eb392f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326306"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="f7fa5-103">Ressourcentyp certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="f7fa5-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="f7fa5-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="f7fa5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7fa5-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f7fa5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7fa5-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="f7fa5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7fa5-107">Connector-Einstellungen für Zertifikate.</span><span class="sxs-lookup"><span data-stu-id="f7fa5-107">Certificate connector settings.</span></span>
## <a name="properties"></a><span data-ttu-id="f7fa5-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f7fa5-108">Properties</span></span>
|<span data-ttu-id="f7fa5-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f7fa5-109">Property</span></span>|<span data-ttu-id="f7fa5-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f7fa5-110">Type</span></span>|<span data-ttu-id="f7fa5-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f7fa5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7fa5-112">status</span><span class="sxs-lookup"><span data-stu-id="f7fa5-112">status</span></span>|<span data-ttu-id="f7fa5-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f7fa5-113">Int32</span></span>|<span data-ttu-id="f7fa5-114">Zertifikat Connectorstatus</span><span class="sxs-lookup"><span data-stu-id="f7fa5-114">Certificate connector status</span></span>|
|<span data-ttu-id="f7fa5-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="f7fa5-115">certExpiryTime</span></span>|<span data-ttu-id="f7fa5-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7fa5-116">DateTimeOffset</span></span>|<span data-ttu-id="f7fa5-117">Zertifikat abläuft Zeit</span><span class="sxs-lookup"><span data-stu-id="f7fa5-117">Certificate expire time</span></span>|
|<span data-ttu-id="f7fa5-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="f7fa5-118">enrollmentError</span></span>|<span data-ttu-id="f7fa5-119">String</span><span class="sxs-lookup"><span data-stu-id="f7fa5-119">String</span></span>|<span data-ttu-id="f7fa5-120">Zertifikatfehler Connector-Registrierung</span><span class="sxs-lookup"><span data-stu-id="f7fa5-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="f7fa5-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="f7fa5-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="f7fa5-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7fa5-122">DateTimeOffset</span></span>|<span data-ttu-id="f7fa5-123">Zuletzt Zertifikat Connector verbunden</span><span class="sxs-lookup"><span data-stu-id="f7fa5-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="f7fa5-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="f7fa5-124">connectorVersion</span></span>|<span data-ttu-id="f7fa5-125">String</span><span class="sxs-lookup"><span data-stu-id="f7fa5-125">String</span></span>|<span data-ttu-id="f7fa5-126">Version des Zertifikat-Connectors</span><span class="sxs-lookup"><span data-stu-id="f7fa5-126">Version of certificate connector</span></span>|
|<span data-ttu-id="f7fa5-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="f7fa5-127">lastUploadVersion</span></span>|<span data-ttu-id="f7fa5-128">Int64</span><span class="sxs-lookup"><span data-stu-id="f7fa5-128">Int64</span></span>|<span data-ttu-id="f7fa5-129">Version des letzten hochgeladenen Zertifikat connector</span><span class="sxs-lookup"><span data-stu-id="f7fa5-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7fa5-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f7fa5-130">Relationships</span></span>
<span data-ttu-id="f7fa5-131">Keine</span><span class="sxs-lookup"><span data-stu-id="f7fa5-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f7fa5-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f7fa5-132">JSON Representation</span></span>
<span data-ttu-id="f7fa5-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f7fa5-133">Here is a JSON representation of the resource.</span></span>
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





