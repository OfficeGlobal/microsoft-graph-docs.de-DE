---
title: managementCertificateWithThumbprint-Ressourcentyp
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36adab8de1cebe884f6932e2a99b3aba9174d518
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151261"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="fb169-103">managementCertificateWithThumbprint-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="fb169-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="fb169-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fb169-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb169-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="fb169-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb169-106">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="fb169-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fb169-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="fb169-107">Properties</span></span>
|<span data-ttu-id="fb169-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="fb169-108">Property</span></span>|<span data-ttu-id="fb169-109">Typ</span><span class="sxs-lookup"><span data-stu-id="fb169-109">Type</span></span>|<span data-ttu-id="fb169-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fb169-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb169-111">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="fb169-111">thumbprint</span></span>|<span data-ttu-id="fb169-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="fb169-112">String</span></span>|<span data-ttu-id="fb169-113">Der Fingerabdruck des Verwaltungszertifikats</span><span class="sxs-lookup"><span data-stu-id="fb169-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="fb169-114">certificate</span><span class="sxs-lookup"><span data-stu-id="fb169-114">certificate</span></span>|<span data-ttu-id="fb169-115">String</span><span class="sxs-lookup"><span data-stu-id="fb169-115">String</span></span>|<span data-ttu-id="fb169-116">Das Basis 64-codierte Verwaltungszertifikat</span><span class="sxs-lookup"><span data-stu-id="fb169-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb169-117">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="fb169-117">Relationships</span></span>
<span data-ttu-id="fb169-118">Keine</span><span class="sxs-lookup"><span data-stu-id="fb169-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb169-119">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="fb169-119">JSON Representation</span></span>
<span data-ttu-id="fb169-120">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="fb169-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```




