---
title: Ressourcentyp managementCertificateWithThumbprint
description: Noch nicht dokumentiert
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 765d3b9370e4b0f5eda481883956c72bf261e65a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418855"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="24c63-103">Ressourcentyp managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="24c63-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="24c63-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="24c63-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="24c63-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="24c63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24c63-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="24c63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24c63-107">Noch nicht dokumentiert</span><span class="sxs-lookup"><span data-stu-id="24c63-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="24c63-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="24c63-108">Properties</span></span>
|<span data-ttu-id="24c63-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="24c63-109">Property</span></span>|<span data-ttu-id="24c63-110">Typ</span><span class="sxs-lookup"><span data-stu-id="24c63-110">Type</span></span>|<span data-ttu-id="24c63-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="24c63-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24c63-112">Fingerabdruck</span><span class="sxs-lookup"><span data-stu-id="24c63-112">thumbprint</span></span>|<span data-ttu-id="24c63-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="24c63-113">String</span></span>|<span data-ttu-id="24c63-114">Den Fingerabdruck des Zertifikats management</span><span class="sxs-lookup"><span data-stu-id="24c63-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="24c63-115">certificate</span><span class="sxs-lookup"><span data-stu-id="24c63-115">certificate</span></span>|<span data-ttu-id="24c63-116">String</span><span class="sxs-lookup"><span data-stu-id="24c63-116">String</span></span>|<span data-ttu-id="24c63-117">Das Zertifikat der Base64-codierten management</span><span class="sxs-lookup"><span data-stu-id="24c63-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="24c63-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="24c63-118">Relationships</span></span>
<span data-ttu-id="24c63-119">Keine</span><span class="sxs-lookup"><span data-stu-id="24c63-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24c63-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="24c63-120">JSON Representation</span></span>
<span data-ttu-id="24c63-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="24c63-121">Here is a JSON representation of the resource.</span></span>
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




