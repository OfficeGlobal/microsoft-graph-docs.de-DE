---
title: windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp
description: Windows Information Protection – Datenwiederherstellungszertifikat
author: tfitzmac
ms.openlocfilehash: c45abb14669c3cf67571748a9da7d62bed037ff6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325823"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="b60b9-103">windowsInformationProtectionDataRecoveryCertificate-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b60b9-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="b60b9-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b60b9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b60b9-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b60b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b60b9-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b60b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b60b9-107">Windows Information Protection – Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="b60b9-107">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="b60b9-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b60b9-108">Properties</span></span>
|<span data-ttu-id="b60b9-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b60b9-109">Property</span></span>|<span data-ttu-id="b60b9-110">Typ</span><span class="sxs-lookup"><span data-stu-id="b60b9-110">Type</span></span>|<span data-ttu-id="b60b9-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b60b9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b60b9-112">subjectName</span><span class="sxs-lookup"><span data-stu-id="b60b9-112">subjectName</span></span>|<span data-ttu-id="b60b9-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b60b9-113">String</span></span>|<span data-ttu-id="b60b9-114">Antragstellername des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="b60b9-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="b60b9-115">description</span><span class="sxs-lookup"><span data-stu-id="b60b9-115">description</span></span>|<span data-ttu-id="b60b9-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b60b9-116">String</span></span>|<span data-ttu-id="b60b9-117">Beschreibung des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="b60b9-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="b60b9-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b60b9-118">expirationDateTime</span></span>|<span data-ttu-id="b60b9-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b60b9-119">DateTimeOffset</span></span>|<span data-ttu-id="b60b9-120">Ablaufdatum des Datenwiederherstellungszertifikats</span><span class="sxs-lookup"><span data-stu-id="b60b9-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="b60b9-121">certificate</span><span class="sxs-lookup"><span data-stu-id="b60b9-121">certificate</span></span>|<span data-ttu-id="b60b9-122">Binär</span><span class="sxs-lookup"><span data-stu-id="b60b9-122">Binary</span></span>|<span data-ttu-id="b60b9-123">Datenwiederherstellungszertifikat</span><span class="sxs-lookup"><span data-stu-id="b60b9-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="b60b9-124">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b60b9-124">Relationships</span></span>
<span data-ttu-id="b60b9-125">Keine</span><span class="sxs-lookup"><span data-stu-id="b60b9-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b60b9-126">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b60b9-126">JSON Representation</span></span>
<span data-ttu-id="b60b9-127">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b60b9-127">Here is a JSON representation of the resource.</span></span>
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





