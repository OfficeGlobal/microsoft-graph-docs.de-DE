---
title: Ressourcentyp onPremisesProvisioningError
description: Stellt die verzeichnissynchronisierungsfehlern für die Benutzer, Gruppe oder Organisation Kontakt Entitäten bei synchronisieren Verzeichnisse zu Azure Active Directory der lokale.
ms.openlocfilehash: 9fa7850d39c9f7a490135a127938fc7fae30b6f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27060788"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="8ad3b-103">Ressourcentyp onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="8ad3b-103">onPremisesProvisioningError resource type</span></span>

> <span data-ttu-id="8ad3b-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="8ad3b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8ad3b-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="8ad3b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8ad3b-106">Stellt die verzeichnissynchronisierungsfehlern für die [Benutzer](user.md), [Gruppe](group.md)oder [Organisation Kontakt](orgcontact.md) Entitäten bei synchronisieren Verzeichnisse zu Azure Active Directory der lokale.</span><span class="sxs-lookup"><span data-stu-id="8ad3b-106">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="8ad3b-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="8ad3b-107">Properties</span></span>

| <span data-ttu-id="8ad3b-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="8ad3b-108">Property</span></span> | <span data-ttu-id="8ad3b-109">Typ</span><span class="sxs-lookup"><span data-stu-id="8ad3b-109">Type</span></span> | <span data-ttu-id="8ad3b-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8ad3b-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8ad3b-111">Kategorie</span><span class="sxs-lookup"><span data-stu-id="8ad3b-111">category</span></span>|<span data-ttu-id="8ad3b-112">String</span><span class="sxs-lookup"><span data-stu-id="8ad3b-112">String</span></span>| <span data-ttu-id="8ad3b-113">Die Kategorie des Fehlers bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="8ad3b-113">Category of the provisioning error.</span></span> <span data-ttu-id="8ad3b-114">Hinweis: Zurzeit besteht nur einen möglichen Wert.</span><span class="sxs-lookup"><span data-stu-id="8ad3b-114">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="8ad3b-115">Wert: *PropertyConflict* - gibt ein Eigenschaftswert ist nicht eindeutig.</span><span class="sxs-lookup"><span data-stu-id="8ad3b-115">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="8ad3b-116">Andere Objekte enthalten den gleichen Wert für die Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="8ad3b-116">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="8ad3b-117">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="8ad3b-117">occurredDateTime</span></span>|<span data-ttu-id="8ad3b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ad3b-118">DateTimeOffset</span></span>| <span data-ttu-id="8ad3b-119">Datum und Uhrzeit, an dem der Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="8ad3b-119">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="8ad3b-120">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="8ad3b-120">propertyCausingError</span></span>|<span data-ttu-id="8ad3b-121">String</span><span class="sxs-lookup"><span data-stu-id="8ad3b-121">String</span></span>| <span data-ttu-id="8ad3b-122">Name der Verzeichniseigenschaft den Fehler verursacht.</span><span class="sxs-lookup"><span data-stu-id="8ad3b-122">Name of the directory property causing the error.</span></span> <span data-ttu-id="8ad3b-123">Aktuelle mögliche Werte: *UserPrincipalName* oder *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="8ad3b-123">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="8ad3b-124">Wert</span><span class="sxs-lookup"><span data-stu-id="8ad3b-124">value</span></span>|<span data-ttu-id="8ad3b-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="8ad3b-125">String</span></span>| <span data-ttu-id="8ad3b-126">Der Wert der Eigenschaft, die den Fehler verursacht.</span><span class="sxs-lookup"><span data-stu-id="8ad3b-126">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="8ad3b-127">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="8ad3b-127">JSON representation</span></span>
<span data-ttu-id="8ad3b-128">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="8ad3b-128">Here is a JSON representation of the resource.</span></span>

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