---
title: windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp
description: Windows Information Protection – Datenwiederherstellungszertifikat
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74c480b8117f3d8dbf0ad8208bac09b63b113906
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156189"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="34a7c-103">windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="34a7c-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="34a7c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="34a7c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34a7c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="34a7c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34a7c-106">Windows Information Protection – Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="34a7c-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="34a7c-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="34a7c-107">Properties</span></span>
|<span data-ttu-id="34a7c-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="34a7c-108">Property</span></span>|<span data-ttu-id="34a7c-109">Typ</span><span class="sxs-lookup"><span data-stu-id="34a7c-109">Type</span></span>|<span data-ttu-id="34a7c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="34a7c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34a7c-111">subjectName</span><span class="sxs-lookup"><span data-stu-id="34a7c-111">subjectName</span></span>|<span data-ttu-id="34a7c-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a7c-112">String</span></span>|<span data-ttu-id="34a7c-113">Antragstellername des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="34a7c-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="34a7c-114">description</span><span class="sxs-lookup"><span data-stu-id="34a7c-114">description</span></span>|<span data-ttu-id="34a7c-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="34a7c-115">String</span></span>|<span data-ttu-id="34a7c-116">Beschreibung des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="34a7c-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="34a7c-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="34a7c-117">expirationDateTime</span></span>|<span data-ttu-id="34a7c-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34a7c-118">DateTimeOffset</span></span>|<span data-ttu-id="34a7c-119">Ablaufdatum des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="34a7c-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="34a7c-120">certificate</span><span class="sxs-lookup"><span data-stu-id="34a7c-120">certificate</span></span>|<span data-ttu-id="34a7c-121">Binär</span><span class="sxs-lookup"><span data-stu-id="34a7c-121">Binary</span></span>|<span data-ttu-id="34a7c-122">Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="34a7c-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="34a7c-123">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="34a7c-123">Relationships</span></span>
<span data-ttu-id="34a7c-124">Keine</span><span class="sxs-lookup"><span data-stu-id="34a7c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34a7c-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="34a7c-125">JSON Representation</span></span>
<span data-ttu-id="34a7c-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="34a7c-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```




