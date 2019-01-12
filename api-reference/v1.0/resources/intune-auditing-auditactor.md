---
title: auditActor-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ba63fd04d917a464933e749622a5abf959c2859e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948702"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="e7e9b-103">auditActor-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="e7e9b-103">auditActor resource type</span></span>

> <span data-ttu-id="e7e9b-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="e7e9b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7e9b-105">Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.</span><span class="sxs-lookup"><span data-stu-id="e7e9b-105">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="e7e9b-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="e7e9b-106">Properties</span></span>
|<span data-ttu-id="e7e9b-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="e7e9b-107">Property</span></span>|<span data-ttu-id="e7e9b-108">Typ</span><span class="sxs-lookup"><span data-stu-id="e7e9b-108">Type</span></span>|<span data-ttu-id="e7e9b-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="e7e9b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7e9b-110">type</span><span class="sxs-lookup"><span data-stu-id="e7e9b-110">type</span></span>|<span data-ttu-id="e7e9b-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e9b-111">String</span></span>|<span data-ttu-id="e7e9b-112">Akteurtyp</span><span class="sxs-lookup"><span data-stu-id="e7e9b-112">Actor Type.</span></span>|
|<span data-ttu-id="e7e9b-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="e7e9b-113">userPermissions</span></span>|<span data-ttu-id="e7e9b-114">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="e7e9b-114">String collection</span></span>|<span data-ttu-id="e7e9b-115">Liste der Benutzerberechtigungen, nachdem die Überwachung ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="e7e9b-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="e7e9b-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="e7e9b-116">applicationId</span></span>|<span data-ttu-id="e7e9b-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e9b-117">String</span></span>|<span data-ttu-id="e7e9b-118">AAD-Anwendungs-ID</span><span class="sxs-lookup"><span data-stu-id="e7e9b-118">AAD Application Id.</span></span>|
|<span data-ttu-id="e7e9b-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="e7e9b-119">applicationDisplayName</span></span>|<span data-ttu-id="e7e9b-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e9b-120">String</span></span>|<span data-ttu-id="e7e9b-121">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="e7e9b-121">Name of the Application.</span></span>|
|<span data-ttu-id="e7e9b-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e7e9b-122">userPrincipalName</span></span>|<span data-ttu-id="e7e9b-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e9b-123">String</span></span>|<span data-ttu-id="e7e9b-124">Benutzerprinzipalname (User Principal Name, UPN)</span><span class="sxs-lookup"><span data-stu-id="e7e9b-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="e7e9b-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="e7e9b-125">servicePrincipalName</span></span>|<span data-ttu-id="e7e9b-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e9b-126">String</span></span>|<span data-ttu-id="e7e9b-127">Dienstprinzipalnamen (Service Principal Name, SPN)</span><span class="sxs-lookup"><span data-stu-id="e7e9b-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="e7e9b-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="e7e9b-128">ipAddress</span></span>|<span data-ttu-id="e7e9b-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e9b-129">String</span></span>|<span data-ttu-id="e7e9b-130">IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="e7e9b-130">IPAddress.</span></span>|
|<span data-ttu-id="e7e9b-131">userId</span><span class="sxs-lookup"><span data-stu-id="e7e9b-131">userId</span></span>|<span data-ttu-id="e7e9b-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="e7e9b-132">String</span></span>|<span data-ttu-id="e7e9b-133">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="e7e9b-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7e9b-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="e7e9b-134">Relationships</span></span>
<span data-ttu-id="e7e9b-135">Keine</span><span class="sxs-lookup"><span data-stu-id="e7e9b-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e7e9b-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="e7e9b-136">JSON Representation</span></span>
<span data-ttu-id="e7e9b-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="e7e9b-137">Here is a JSON representation of the resource.</span></span>
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



