---
title: Ressourcentyp appIdentity
description: Gibt die Identität der Anwendung, die die Aktion ausgeführt oder wurde geändert. Enthält Anwendungs-Id, Name, Dienstprinzipalnamen-ID und Name. Diese Ressource wird von der DirectoryAudit API aufgerufen.
localization_priority: Normal
ms.openlocfilehash: ec61782fca0ab4004fab5a55bd4774c0d64afb3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855783"
---
# <a name="appidentity-resource-type"></a><span data-ttu-id="a5f2a-105">Ressourcentyp appIdentity</span><span class="sxs-lookup"><span data-stu-id="a5f2a-105">appIdentity resource type</span></span>
<span data-ttu-id="a5f2a-106">Gibt die Identität der Anwendung, die die Aktion ausgeführt oder wurde geändert.</span><span class="sxs-lookup"><span data-stu-id="a5f2a-106">Indicates the identity of the application that performed the action or was changed.</span></span> <span data-ttu-id="a5f2a-107">Enthält Anwendungs-Id, Name, Dienstprinzipalnamen-ID und Name.</span><span class="sxs-lookup"><span data-stu-id="a5f2a-107">Includes Application Id, Name, Service Principal ID and Name.</span></span> <span data-ttu-id="a5f2a-108">Diese Ressource wird von der [DirectoryAudit](../api/directoryaudit-get.md) API aufgerufen.</span><span class="sxs-lookup"><span data-stu-id="a5f2a-108">This resource is called by the [directoryAudit](../api/directoryaudit-get.md) API</span></span>


## <a name="properties"></a><span data-ttu-id="a5f2a-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="a5f2a-109">Properties</span></span>
| <span data-ttu-id="a5f2a-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5f2a-110">Property</span></span>     | <span data-ttu-id="a5f2a-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a5f2a-111">Type</span></span>   |<span data-ttu-id="a5f2a-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5f2a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5f2a-113">appId</span><span class="sxs-lookup"><span data-stu-id="a5f2a-113">appId</span></span>|<span data-ttu-id="a5f2a-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5f2a-114">String</span></span>|<span data-ttu-id="a5f2a-115">Bezieht sich auf die eindeutige GUID, die Id der Anwendung in Azure Active Directory darstellt.</span><span class="sxs-lookup"><span data-stu-id="a5f2a-115">Refers to the Unique GUID representing Application Id in the Azure Active Directory.</span></span>|
|<span data-ttu-id="a5f2a-116">displayName</span><span class="sxs-lookup"><span data-stu-id="a5f2a-116">displayName</span></span>|<span data-ttu-id="a5f2a-117">String</span><span class="sxs-lookup"><span data-stu-id="a5f2a-117">String</span></span>|<span data-ttu-id="a5f2a-118">Bezieht sich auf den Namen der Anwendung in der Azure-Verwaltungsportal angezeigt.</span><span class="sxs-lookup"><span data-stu-id="a5f2a-118">Refers to the Application Name displayed in the Azure Portal.</span></span>|
|<span data-ttu-id="a5f2a-119">servicePrincipalId</span><span class="sxs-lookup"><span data-stu-id="a5f2a-119">servicePrincipalId</span></span>|<span data-ttu-id="a5f2a-120">String</span><span class="sxs-lookup"><span data-stu-id="a5f2a-120">String</span></span>|<span data-ttu-id="a5f2a-121">Bezieht sich auf die eindeutige GUID, die für die entsprechenden App Service Principal-Id in Azure Active Directory angibt.</span><span class="sxs-lookup"><span data-stu-id="a5f2a-121">Refers to the Unique GUID indicating Service Principal Id in Azure Active Directory for the corresponding App.</span></span>|
|<span data-ttu-id="a5f2a-122">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="a5f2a-122">servicePrincipalName</span></span>|<span data-ttu-id="a5f2a-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="a5f2a-123">String</span></span>|<span data-ttu-id="a5f2a-124">Bezieht sich auf der Service Principal Name ist der Name der Anwendung im Mandanten.</span><span class="sxs-lookup"><span data-stu-id="a5f2a-124">Refers to the Service Principal Name is the Application name in the tenant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a5f2a-125">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="a5f2a-125">JSON representation</span></span>

<span data-ttu-id="a5f2a-126">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="a5f2a-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appIdentity"
}-->

```json
{
  "appId": "String",
  "displayName": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appIdentity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
