---
title: Ressourcentyp onPremisesProvisioningError
description: Stellt verzeichnissynchronisierungsfehlern für die Benutzer- und Entitäten dar, bei der lokalen Verzeichnisse zu Azure Active Directory-Synchronisierung.
localization_priority: Normal
ms.openlocfilehash: c8989a78dfb60a6c7c25a66a9f1e619dcbdca15d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830667"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="2ec6c-103">Ressourcentyp onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="2ec6c-103">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="2ec6c-104">Stellt die verzeichnissynchronisierungsfehlern für die [ [Benutzer-](user.md) und](group.md) Entitäten bei synchronisieren Verzeichnisse zu Azure Active Directory der lokale.</span><span class="sxs-lookup"><span data-stu-id="2ec6c-104">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="2ec6c-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="2ec6c-105">Properties</span></span>

| <span data-ttu-id="2ec6c-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2ec6c-106">Property</span></span> | <span data-ttu-id="2ec6c-107">Typ</span><span class="sxs-lookup"><span data-stu-id="2ec6c-107">Type</span></span> | <span data-ttu-id="2ec6c-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2ec6c-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2ec6c-109">Kategorie</span><span class="sxs-lookup"><span data-stu-id="2ec6c-109">category</span></span>|<span data-ttu-id="2ec6c-110">String</span><span class="sxs-lookup"><span data-stu-id="2ec6c-110">String</span></span>| <span data-ttu-id="2ec6c-111">Die Kategorie des Fehlers bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="2ec6c-111">Category of the provisioning error.</span></span> <span data-ttu-id="2ec6c-112">Hinweis: Zurzeit besteht nur einen möglichen Wert.</span><span class="sxs-lookup"><span data-stu-id="2ec6c-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="2ec6c-113">Wert: *PropertyConflict* - gibt ein Eigenschaftswert ist nicht eindeutig.</span><span class="sxs-lookup"><span data-stu-id="2ec6c-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="2ec6c-114">Andere Objekte enthalten den gleichen Wert für die Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="2ec6c-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="2ec6c-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="2ec6c-115">occurredDateTime</span></span>|<span data-ttu-id="2ec6c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ec6c-116">DateTimeOffset</span></span>| <span data-ttu-id="2ec6c-117">Datum und Uhrzeit, an dem der Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="2ec6c-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="2ec6c-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="2ec6c-118">propertyCausingError</span></span>|<span data-ttu-id="2ec6c-119">String</span><span class="sxs-lookup"><span data-stu-id="2ec6c-119">String</span></span>| <span data-ttu-id="2ec6c-120">Name der Verzeichniseigenschaft den Fehler verursacht.</span><span class="sxs-lookup"><span data-stu-id="2ec6c-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="2ec6c-121">Aktuelle mögliche Werte: *UserPrincipalName* oder *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="2ec6c-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="2ec6c-122">Wert</span><span class="sxs-lookup"><span data-stu-id="2ec6c-122">value</span></span>|<span data-ttu-id="2ec6c-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="2ec6c-123">String</span></span>| <span data-ttu-id="2ec6c-124">Der Wert der Eigenschaft, die den Fehler verursacht.</span><span class="sxs-lookup"><span data-stu-id="2ec6c-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2ec6c-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="2ec6c-125">JSON representation</span></span>
<span data-ttu-id="2ec6c-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="2ec6c-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
