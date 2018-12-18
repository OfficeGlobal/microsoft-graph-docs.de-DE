---
title: Ressourcentyp managementCertificateWithThumbprint
description: Noch nicht dokumentiert
author: tfitzmac
ms.openlocfilehash: 03846890822cae02a2eb04fc058895992119c98a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348937"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="51739-103">Ressourcentyp managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="51739-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="51739-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="51739-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="51739-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="51739-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51739-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="51739-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51739-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="51739-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="51739-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="51739-108">Properties</span></span>
|<span data-ttu-id="51739-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="51739-109">Property</span></span>|<span data-ttu-id="51739-110">Typ</span><span class="sxs-lookup"><span data-stu-id="51739-110">Type</span></span>|<span data-ttu-id="51739-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="51739-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51739-112">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="51739-112">thumbprint</span></span>|<span data-ttu-id="51739-113">String</span><span class="sxs-lookup"><span data-stu-id="51739-113">String</span></span>|<span data-ttu-id="51739-114">Den Fingerabdruck des Zertifikats management</span><span class="sxs-lookup"><span data-stu-id="51739-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="51739-115">certificate</span><span class="sxs-lookup"><span data-stu-id="51739-115">certificate</span></span>|<span data-ttu-id="51739-116">String</span><span class="sxs-lookup"><span data-stu-id="51739-116">String</span></span>|<span data-ttu-id="51739-117">Das Zertifikat der Base64-codierten management</span><span class="sxs-lookup"><span data-stu-id="51739-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="51739-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="51739-118">Relationships</span></span>
<span data-ttu-id="51739-119">Keine</span><span class="sxs-lookup"><span data-stu-id="51739-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51739-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="51739-120">JSON Representation</span></span>
<span data-ttu-id="51739-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="51739-121">Here is a JSON representation of the resource.</span></span>
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





