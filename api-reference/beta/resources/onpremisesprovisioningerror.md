---
title: Ressourcentyp onPremisesProvisioningError
description: Stellt die verzeichnissynchronisierungsfehlern für die Benutzer, Gruppe oder Organisation Kontakt Entitäten bei synchronisieren Verzeichnisse zu Azure Active Directory der lokale.
localization_priority: Normal
ms.openlocfilehash: 7e4d51ea3bde6158256c607027b3e56236a8151c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512731"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="79d51-103">Ressourcentyp onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="79d51-103">onPremisesProvisioningError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79d51-104">Stellt die verzeichnissynchronisierungsfehlern für die [Benutzer](user.md), [Gruppe](group.md)oder [Organisation Kontakt](orgcontact.md) Entitäten bei synchronisieren Verzeichnisse zu Azure Active Directory der lokale.</span><span class="sxs-lookup"><span data-stu-id="79d51-104">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="79d51-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="79d51-105">Properties</span></span>

| <span data-ttu-id="79d51-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="79d51-106">Property</span></span> | <span data-ttu-id="79d51-107">Typ</span><span class="sxs-lookup"><span data-stu-id="79d51-107">Type</span></span> | <span data-ttu-id="79d51-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="79d51-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="79d51-109">Kategorie</span><span class="sxs-lookup"><span data-stu-id="79d51-109">category</span></span>|<span data-ttu-id="79d51-110">String</span><span class="sxs-lookup"><span data-stu-id="79d51-110">String</span></span>| <span data-ttu-id="79d51-111">Die Kategorie des Fehlers bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="79d51-111">Category of the provisioning error.</span></span> <span data-ttu-id="79d51-112">Hinweis: Zurzeit besteht nur einen möglichen Wert.</span><span class="sxs-lookup"><span data-stu-id="79d51-112">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="79d51-113">Wert: *PropertyConflict* - gibt ein Eigenschaftswert ist nicht eindeutig.</span><span class="sxs-lookup"><span data-stu-id="79d51-113">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="79d51-114">Andere Objekte enthalten den gleichen Wert für die Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="79d51-114">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="79d51-115">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="79d51-115">occurredDateTime</span></span>|<span data-ttu-id="79d51-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79d51-116">DateTimeOffset</span></span>| <span data-ttu-id="79d51-117">Datum und Uhrzeit, an dem der Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="79d51-117">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="79d51-118">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="79d51-118">propertyCausingError</span></span>|<span data-ttu-id="79d51-119">String</span><span class="sxs-lookup"><span data-stu-id="79d51-119">String</span></span>| <span data-ttu-id="79d51-120">Name der Verzeichniseigenschaft den Fehler verursacht.</span><span class="sxs-lookup"><span data-stu-id="79d51-120">Name of the directory property causing the error.</span></span> <span data-ttu-id="79d51-121">Aktuelle mögliche Werte: *UserPrincipalName* oder *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="79d51-121">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="79d51-122">Wert</span><span class="sxs-lookup"><span data-stu-id="79d51-122">value</span></span>|<span data-ttu-id="79d51-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="79d51-123">String</span></span>| <span data-ttu-id="79d51-124">Der Wert der Eigenschaft, die den Fehler verursacht.</span><span class="sxs-lookup"><span data-stu-id="79d51-124">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="79d51-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="79d51-125">JSON representation</span></span>
<span data-ttu-id="79d51-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="79d51-126">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisesprovisioningerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
