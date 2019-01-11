---
title: Ressourcentyp deviceDetail
description: Gibt Gerätedetails zugeordnete eines Geräts zum Anmelden an. Enthält Informationen wie Gerätebrowser und Betriebssystem Info, wenn Gerät Azure AD verwaltet wird.
localization_priority: Normal
ms.openlocfilehash: ca4679a8c484b6dc5b36ef39d3d6d039537cbdbb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884840"
---
# <a name="devicedetail-resource-type"></a><span data-ttu-id="86ce0-104">Ressourcentyp deviceDetail</span><span class="sxs-lookup"><span data-stu-id="86ce0-104">deviceDetail resource type</span></span>
<span data-ttu-id="86ce0-105">Gibt Gerätedetails zugeordnete eines Geräts zum Anmelden an.</span><span class="sxs-lookup"><span data-stu-id="86ce0-105">Indicates device details associated with a device used for signing in.</span></span> <span data-ttu-id="86ce0-106">Enthält Informationen wie Gerätebrowser und Betriebssystem Info, wenn Gerät Azure AD verwaltet wird.</span><span class="sxs-lookup"><span data-stu-id="86ce0-106">Includes information like device browser and  OS info, if device is Azure AD managed.</span></span>



## <a name="properties"></a><span data-ttu-id="86ce0-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="86ce0-107">Properties</span></span>
| <span data-ttu-id="86ce0-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="86ce0-108">Property</span></span>     | <span data-ttu-id="86ce0-109">Typ</span><span class="sxs-lookup"><span data-stu-id="86ce0-109">Type</span></span>   |<span data-ttu-id="86ce0-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="86ce0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86ce0-111">Browser</span><span class="sxs-lookup"><span data-stu-id="86ce0-111">browser</span></span>|<span data-ttu-id="86ce0-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86ce0-112">String</span></span>|<span data-ttu-id="86ce0-113">Gibt die Browserinformationen an der die verwendeten für die Anmeldung.</span><span class="sxs-lookup"><span data-stu-id="86ce0-113">Indicates the browser information of the used for signing-in.</span></span>|
|<span data-ttu-id="86ce0-114">deviceId</span><span class="sxs-lookup"><span data-stu-id="86ce0-114">deviceId</span></span>|<span data-ttu-id="86ce0-115">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86ce0-115">String</span></span>|<span data-ttu-id="86ce0-116">Bezieht sich auf die UniqueID des Geräts für die Anmeldung verwendet.</span><span class="sxs-lookup"><span data-stu-id="86ce0-116">Refers to the UniqueID of the device used for signing-in.</span></span>|
|<span data-ttu-id="86ce0-117">displayName</span><span class="sxs-lookup"><span data-stu-id="86ce0-117">displayName</span></span>|<span data-ttu-id="86ce0-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86ce0-118">String</span></span>|<span data-ttu-id="86ce0-119">Bezieht sich auf den Namen des Geräts für die Anmeldung verwendet.</span><span class="sxs-lookup"><span data-stu-id="86ce0-119">Refers to the name of the device used for signing-in.</span></span>|
|<span data-ttu-id="86ce0-120">isCompliant</span><span class="sxs-lookup"><span data-stu-id="86ce0-120">isCompliant</span></span>|<span data-ttu-id="86ce0-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="86ce0-121">Boolean</span></span>|<span data-ttu-id="86ce0-122">Gibt an, ob das Gerät kompatibel ist.</span><span class="sxs-lookup"><span data-stu-id="86ce0-122">Indicates whether the device is compliant or not.</span></span>|
|<span data-ttu-id="86ce0-123">isManaged</span><span class="sxs-lookup"><span data-stu-id="86ce0-123">isManaged</span></span>|<span data-ttu-id="86ce0-124">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="86ce0-124">Boolean</span></span>|<span data-ttu-id="86ce0-125">Gibt an, ob das Gerät oder nicht verwaltet ist.</span><span class="sxs-lookup"><span data-stu-id="86ce0-125">Indicates if the device is managed or not.</span></span>|
|<span data-ttu-id="86ce0-126">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="86ce0-126">operatingSystem</span></span>|<span data-ttu-id="86ce0-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86ce0-127">String</span></span>|<span data-ttu-id="86ce0-128">Gibt an, der Name des Betriebssystems und die Version für die Anmeldung verwendet.</span><span class="sxs-lookup"><span data-stu-id="86ce0-128">Indicates the OS name and version used for signing-in.</span></span>|
|<span data-ttu-id="86ce0-129">trustType</span><span class="sxs-lookup"><span data-stu-id="86ce0-129">trustType</span></span>|<span data-ttu-id="86ce0-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="86ce0-130">String</span></span>|<span data-ttu-id="86ce0-131">Gibt an, ob das Gerät angemeldet ist Jahrestag beigetreten AzureAD beigetreten ist, ist die Domäne eingebundener Informationen.</span><span class="sxs-lookup"><span data-stu-id="86ce0-131">Indicates information on whether the signed-in device is Workplace Joined, AzureAD Joined, Domain Joined.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="86ce0-132">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="86ce0-132">JSON representation</span></span>

<span data-ttu-id="86ce0-133">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="86ce0-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "browser": "String",
  "deviceId": "String",
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "operatingSystem": "String",
  "trustType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
