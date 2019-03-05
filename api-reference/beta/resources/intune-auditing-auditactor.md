---
title: auditActor-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b748eaea907bc2f763bb5567d7963c33b31bddd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141125"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="7b486-103">auditActor-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7b486-103">auditActor resource type</span></span>

> <span data-ttu-id="7b486-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7b486-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b486-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="7b486-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b486-106">Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.</span><span class="sxs-lookup"><span data-stu-id="7b486-106">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="7b486-107">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="7b486-107">Properties</span></span>
|<span data-ttu-id="7b486-108">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="7b486-108">Property</span></span>|<span data-ttu-id="7b486-109">Typ</span><span class="sxs-lookup"><span data-stu-id="7b486-109">Type</span></span>|<span data-ttu-id="7b486-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7b486-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b486-111">type</span><span class="sxs-lookup"><span data-stu-id="7b486-111">type</span></span>|<span data-ttu-id="7b486-112">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7b486-112">String</span></span>|<span data-ttu-id="7b486-113">Akteurtyp</span><span class="sxs-lookup"><span data-stu-id="7b486-113">Actor Type.</span></span>|
|<span data-ttu-id="7b486-114">userPermissions</span><span class="sxs-lookup"><span data-stu-id="7b486-114">userPermissions</span></span>|<span data-ttu-id="7b486-115">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="7b486-115">String collection</span></span>|<span data-ttu-id="7b486-116">Liste der Benutzerberechtigungen, nachdem die Überwachung ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="7b486-116">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="7b486-117">applicationId</span><span class="sxs-lookup"><span data-stu-id="7b486-117">applicationId</span></span>|<span data-ttu-id="7b486-118">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7b486-118">String</span></span>|<span data-ttu-id="7b486-119">AAD-Anwendungs-ID</span><span class="sxs-lookup"><span data-stu-id="7b486-119">AAD Application Id.</span></span>|
|<span data-ttu-id="7b486-120">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="7b486-120">applicationDisplayName</span></span>|<span data-ttu-id="7b486-121">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7b486-121">String</span></span>|<span data-ttu-id="7b486-122">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="7b486-122">Name of the Application.</span></span>|
|<span data-ttu-id="7b486-123">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7b486-123">userPrincipalName</span></span>|<span data-ttu-id="7b486-124">String</span><span class="sxs-lookup"><span data-stu-id="7b486-124">String</span></span>|<span data-ttu-id="7b486-125">Benutzerprinzipalname (User Principal Name, UPN)</span><span class="sxs-lookup"><span data-stu-id="7b486-125">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="7b486-126">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="7b486-126">servicePrincipalName</span></span>|<span data-ttu-id="7b486-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7b486-127">String</span></span>|<span data-ttu-id="7b486-128">Dienstprinzipalnamen (Service Principal Name, SPN)</span><span class="sxs-lookup"><span data-stu-id="7b486-128">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="7b486-129">ipAddress</span><span class="sxs-lookup"><span data-stu-id="7b486-129">ipAddress</span></span>|<span data-ttu-id="7b486-130">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7b486-130">String</span></span>|<span data-ttu-id="7b486-131">IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="7b486-131">IPAddress.</span></span>|
|<span data-ttu-id="7b486-132">userId</span><span class="sxs-lookup"><span data-stu-id="7b486-132">userId</span></span>|<span data-ttu-id="7b486-133">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="7b486-133">String</span></span>|<span data-ttu-id="7b486-134">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="7b486-134">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b486-135">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="7b486-135">Relationships</span></span>
<span data-ttu-id="7b486-136">Keine</span><span class="sxs-lookup"><span data-stu-id="7b486-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b486-137">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="7b486-137">JSON Representation</span></span>
<span data-ttu-id="7b486-138">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="7b486-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String"
}
```




