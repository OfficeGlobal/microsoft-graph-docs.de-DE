---
title: Ressourcentyp customSubjectAlternativeName
description: Benutzerdefinierte Subject Alternative Name-definition
ms.openlocfilehash: 14d6c24cd5e8c087b81fa51194301da522d169b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27061969"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="104af-103">Ressourcentyp customSubjectAlternativeName</span><span class="sxs-lookup"><span data-stu-id="104af-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="104af-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="104af-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="104af-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="104af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="104af-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="104af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="104af-107">Benutzerdefinierte Subject Alternative Name-definition</span><span class="sxs-lookup"><span data-stu-id="104af-107">Custom Subject Alternative Name definition</span></span>
## <a name="properties"></a><span data-ttu-id="104af-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="104af-108">Properties</span></span>
|<span data-ttu-id="104af-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="104af-109">Property</span></span>|<span data-ttu-id="104af-110">Typ</span><span class="sxs-lookup"><span data-stu-id="104af-110">Type</span></span>|<span data-ttu-id="104af-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="104af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="104af-112">sanType</span><span class="sxs-lookup"><span data-stu-id="104af-112">sanType</span></span>|[<span data-ttu-id="104af-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="104af-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="104af-114">Benutzerdefinierte SAN-Typ.</span><span class="sxs-lookup"><span data-stu-id="104af-114">Custom SAN Type.</span></span> <span data-ttu-id="104af-115">Mögliche Werte sind: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute` und `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="104af-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="104af-116">name</span><span class="sxs-lookup"><span data-stu-id="104af-116">name</span></span>|<span data-ttu-id="104af-117">String</span><span class="sxs-lookup"><span data-stu-id="104af-117">String</span></span>|<span data-ttu-id="104af-118">Benutzerdefinierte SAN-Name</span><span class="sxs-lookup"><span data-stu-id="104af-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="104af-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="104af-119">Relationships</span></span>
<span data-ttu-id="104af-120">Keine</span><span class="sxs-lookup"><span data-stu-id="104af-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="104af-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="104af-121">JSON Representation</span></span>
<span data-ttu-id="104af-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="104af-122">Here is a JSON representation of the resource.</span></span>
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





