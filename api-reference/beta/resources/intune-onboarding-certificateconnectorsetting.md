---
title: Ressourcentyp certificateConnectorSetting
description: Connector-Einstellungen für Zertifikate.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5886418aaddede43f2397ad626028598a63a0066
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398653"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="b2714-103">Ressourcentyp certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="b2714-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="b2714-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="b2714-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b2714-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b2714-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2714-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b2714-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2714-107">Connector-Einstellungen für Zertifikate.</span><span class="sxs-lookup"><span data-stu-id="b2714-107">Certificate connector settings.</span></span>

## <a name="properties"></a><span data-ttu-id="b2714-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b2714-108">Properties</span></span>
|<span data-ttu-id="b2714-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b2714-109">Property</span></span>|<span data-ttu-id="b2714-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b2714-110">Type</span></span>|<span data-ttu-id="b2714-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b2714-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2714-112">status</span><span class="sxs-lookup"><span data-stu-id="b2714-112">status</span></span>|<span data-ttu-id="b2714-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b2714-113">Int32</span></span>|<span data-ttu-id="b2714-114">Zertifikat Connectorstatus</span><span class="sxs-lookup"><span data-stu-id="b2714-114">Certificate connector status</span></span>|
|<span data-ttu-id="b2714-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="b2714-115">certExpiryTime</span></span>|<span data-ttu-id="b2714-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2714-116">DateTimeOffset</span></span>|<span data-ttu-id="b2714-117">Zertifikat abläuft Zeit</span><span class="sxs-lookup"><span data-stu-id="b2714-117">Certificate expire time</span></span>|
|<span data-ttu-id="b2714-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="b2714-118">enrollmentError</span></span>|<span data-ttu-id="b2714-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2714-119">String</span></span>|<span data-ttu-id="b2714-120">Zertifikatfehler Connector-Registrierung</span><span class="sxs-lookup"><span data-stu-id="b2714-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="b2714-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="b2714-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="b2714-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2714-122">DateTimeOffset</span></span>|<span data-ttu-id="b2714-123">Zuletzt Zertifikat Connector verbunden</span><span class="sxs-lookup"><span data-stu-id="b2714-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="b2714-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="b2714-124">connectorVersion</span></span>|<span data-ttu-id="b2714-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b2714-125">String</span></span>|<span data-ttu-id="b2714-126">Version des Zertifikat-Connectors</span><span class="sxs-lookup"><span data-stu-id="b2714-126">Version of certificate connector</span></span>|
|<span data-ttu-id="b2714-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="b2714-127">lastUploadVersion</span></span>|<span data-ttu-id="b2714-128">Int64</span><span class="sxs-lookup"><span data-stu-id="b2714-128">Int64</span></span>|<span data-ttu-id="b2714-129">Version des letzten hochgeladenen Zertifikat connector</span><span class="sxs-lookup"><span data-stu-id="b2714-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2714-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b2714-130">Relationships</span></span>
<span data-ttu-id="b2714-131">Keine</span><span class="sxs-lookup"><span data-stu-id="b2714-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b2714-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b2714-132">JSON Representation</span></span>
<span data-ttu-id="b2714-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b2714-133">Here is a JSON representation of the resource.</span></span>
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




