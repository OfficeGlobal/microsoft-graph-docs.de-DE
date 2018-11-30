---
title: Ressourcentyp extendedKeyUsage
description: Benutzerdefinierte erweiterte Schlüsselverwendung definition
ms.openlocfilehash: bbf869dd32c384a12aa8e80e8a3b5984e699de48
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27058196"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="857e4-103">Ressourcentyp extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="857e4-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="857e4-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="857e4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="857e4-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="857e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="857e4-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="857e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="857e4-107">Benutzerdefinierte erweiterte Schlüsselverwendung definition</span><span class="sxs-lookup"><span data-stu-id="857e4-107">Custom Extended Key Usage definition</span></span>
## <a name="properties"></a><span data-ttu-id="857e4-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="857e4-108">Properties</span></span>
|<span data-ttu-id="857e4-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="857e4-109">Property</span></span>|<span data-ttu-id="857e4-110">Typ</span><span class="sxs-lookup"><span data-stu-id="857e4-110">Type</span></span>|<span data-ttu-id="857e4-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="857e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="857e4-112">name</span><span class="sxs-lookup"><span data-stu-id="857e4-112">name</span></span>|<span data-ttu-id="857e4-113">String</span><span class="sxs-lookup"><span data-stu-id="857e4-113">String</span></span>|<span data-ttu-id="857e4-114">Erweiterte Schlüsselverwendung Name</span><span class="sxs-lookup"><span data-stu-id="857e4-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="857e4-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="857e4-115">objectIdentifier</span></span>|<span data-ttu-id="857e4-116">String</span><span class="sxs-lookup"><span data-stu-id="857e4-116">String</span></span>|<span data-ttu-id="857e4-117">Erweiterte Schlüsselverwendung Objektbezeichner</span><span class="sxs-lookup"><span data-stu-id="857e4-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="857e4-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="857e4-118">Relationships</span></span>
<span data-ttu-id="857e4-119">Keine</span><span class="sxs-lookup"><span data-stu-id="857e4-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="857e4-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="857e4-120">JSON Representation</span></span>
<span data-ttu-id="857e4-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="857e4-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.extendedKeyUsage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.extendedKeyUsage",
  "name": "String",
  "objectIdentifier": "String"
}
```





