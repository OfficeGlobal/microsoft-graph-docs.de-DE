---
title: targetResource-Ressourcentyp – Microsoft Graph-API
description: Definiert den komplexen Typ der targetResource-entitätsressource der Microsoft Graph-API, die die Aktivität des Überwachungsprotokoll-Organisations Diensts (Mandanten) unterstützt.
author: lleonard-msft
localization_priority: Normal
ms.prod: azure-ad
ms.openlocfilehash: a03ca03e0b7105c8f07347f6ed52aa322a6fd090
ms.sourcegitcommit: e8b488f8068845522b869bf97475da7b078bee3d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/01/2019
ms.locfileid: "30342289"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="3299a-103">targetResource-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="3299a-103">targetResource resource type</span></span>

<span data-ttu-id="3299a-104">Stellt Ziel Ressourcentypen dar, die der Überwachungsaktivität zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="3299a-104">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="3299a-105">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="3299a-105">Properties</span></span>

| <span data-ttu-id="3299a-106">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="3299a-106">Property</span></span>     | <span data-ttu-id="3299a-107">Typ</span><span class="sxs-lookup"><span data-stu-id="3299a-107">Type</span></span>   |<span data-ttu-id="3299a-108">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3299a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3299a-109">id</span><span class="sxs-lookup"><span data-stu-id="3299a-109">id</span></span>|<span data-ttu-id="3299a-110">string</span><span class="sxs-lookup"><span data-stu-id="3299a-110">String</span></span>|<span data-ttu-id="3299a-111">Gibt die eindeutige ID der Ressource an.</span><span class="sxs-lookup"><span data-stu-id="3299a-111">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="3299a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="3299a-112">displayName</span></span>|<span data-ttu-id="3299a-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3299a-113">String</span></span>|<span data-ttu-id="3299a-114">Gibt den sichtbaren Namen an, der für die Ressource definiert ist.</span><span class="sxs-lookup"><span data-stu-id="3299a-114">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="3299a-115">Wird in der Regel bei der Erstellung der Ressource angegeben.</span><span class="sxs-lookup"><span data-stu-id="3299a-115">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="3299a-116">type</span><span class="sxs-lookup"><span data-stu-id="3299a-116">type</span></span>|<span data-ttu-id="3299a-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3299a-117">String</span></span>|<span data-ttu-id="3299a-118">Beschreibt den Ressourcentyp.</span><span class="sxs-lookup"><span data-stu-id="3299a-118">Describes the resource type.</span></span>  <span data-ttu-id="3299a-119">Zu den Beispiel `Application`Werten `Group`gehört `ServicePrincipal`,, `User`und.</span><span class="sxs-lookup"><span data-stu-id="3299a-119">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="3299a-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3299a-120">userPrincipalName</span></span>|<span data-ttu-id="3299a-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3299a-121">String</span></span>|<span data-ttu-id="3299a-122">Wenn **Type** auf `User`festgelegt ist, enthält dies den Benutzernamen, der die Aktion initiiert hat; `null` für andere Typen.</span><span class="sxs-lookup"><span data-stu-id="3299a-122">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="3299a-123">groupType</span><span class="sxs-lookup"><span data-stu-id="3299a-123">groupType</span></span>|<span data-ttu-id="3299a-124">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="3299a-124">String</span></span>|<span data-ttu-id="3299a-125">Wenn **Type** auf `Group`festgelegt ist, gibt dies den Gruppentyp an.</span><span class="sxs-lookup"><span data-stu-id="3299a-125">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="3299a-126">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="3299a-126">modifiedProperties</span></span>|<span data-ttu-id="3299a-127">[modifiedproperty](modifiedproperty.md) -Auflistung</span><span class="sxs-lookup"><span data-stu-id="3299a-127">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="3299a-128">Gibt den Namen, den alten Wert und den neuen Wert der einzelnen geänderten Attribute an.</span><span class="sxs-lookup"><span data-stu-id="3299a-128">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="3299a-129">Eigenschaftswerte sind vom Vorgangstyp abhängig. \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="3299a-129">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3299a-130">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="3299a-130">JSON representation</span></span>

<span data-ttu-id="3299a-131">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="3299a-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String", 
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
