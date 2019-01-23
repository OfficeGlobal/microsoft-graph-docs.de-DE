---
title: Ressourcentyp customSubjectAlternativeName
description: Benutzerdefinierte Subject Alternative Name-definition
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3f081b37b79be45d6705d24be58ea7295b58b68
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415670"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="a28d6-103">Ressourcentyp customSubjectAlternativeName</span><span class="sxs-lookup"><span data-stu-id="a28d6-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="a28d6-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a28d6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a28d6-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a28d6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a28d6-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a28d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a28d6-107">Benutzerdefinierte Subject Alternative Name-definition</span><span class="sxs-lookup"><span data-stu-id="a28d6-107">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="a28d6-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a28d6-108">Properties</span></span>
|<span data-ttu-id="a28d6-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a28d6-109">Property</span></span>|<span data-ttu-id="a28d6-110">Typ</span><span class="sxs-lookup"><span data-stu-id="a28d6-110">Type</span></span>|<span data-ttu-id="a28d6-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a28d6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a28d6-112">sanType</span><span class="sxs-lookup"><span data-stu-id="a28d6-112">sanType</span></span>|[<span data-ttu-id="a28d6-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a28d6-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a28d6-114">Benutzerdefinierte SAN-Typ.</span><span class="sxs-lookup"><span data-stu-id="a28d6-114">Custom SAN Type.</span></span> <span data-ttu-id="a28d6-115">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a28d6-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a28d6-116">name</span><span class="sxs-lookup"><span data-stu-id="a28d6-116">name</span></span>|<span data-ttu-id="a28d6-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a28d6-117">String</span></span>|<span data-ttu-id="a28d6-118">Benutzerdefinierte SAN-Name</span><span class="sxs-lookup"><span data-stu-id="a28d6-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="a28d6-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a28d6-119">Relationships</span></span>
<span data-ttu-id="a28d6-120">Keine</span><span class="sxs-lookup"><span data-stu-id="a28d6-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a28d6-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a28d6-121">JSON Representation</span></span>
<span data-ttu-id="a28d6-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a28d6-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```




