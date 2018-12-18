---
title: windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp
description: Windows Information Protection – Datenwiederherstellungszertifikat
author: tfitzmac
ms.openlocfilehash: a66c1eeae6d405aa8d0546ac0143e2a8b3404231
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361663"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="21c10-103">windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="21c10-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="21c10-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="21c10-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21c10-105">Windows Information Protection – Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="21c10-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="21c10-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="21c10-106">Properties</span></span>
|<span data-ttu-id="21c10-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="21c10-107">Property</span></span>|<span data-ttu-id="21c10-108">Typ</span><span class="sxs-lookup"><span data-stu-id="21c10-108">Type</span></span>|<span data-ttu-id="21c10-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21c10-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21c10-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="21c10-110">subjectName</span></span>|<span data-ttu-id="21c10-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21c10-111">String</span></span>|<span data-ttu-id="21c10-112">Antragstellername des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="21c10-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="21c10-113">description</span><span class="sxs-lookup"><span data-stu-id="21c10-113">description</span></span>|<span data-ttu-id="21c10-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="21c10-114">String</span></span>|<span data-ttu-id="21c10-115">Beschreibung des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="21c10-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="21c10-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="21c10-116">expirationDateTime</span></span>|<span data-ttu-id="21c10-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="21c10-117">DateTimeOffset</span></span>|<span data-ttu-id="21c10-118">Ablaufdatum des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="21c10-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="21c10-119">certificate</span><span class="sxs-lookup"><span data-stu-id="21c10-119">certificate</span></span>|<span data-ttu-id="21c10-120">Binär</span><span class="sxs-lookup"><span data-stu-id="21c10-120">Binary</span></span>|<span data-ttu-id="21c10-121">Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="21c10-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="21c10-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="21c10-122">Relationships</span></span>
<span data-ttu-id="21c10-123">Keine</span><span class="sxs-lookup"><span data-stu-id="21c10-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="21c10-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="21c10-124">JSON Representation</span></span>
<span data-ttu-id="21c10-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="21c10-125">Here is a JSON representation of the resource.</span></span>
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



