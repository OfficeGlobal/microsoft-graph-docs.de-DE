---
title: auditActor-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 632e3018f606b62171461b4b1235ccdafc6b1b5a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254457"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="b0c25-103">auditActor-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b0c25-103">auditActor resource type</span></span>

> <span data-ttu-id="b0c25-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="b0c25-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0c25-105">Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.</span><span class="sxs-lookup"><span data-stu-id="b0c25-105">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="b0c25-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b0c25-106">Properties</span></span>
|<span data-ttu-id="b0c25-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b0c25-107">Property</span></span>|<span data-ttu-id="b0c25-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b0c25-108">Type</span></span>|<span data-ttu-id="b0c25-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b0c25-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0c25-110">type</span><span class="sxs-lookup"><span data-stu-id="b0c25-110">type</span></span>|<span data-ttu-id="b0c25-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0c25-111">String</span></span>|<span data-ttu-id="b0c25-112">Akteurtyp</span><span class="sxs-lookup"><span data-stu-id="b0c25-112">Actor Type.</span></span>|
|<span data-ttu-id="b0c25-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="b0c25-113">userPermissions</span></span>|<span data-ttu-id="b0c25-114">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b0c25-114">String collection</span></span>|<span data-ttu-id="b0c25-115">Liste der Benutzerberechtigungen, nachdem die Überwachung ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="b0c25-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="b0c25-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="b0c25-116">applicationId</span></span>|<span data-ttu-id="b0c25-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0c25-117">String</span></span>|<span data-ttu-id="b0c25-118">AAD-Anwendungs-ID</span><span class="sxs-lookup"><span data-stu-id="b0c25-118">AAD Application Id.</span></span>|
|<span data-ttu-id="b0c25-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="b0c25-119">applicationDisplayName</span></span>|<span data-ttu-id="b0c25-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0c25-120">String</span></span>|<span data-ttu-id="b0c25-121">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="b0c25-121">Name of the Application.</span></span>|
|<span data-ttu-id="b0c25-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b0c25-122">userPrincipalName</span></span>|<span data-ttu-id="b0c25-123">String</span><span class="sxs-lookup"><span data-stu-id="b0c25-123">String</span></span>|<span data-ttu-id="b0c25-124">Benutzerprinzipalname (User Principal Name, UPN)</span><span class="sxs-lookup"><span data-stu-id="b0c25-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="b0c25-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="b0c25-125">servicePrincipalName</span></span>|<span data-ttu-id="b0c25-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0c25-126">String</span></span>|<span data-ttu-id="b0c25-127">Dienstprinzipalnamen (Service Principal Name, SPN)</span><span class="sxs-lookup"><span data-stu-id="b0c25-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="b0c25-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b0c25-128">ipAddress</span></span>|<span data-ttu-id="b0c25-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0c25-129">String</span></span>|<span data-ttu-id="b0c25-130">IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="b0c25-130">IPAddress.</span></span>|
|<span data-ttu-id="b0c25-131">userId</span><span class="sxs-lookup"><span data-stu-id="b0c25-131">userId</span></span>|<span data-ttu-id="b0c25-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b0c25-132">String</span></span>|<span data-ttu-id="b0c25-133">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="b0c25-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0c25-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b0c25-134">Relationships</span></span>
<span data-ttu-id="b0c25-135">Keine</span><span class="sxs-lookup"><span data-stu-id="b0c25-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0c25-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b0c25-136">JSON Representation</span></span>
<span data-ttu-id="b0c25-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b0c25-137">Here is a JSON representation of the resource.</span></span>
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



