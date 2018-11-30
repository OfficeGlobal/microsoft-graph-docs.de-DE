---
title: windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp
description: Windows Information Protection – Datenwiederherstellungszertifikat
ms.openlocfilehash: 68faf0e78c68468216c3e69d64926f2c8b18e3c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018627"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="c9807-103">windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="c9807-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="c9807-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="c9807-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9807-105">Windows Information Protection – Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="c9807-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="c9807-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c9807-106">Properties</span></span>
|<span data-ttu-id="c9807-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="c9807-107">Property</span></span>|<span data-ttu-id="c9807-108">Typ</span><span class="sxs-lookup"><span data-stu-id="c9807-108">Type</span></span>|<span data-ttu-id="c9807-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="c9807-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9807-110">subjectName</span><span class="sxs-lookup"><span data-stu-id="c9807-110">subjectName</span></span>|<span data-ttu-id="c9807-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9807-111">String</span></span>|<span data-ttu-id="c9807-112">Antragstellername des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="c9807-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="c9807-113">description</span><span class="sxs-lookup"><span data-stu-id="c9807-113">description</span></span>|<span data-ttu-id="c9807-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="c9807-114">String</span></span>|<span data-ttu-id="c9807-115">Beschreibung des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="c9807-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="c9807-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c9807-116">expirationDateTime</span></span>|<span data-ttu-id="c9807-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9807-117">DateTimeOffset</span></span>|<span data-ttu-id="c9807-118">Ablaufdatum des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="c9807-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="c9807-119">certificate</span><span class="sxs-lookup"><span data-stu-id="c9807-119">certificate</span></span>|<span data-ttu-id="c9807-120">Binär</span><span class="sxs-lookup"><span data-stu-id="c9807-120">Binary</span></span>|<span data-ttu-id="c9807-121">Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="c9807-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9807-122">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="c9807-122">Relationships</span></span>
<span data-ttu-id="c9807-123">Keine</span><span class="sxs-lookup"><span data-stu-id="c9807-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9807-124">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="c9807-124">JSON Representation</span></span>
<span data-ttu-id="c9807-125">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="c9807-125">Here is a JSON representation of the resource.</span></span>
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



