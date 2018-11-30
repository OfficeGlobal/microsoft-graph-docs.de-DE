---
title: Ressourcentyp certificateConnectorSetting
description: Connector-Einstellungen für Zertifikate.
ms.openlocfilehash: 65f87002016c4d5bd6b19106ba1aa988ad30d92e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27057903"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="6da72-103">Ressourcentyp certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="6da72-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="6da72-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6da72-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6da72-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6da72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6da72-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="6da72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6da72-107">Connector-Einstellungen für Zertifikate.</span><span class="sxs-lookup"><span data-stu-id="6da72-107">Certificate connector settings.</span></span>
## <a name="properties"></a><span data-ttu-id="6da72-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="6da72-108">Properties</span></span>
|<span data-ttu-id="6da72-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6da72-109">Property</span></span>|<span data-ttu-id="6da72-110">Typ</span><span class="sxs-lookup"><span data-stu-id="6da72-110">Type</span></span>|<span data-ttu-id="6da72-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6da72-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6da72-112">status</span><span class="sxs-lookup"><span data-stu-id="6da72-112">status</span></span>|<span data-ttu-id="6da72-113">Int32</span><span class="sxs-lookup"><span data-stu-id="6da72-113">Int32</span></span>|<span data-ttu-id="6da72-114">Zertifikat Connectorstatus</span><span class="sxs-lookup"><span data-stu-id="6da72-114">Certificate connector status</span></span>|
|<span data-ttu-id="6da72-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="6da72-115">certExpiryTime</span></span>|<span data-ttu-id="6da72-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6da72-116">DateTimeOffset</span></span>|<span data-ttu-id="6da72-117">Zertifikat abläuft Zeit</span><span class="sxs-lookup"><span data-stu-id="6da72-117">Certificate expire time</span></span>|
|<span data-ttu-id="6da72-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="6da72-118">enrollmentError</span></span>|<span data-ttu-id="6da72-119">String</span><span class="sxs-lookup"><span data-stu-id="6da72-119">String</span></span>|<span data-ttu-id="6da72-120">Zertifikatfehler Connector-Registrierung</span><span class="sxs-lookup"><span data-stu-id="6da72-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="6da72-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="6da72-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="6da72-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6da72-122">DateTimeOffset</span></span>|<span data-ttu-id="6da72-123">Zuletzt Zertifikat Connector verbunden</span><span class="sxs-lookup"><span data-stu-id="6da72-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="6da72-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="6da72-124">connectorVersion</span></span>|<span data-ttu-id="6da72-125">String</span><span class="sxs-lookup"><span data-stu-id="6da72-125">String</span></span>|<span data-ttu-id="6da72-126">Version des Zertifikat-Connectors</span><span class="sxs-lookup"><span data-stu-id="6da72-126">Version of certificate connector</span></span>|
|<span data-ttu-id="6da72-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="6da72-127">lastUploadVersion</span></span>|<span data-ttu-id="6da72-128">Int64</span><span class="sxs-lookup"><span data-stu-id="6da72-128">Int64</span></span>|<span data-ttu-id="6da72-129">Version des letzten hochgeladenen Zertifikat connector</span><span class="sxs-lookup"><span data-stu-id="6da72-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="6da72-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="6da72-130">Relationships</span></span>
<span data-ttu-id="6da72-131">Keine</span><span class="sxs-lookup"><span data-stu-id="6da72-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6da72-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="6da72-132">JSON Representation</span></span>
<span data-ttu-id="6da72-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="6da72-133">Here is a JSON representation of the resource.</span></span>
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





