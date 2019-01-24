---
title: Ressourcentyp deviceManagementTroubleshootingErrorResource
description: -Objekt, der einen Link zu Informationen, die den Link zur Problembehandlung konnte der Azure-Verwaltungsportal oder eine Microsoft Doc sein.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5653801fb3e4575e642c012721b667f51e791cc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430222"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="8b5d3-103">Ressourcentyp deviceManagementTroubleshootingErrorResource</span><span class="sxs-lookup"><span data-stu-id="8b5d3-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="8b5d3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="8b5d3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8b5d3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8b5d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8b5d3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="8b5d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b5d3-107">-Objekt, der einen Link zu Informationen, die den Link zur Problembehandlung konnte der Azure-Verwaltungsportal oder eine Microsoft Doc sein.</span><span class="sxs-lookup"><span data-stu-id="8b5d3-107">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="8b5d3-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8b5d3-108">Properties</span></span>
|<span data-ttu-id="8b5d3-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8b5d3-109">Property</span></span>|<span data-ttu-id="8b5d3-110">Typ</span><span class="sxs-lookup"><span data-stu-id="8b5d3-110">Type</span></span>|<span data-ttu-id="8b5d3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8b5d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b5d3-112">text</span><span class="sxs-lookup"><span data-stu-id="8b5d3-112">text</span></span>|<span data-ttu-id="8b5d3-113">String</span><span class="sxs-lookup"><span data-stu-id="8b5d3-113">String</span></span>|<span data-ttu-id="8b5d3-114">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="8b5d3-114">Not yet documented</span></span>|
|<span data-ttu-id="8b5d3-115">Link</span><span class="sxs-lookup"><span data-stu-id="8b5d3-115">link</span></span>|<span data-ttu-id="8b5d3-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8b5d3-116">String</span></span>|<span data-ttu-id="8b5d3-117">Den Link zur Webressource.</span><span class="sxs-lookup"><span data-stu-id="8b5d3-117">The link to the web resource.</span></span> <span data-ttu-id="8b5d3-118">Kann eine der folgenden Formatierungsprogramme enthalten: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span><span class="sxs-lookup"><span data-stu-id="8b5d3-118">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b5d3-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="8b5d3-119">Relationships</span></span>
<span data-ttu-id="8b5d3-120">Keine</span><span class="sxs-lookup"><span data-stu-id="8b5d3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8b5d3-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8b5d3-121">JSON Representation</span></span>
<span data-ttu-id="8b5d3-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8b5d3-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```



