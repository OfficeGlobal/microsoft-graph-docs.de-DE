---
title: customSubjectAlternativeName-Ressourcentyp
description: Definition des benutzerdefinierten Alternativen AntragsTellernamens
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b1583a88a52a626803fe45837e056ec020b05e2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146214"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="a353d-103">customSubjectAlternativeName-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="a353d-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="a353d-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a353d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a353d-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a353d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a353d-106">Definition des benutzerdefinierten Alternativen AntragsTellernamens</span><span class="sxs-lookup"><span data-stu-id="a353d-106">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="a353d-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a353d-107">Properties</span></span>
|<span data-ttu-id="a353d-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a353d-108">Property</span></span>|<span data-ttu-id="a353d-109">Typ</span><span class="sxs-lookup"><span data-stu-id="a353d-109">Type</span></span>|<span data-ttu-id="a353d-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a353d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a353d-111">sanType</span><span class="sxs-lookup"><span data-stu-id="a353d-111">sanType</span></span>|[<span data-ttu-id="a353d-112">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="a353d-112">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="a353d-113">Benutzerdefinierter SAN-Typ.</span><span class="sxs-lookup"><span data-stu-id="a353d-113">Custom SAN Type.</span></span> <span data-ttu-id="a353d-114">Mögliche Werte: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="a353d-114">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="a353d-115">name</span><span class="sxs-lookup"><span data-stu-id="a353d-115">name</span></span>|<span data-ttu-id="a353d-116">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a353d-116">String</span></span>|<span data-ttu-id="a353d-117">Benutzerdefinierter SAN-Name</span><span class="sxs-lookup"><span data-stu-id="a353d-117">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="a353d-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="a353d-118">Relationships</span></span>
<span data-ttu-id="a353d-119">Keine</span><span class="sxs-lookup"><span data-stu-id="a353d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a353d-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a353d-120">JSON Representation</span></span>
<span data-ttu-id="a353d-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a353d-121">Here is a JSON representation of the resource.</span></span>
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




