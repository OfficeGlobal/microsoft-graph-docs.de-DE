---
title: Ressourcentyp extendedKeyUsage
description: Benutzerdefinierte erweiterte Schlüsselverwendung definition
author: tfitzmac
ms.openlocfilehash: 2b6155a0fbb234cb0b2081a8a4a226a8d218dbc2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337289"
---
# <a name="extendedkeyusage-resource-type"></a><span data-ttu-id="835e7-103">Ressourcentyp extendedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="835e7-103">extendedKeyUsage resource type</span></span>

> <span data-ttu-id="835e7-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="835e7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="835e7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="835e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="835e7-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="835e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="835e7-107">Benutzerdefinierte erweiterte Schlüsselverwendung definition</span><span class="sxs-lookup"><span data-stu-id="835e7-107">Custom Extended Key Usage definition</span></span>
## <a name="properties"></a><span data-ttu-id="835e7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="835e7-108">Properties</span></span>
|<span data-ttu-id="835e7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="835e7-109">Property</span></span>|<span data-ttu-id="835e7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="835e7-110">Type</span></span>|<span data-ttu-id="835e7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="835e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="835e7-112">name</span><span class="sxs-lookup"><span data-stu-id="835e7-112">name</span></span>|<span data-ttu-id="835e7-113">String</span><span class="sxs-lookup"><span data-stu-id="835e7-113">String</span></span>|<span data-ttu-id="835e7-114">Erweiterte Schlüsselverwendung Name</span><span class="sxs-lookup"><span data-stu-id="835e7-114">Extended Key Usage Name</span></span>|
|<span data-ttu-id="835e7-115">objectIdentifier</span><span class="sxs-lookup"><span data-stu-id="835e7-115">objectIdentifier</span></span>|<span data-ttu-id="835e7-116">String</span><span class="sxs-lookup"><span data-stu-id="835e7-116">String</span></span>|<span data-ttu-id="835e7-117">Erweiterte Schlüsselverwendung Objektbezeichner</span><span class="sxs-lookup"><span data-stu-id="835e7-117">Extended Key Usage Object Identifier</span></span>|

## <a name="relationships"></a><span data-ttu-id="835e7-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="835e7-118">Relationships</span></span>
<span data-ttu-id="835e7-119">Keine</span><span class="sxs-lookup"><span data-stu-id="835e7-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="835e7-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="835e7-120">JSON Representation</span></span>
<span data-ttu-id="835e7-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="835e7-121">Here is a JSON representation of the resource.</span></span>
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





