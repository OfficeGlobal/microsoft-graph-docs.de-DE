---
title: komplexe Typen JSON
description: Komplexe Datentypen in JSON für Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 4fc4d4f53014f5b8c656cd069cadf7b19190e0f0
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366767"
---
# <a name="complex-types-json"></a><span data-ttu-id="52b26-103">komplexe Typen JSON</span><span class="sxs-lookup"><span data-stu-id="52b26-103">complex types JSON</span></span>
<span data-ttu-id="52b26-104">Dies sind die verschiedenen komplexen Typen in Dynamics 365 Business Central.</span><span class="sxs-lookup"><span data-stu-id="52b26-104">These are the various complex types in Dynamics 365 Business Central.</span></span> <span data-ttu-id="52b26-105">Sie können die Verwendung dieser komplexen Typen in den verschiedenen einzelnen Methoden anzeigen, die Sie verwenden.</span><span class="sxs-lookup"><span data-stu-id="52b26-105">You can see usage of these complex types in the various individual methods that make use of them.</span></span>

## <a name="postal-address"></a><span data-ttu-id="52b26-106">Postanschrift</span><span class="sxs-lookup"><span data-stu-id="52b26-106">Postal address</span></span>

<span data-ttu-id="52b26-107">Stellt einen komplexen Postanschrift-Typ in Dynamics 365 Business Central dar.</span><span class="sxs-lookup"><span data-stu-id="52b26-107">Represents a Postal Address complex type in Dynamics 365 Business Central.</span></span>

### <a name="properties"></a><span data-ttu-id="52b26-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="52b26-108">Properties</span></span>
| <span data-ttu-id="52b26-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="52b26-109">Property</span></span>     | <span data-ttu-id="52b26-110">Typ</span><span class="sxs-lookup"><span data-stu-id="52b26-110">Type</span></span>       |<span data-ttu-id="52b26-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="52b26-111">Description</span></span>             |
|:-------------|:---------|:-----------------------|
|<span data-ttu-id="52b26-112">street</span><span class="sxs-lookup"><span data-stu-id="52b26-112">street</span></span>        |<span data-ttu-id="52b26-113">string</span><span class="sxs-lookup"><span data-stu-id="52b26-113">string</span></span>    |<span data-ttu-id="52b26-114">Postanschrift Straße.</span><span class="sxs-lookup"><span data-stu-id="52b26-114">Postal address street.</span></span>  |
|<span data-ttu-id="52b26-115">city</span><span class="sxs-lookup"><span data-stu-id="52b26-115">city</span></span>          |<span data-ttu-id="52b26-116">string</span><span class="sxs-lookup"><span data-stu-id="52b26-116">string</span></span>    |<span data-ttu-id="52b26-117">Postanschrift Stadt.</span><span class="sxs-lookup"><span data-stu-id="52b26-117">Postal address city.</span></span>    |
|<span data-ttu-id="52b26-118">state</span><span class="sxs-lookup"><span data-stu-id="52b26-118">state</span></span>         |<span data-ttu-id="52b26-119">string</span><span class="sxs-lookup"><span data-stu-id="52b26-119">string</span></span>    |<span data-ttu-id="52b26-120">Postanschrift.</span><span class="sxs-lookup"><span data-stu-id="52b26-120">Postal address state.</span></span>   |
|<span data-ttu-id="52b26-121">countryLetterCode</span><span class="sxs-lookup"><span data-stu-id="52b26-121">countryLetterCode</span></span>|<span data-ttu-id="52b26-122">string</span><span class="sxs-lookup"><span data-stu-id="52b26-122">string</span></span> |<span data-ttu-id="52b26-123">Postanschrift Land Buchstabencode (zwei Zeichen Wort)</span><span class="sxs-lookup"><span data-stu-id="52b26-123">Postal address country letter code (two character word)</span></span>|
|<span data-ttu-id="52b26-124">postalCode</span><span class="sxs-lookup"><span data-stu-id="52b26-124">postalCode</span></span>    |<span data-ttu-id="52b26-125">string</span><span class="sxs-lookup"><span data-stu-id="52b26-125">string</span></span>    |<span data-ttu-id="52b26-126">Postanschrift PLZ</span><span class="sxs-lookup"><span data-stu-id="52b26-126">Postal address post code</span></span>|

```json
"PostalAddress" 
{ 
"street": "string",
"city": "string", 
"state": "string", 
"countryLetterCode": "string", 
"postalCode": "string" 
} 
 ```

