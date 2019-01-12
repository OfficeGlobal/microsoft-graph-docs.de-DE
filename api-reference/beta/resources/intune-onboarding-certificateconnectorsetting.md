---
title: Ressourcentyp certificateConnectorSetting
description: Connector-Einstellungen für Zertifikate.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 74a63d308d53d09b71b19b2ff10a9d94c3fa818d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980993"
---
# <a name="certificateconnectorsetting-resource-type"></a><span data-ttu-id="51203-103">Ressourcentyp certificateConnectorSetting</span><span class="sxs-lookup"><span data-stu-id="51203-103">certificateConnectorSetting resource type</span></span>

> <span data-ttu-id="51203-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="51203-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51203-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51203-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51203-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="51203-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51203-107">Connector-Einstellungen für Zertifikate.</span><span class="sxs-lookup"><span data-stu-id="51203-107">Certificate connector settings.</span></span>
## <a name="properties"></a><span data-ttu-id="51203-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="51203-108">Properties</span></span>
|<span data-ttu-id="51203-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="51203-109">Property</span></span>|<span data-ttu-id="51203-110">Typ</span><span class="sxs-lookup"><span data-stu-id="51203-110">Type</span></span>|<span data-ttu-id="51203-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51203-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51203-112">status</span><span class="sxs-lookup"><span data-stu-id="51203-112">status</span></span>|<span data-ttu-id="51203-113">Int32</span><span class="sxs-lookup"><span data-stu-id="51203-113">Int32</span></span>|<span data-ttu-id="51203-114">Zertifikat Connectorstatus</span><span class="sxs-lookup"><span data-stu-id="51203-114">Certificate connector status</span></span>|
|<span data-ttu-id="51203-115">certExpiryTime</span><span class="sxs-lookup"><span data-stu-id="51203-115">certExpiryTime</span></span>|<span data-ttu-id="51203-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51203-116">DateTimeOffset</span></span>|<span data-ttu-id="51203-117">Zertifikat abläuft Zeit</span><span class="sxs-lookup"><span data-stu-id="51203-117">Certificate expire time</span></span>|
|<span data-ttu-id="51203-118">enrollmentError</span><span class="sxs-lookup"><span data-stu-id="51203-118">enrollmentError</span></span>|<span data-ttu-id="51203-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="51203-119">String</span></span>|<span data-ttu-id="51203-120">Zertifikatfehler Connector-Registrierung</span><span class="sxs-lookup"><span data-stu-id="51203-120">Certificate connector enrollment error</span></span>|
|<span data-ttu-id="51203-121">lastConnectorConnectionTime</span><span class="sxs-lookup"><span data-stu-id="51203-121">lastConnectorConnectionTime</span></span>|<span data-ttu-id="51203-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51203-122">DateTimeOffset</span></span>|<span data-ttu-id="51203-123">Zuletzt Zertifikat Connector verbunden</span><span class="sxs-lookup"><span data-stu-id="51203-123">Last time certificate connector connected</span></span>|
|<span data-ttu-id="51203-124">connectorVersion</span><span class="sxs-lookup"><span data-stu-id="51203-124">connectorVersion</span></span>|<span data-ttu-id="51203-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="51203-125">String</span></span>|<span data-ttu-id="51203-126">Version des Zertifikat-Connectors</span><span class="sxs-lookup"><span data-stu-id="51203-126">Version of certificate connector</span></span>|
|<span data-ttu-id="51203-127">lastUploadVersion</span><span class="sxs-lookup"><span data-stu-id="51203-127">lastUploadVersion</span></span>|<span data-ttu-id="51203-128">Int64</span><span class="sxs-lookup"><span data-stu-id="51203-128">Int64</span></span>|<span data-ttu-id="51203-129">Version des letzten hochgeladenen Zertifikat connector</span><span class="sxs-lookup"><span data-stu-id="51203-129">Version of last uploaded certificate connector</span></span>|

## <a name="relationships"></a><span data-ttu-id="51203-130">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="51203-130">Relationships</span></span>
<span data-ttu-id="51203-131">Keine</span><span class="sxs-lookup"><span data-stu-id="51203-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51203-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="51203-132">JSON Representation</span></span>
<span data-ttu-id="51203-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="51203-133">Here is a JSON representation of the resource.</span></span>
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





