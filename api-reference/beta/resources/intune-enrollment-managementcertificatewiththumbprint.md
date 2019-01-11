---
title: Ressourcentyp managementCertificateWithThumbprint
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d8f18e7fc117f00f99346267f544abc7d12db17e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827216"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="bdcdb-103">Ressourcentyp managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="bdcdb-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="bdcdb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="bdcdb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bdcdb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="bdcdb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bdcdb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="bdcdb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdcdb-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="bdcdb-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bdcdb-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="bdcdb-108">Properties</span></span>
|<span data-ttu-id="bdcdb-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="bdcdb-109">Property</span></span>|<span data-ttu-id="bdcdb-110">Typ</span><span class="sxs-lookup"><span data-stu-id="bdcdb-110">Type</span></span>|<span data-ttu-id="bdcdb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="bdcdb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdcdb-112">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="bdcdb-112">thumbprint</span></span>|<span data-ttu-id="bdcdb-113">String</span><span class="sxs-lookup"><span data-stu-id="bdcdb-113">String</span></span>|<span data-ttu-id="bdcdb-114">Den Fingerabdruck des Zertifikats management</span><span class="sxs-lookup"><span data-stu-id="bdcdb-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="bdcdb-115">certificate</span><span class="sxs-lookup"><span data-stu-id="bdcdb-115">certificate</span></span>|<span data-ttu-id="bdcdb-116">String</span><span class="sxs-lookup"><span data-stu-id="bdcdb-116">String</span></span>|<span data-ttu-id="bdcdb-117">Das Zertifikat der Base64-codierten management</span><span class="sxs-lookup"><span data-stu-id="bdcdb-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdcdb-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="bdcdb-118">Relationships</span></span>
<span data-ttu-id="bdcdb-119">Keine</span><span class="sxs-lookup"><span data-stu-id="bdcdb-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bdcdb-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="bdcdb-120">JSON Representation</span></span>
<span data-ttu-id="bdcdb-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="bdcdb-121">Here is a JSON representation of the resource.</span></span>
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





