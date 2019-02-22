---
title: deviceManagementTroubleshootingErrorResource-Ressourcentyp
description: -Objekt, das einen Link zu Informationen zur Problembehandlung darstellt, kann die Verknüpfung zum Azure-Portal oder einem Microsoft-Dokument sein.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 25d97a6d085b9f1b7e0b1ab73361be3ac7ae74d2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155559"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a><span data-ttu-id="d1be4-103">deviceManagementTroubleshootingErrorResource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d1be4-103">deviceManagementTroubleshootingErrorResource resource type</span></span>

> <span data-ttu-id="d1be4-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d1be4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1be4-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d1be4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1be4-106">-Objekt, das einen Link zu Informationen zur Problembehandlung darstellt, kann die Verknüpfung zum Azure-Portal oder einem Microsoft-Dokument sein.</span><span class="sxs-lookup"><span data-stu-id="d1be4-106">Object representing a link to troubleshooting information, the link could be to the Azure Portal or a Microsoft doc.</span></span>

## <a name="properties"></a><span data-ttu-id="d1be4-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="d1be4-107">Properties</span></span>
|<span data-ttu-id="d1be4-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d1be4-108">Property</span></span>|<span data-ttu-id="d1be4-109">Typ</span><span class="sxs-lookup"><span data-stu-id="d1be4-109">Type</span></span>|<span data-ttu-id="d1be4-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d1be4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1be4-111">text</span><span class="sxs-lookup"><span data-stu-id="d1be4-111">text</span></span>|<span data-ttu-id="d1be4-112">String</span><span class="sxs-lookup"><span data-stu-id="d1be4-112">String</span></span>|<span data-ttu-id="d1be4-113">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="d1be4-113">Not yet documented</span></span>|
|<span data-ttu-id="d1be4-114">Link</span><span class="sxs-lookup"><span data-stu-id="d1be4-114">link</span></span>|<span data-ttu-id="d1be4-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d1be4-115">String</span></span>|<span data-ttu-id="d1be4-116">Die Verknüpfung zur Webressource.</span><span class="sxs-lookup"><span data-stu-id="d1be4-116">The link to the web resource.</span></span> <span data-ttu-id="d1be4-117">Kann beliebige der folgenden Formatierungen enthalten: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span><span class="sxs-lookup"><span data-stu-id="d1be4-117">Can contain any of the following formatters: {{UPN}}, {{DeviceGUID}}, {{UserGUID}}</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1be4-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="d1be4-118">Relationships</span></span>
<span data-ttu-id="d1be4-119">Keine</span><span class="sxs-lookup"><span data-stu-id="d1be4-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1be4-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="d1be4-120">JSON Representation</span></span>
<span data-ttu-id="d1be4-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="d1be4-121">Here is a JSON representation of the resource.</span></span>
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




