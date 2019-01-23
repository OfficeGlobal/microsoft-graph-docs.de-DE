---
title: Ressourcentyp loggedOnUser
description: Angemeldete Benutzer
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ac0ca08c6d324836e4bb9dd9951fdfe742b8b5f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395195"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="622f7-103">Ressourcentyp loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="622f7-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="622f7-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="622f7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="622f7-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="622f7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="622f7-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="622f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="622f7-107">Angemeldete Benutzer</span><span class="sxs-lookup"><span data-stu-id="622f7-107">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="622f7-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="622f7-108">Properties</span></span>
|<span data-ttu-id="622f7-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="622f7-109">Property</span></span>|<span data-ttu-id="622f7-110">Typ</span><span class="sxs-lookup"><span data-stu-id="622f7-110">Type</span></span>|<span data-ttu-id="622f7-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="622f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="622f7-112">userId</span><span class="sxs-lookup"><span data-stu-id="622f7-112">userId</span></span>|<span data-ttu-id="622f7-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="622f7-113">String</span></span>|<span data-ttu-id="622f7-114">Benutzer-id</span><span class="sxs-lookup"><span data-stu-id="622f7-114">User id</span></span>|
|<span data-ttu-id="622f7-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="622f7-115">lastLogOnDateTime</span></span>|<span data-ttu-id="622f7-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="622f7-116">DateTimeOffset</span></span>|<span data-ttu-id="622f7-117">Datum-Uhrzeit, wann Benutzer anmeldet</span><span class="sxs-lookup"><span data-stu-id="622f7-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="622f7-118">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="622f7-118">Relationships</span></span>
<span data-ttu-id="622f7-119">Keine</span><span class="sxs-lookup"><span data-stu-id="622f7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="622f7-120">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="622f7-120">JSON Representation</span></span>
<span data-ttu-id="622f7-121">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="622f7-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```




