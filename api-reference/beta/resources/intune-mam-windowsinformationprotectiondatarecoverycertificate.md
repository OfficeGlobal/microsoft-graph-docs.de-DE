---
title: windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp
description: Windows Information Protection – Datenwiederherstellungszertifikat
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6a5606906cbec0122137faf3cb454edec785c42
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405800"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="f259d-103">windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="f259d-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="f259d-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="f259d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f259d-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="f259d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f259d-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="f259d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f259d-107">Windows Information Protection – Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="f259d-107">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="f259d-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="f259d-108">Properties</span></span>
|<span data-ttu-id="f259d-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="f259d-109">Property</span></span>|<span data-ttu-id="f259d-110">Typ</span><span class="sxs-lookup"><span data-stu-id="f259d-110">Type</span></span>|<span data-ttu-id="f259d-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="f259d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f259d-112">subjectName</span><span class="sxs-lookup"><span data-stu-id="f259d-112">subjectName</span></span>|<span data-ttu-id="f259d-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f259d-113">String</span></span>|<span data-ttu-id="f259d-114">Antragstellername des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="f259d-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="f259d-115">description</span><span class="sxs-lookup"><span data-stu-id="f259d-115">description</span></span>|<span data-ttu-id="f259d-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="f259d-116">String</span></span>|<span data-ttu-id="f259d-117">Beschreibung des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="f259d-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="f259d-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f259d-118">expirationDateTime</span></span>|<span data-ttu-id="f259d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f259d-119">DateTimeOffset</span></span>|<span data-ttu-id="f259d-120">Ablaufdatum des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="f259d-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="f259d-121">certificate</span><span class="sxs-lookup"><span data-stu-id="f259d-121">certificate</span></span>|<span data-ttu-id="f259d-122">Binär</span><span class="sxs-lookup"><span data-stu-id="f259d-122">Binary</span></span>|<span data-ttu-id="f259d-123">Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="f259d-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="f259d-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="f259d-124">Relationships</span></span>
<span data-ttu-id="f259d-125">Keine</span><span class="sxs-lookup"><span data-stu-id="f259d-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f259d-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="f259d-126">JSON Representation</span></span>
<span data-ttu-id="f259d-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="f259d-127">Here is a JSON representation of the resource.</span></span>
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




