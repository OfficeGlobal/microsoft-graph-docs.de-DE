---
title: windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp
description: Windows Information Protection – Datenwiederherstellungszertifikat
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c321ea06e27e7d6fba0a35446e2b916aaf0689de
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253652"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="cc13e-103">windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="cc13e-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="cc13e-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="cc13e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc13e-105">Windows Information Protection – Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="cc13e-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="cc13e-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="cc13e-106">Properties</span></span>
|<span data-ttu-id="cc13e-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="cc13e-107">Property</span></span>|<span data-ttu-id="cc13e-108">Typ</span><span class="sxs-lookup"><span data-stu-id="cc13e-108">Type</span></span>|<span data-ttu-id="cc13e-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cc13e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc13e-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="cc13e-110">subjectName</span></span>|<span data-ttu-id="cc13e-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cc13e-111">String</span></span>|<span data-ttu-id="cc13e-112">Antragstellername des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="cc13e-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="cc13e-113">description</span><span class="sxs-lookup"><span data-stu-id="cc13e-113">description</span></span>|<span data-ttu-id="cc13e-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="cc13e-114">String</span></span>|<span data-ttu-id="cc13e-115">Beschreibung des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="cc13e-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="cc13e-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="cc13e-116">expirationDateTime</span></span>|<span data-ttu-id="cc13e-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc13e-117">DateTimeOffset</span></span>|<span data-ttu-id="cc13e-118">Ablaufdatum des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="cc13e-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="cc13e-119">certificate</span><span class="sxs-lookup"><span data-stu-id="cc13e-119">certificate</span></span>|<span data-ttu-id="cc13e-120">Binär</span><span class="sxs-lookup"><span data-stu-id="cc13e-120">Binary</span></span>|<span data-ttu-id="cc13e-121">Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="cc13e-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc13e-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="cc13e-122">Relationships</span></span>
<span data-ttu-id="cc13e-123">Keine</span><span class="sxs-lookup"><span data-stu-id="cc13e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc13e-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="cc13e-124">JSON Representation</span></span>
<span data-ttu-id="cc13e-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="cc13e-125">Here is a JSON representation of the resource.</span></span>
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



