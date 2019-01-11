---
title: windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp
description: Windows Information Protection – Datenwiederherstellungszertifikat
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 72edbdc16b2d84a2df6a4582bba12bab2feaa04c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821063"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="99622-103">windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="99622-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="99622-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="99622-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99622-105">Windows Information Protection – Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="99622-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="99622-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="99622-106">Properties</span></span>
|<span data-ttu-id="99622-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="99622-107">Property</span></span>|<span data-ttu-id="99622-108">Typ</span><span class="sxs-lookup"><span data-stu-id="99622-108">Type</span></span>|<span data-ttu-id="99622-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="99622-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99622-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="99622-110">subjectName</span></span>|<span data-ttu-id="99622-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="99622-111">String</span></span>|<span data-ttu-id="99622-112">Antragstellername des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="99622-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="99622-113">description</span><span class="sxs-lookup"><span data-stu-id="99622-113">description</span></span>|<span data-ttu-id="99622-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="99622-114">String</span></span>|<span data-ttu-id="99622-115">Beschreibung des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="99622-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="99622-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="99622-116">expirationDateTime</span></span>|<span data-ttu-id="99622-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99622-117">DateTimeOffset</span></span>|<span data-ttu-id="99622-118">Ablaufdatum des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="99622-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="99622-119">certificate</span><span class="sxs-lookup"><span data-stu-id="99622-119">certificate</span></span>|<span data-ttu-id="99622-120">Binär</span><span class="sxs-lookup"><span data-stu-id="99622-120">Binary</span></span>|<span data-ttu-id="99622-121">Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="99622-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="99622-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="99622-122">Relationships</span></span>
<span data-ttu-id="99622-123">Keine</span><span class="sxs-lookup"><span data-stu-id="99622-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="99622-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="99622-124">JSON Representation</span></span>
<span data-ttu-id="99622-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="99622-125">Here is a JSON representation of the resource.</span></span>
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



