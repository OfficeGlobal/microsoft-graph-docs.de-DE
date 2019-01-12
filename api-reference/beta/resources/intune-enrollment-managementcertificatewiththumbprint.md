---
title: Ressourcentyp managementCertificateWithThumbprint
description: Noch nicht dokumentiert
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6e6259c1f90547ff875fa31d3f383606749bc0dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983352"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="640eb-103">Ressourcentyp managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="640eb-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="640eb-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="640eb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="640eb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="640eb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="640eb-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="640eb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="640eb-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="640eb-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="640eb-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="640eb-108">Properties</span></span>
|<span data-ttu-id="640eb-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="640eb-109">Property</span></span>|<span data-ttu-id="640eb-110">Typ</span><span class="sxs-lookup"><span data-stu-id="640eb-110">Type</span></span>|<span data-ttu-id="640eb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="640eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="640eb-112">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="640eb-112">thumbprint</span></span>|<span data-ttu-id="640eb-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="640eb-113">String</span></span>|<span data-ttu-id="640eb-114">Den Fingerabdruck des Zertifikats management</span><span class="sxs-lookup"><span data-stu-id="640eb-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="640eb-115">certificate</span><span class="sxs-lookup"><span data-stu-id="640eb-115">certificate</span></span>|<span data-ttu-id="640eb-116">String</span><span class="sxs-lookup"><span data-stu-id="640eb-116">String</span></span>|<span data-ttu-id="640eb-117">Das Zertifikat der Base64-codierten management</span><span class="sxs-lookup"><span data-stu-id="640eb-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="640eb-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="640eb-118">Relationships</span></span>
<span data-ttu-id="640eb-119">Keine</span><span class="sxs-lookup"><span data-stu-id="640eb-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="640eb-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="640eb-120">JSON Representation</span></span>
<span data-ttu-id="640eb-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="640eb-121">Here is a JSON representation of the resource.</span></span>
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





