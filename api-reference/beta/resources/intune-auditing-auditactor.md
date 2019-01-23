---
title: auditActor-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: fcb9ededd9d1a2bb93f970f9f0da0c41a248e840
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425799"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="0fd70-103">auditActor-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="0fd70-103">auditActor resource type</span></span>

> <span data-ttu-id="0fd70-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="0fd70-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0fd70-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0fd70-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0fd70-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0fd70-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fd70-107">Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.</span><span class="sxs-lookup"><span data-stu-id="0fd70-107">A class containing the properties for Audit Actor.</span></span>

## <a name="properties"></a><span data-ttu-id="0fd70-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="0fd70-108">Properties</span></span>
|<span data-ttu-id="0fd70-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0fd70-109">Property</span></span>|<span data-ttu-id="0fd70-110">Typ</span><span class="sxs-lookup"><span data-stu-id="0fd70-110">Type</span></span>|<span data-ttu-id="0fd70-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0fd70-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fd70-112">type</span><span class="sxs-lookup"><span data-stu-id="0fd70-112">type</span></span>|<span data-ttu-id="0fd70-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0fd70-113">String</span></span>|<span data-ttu-id="0fd70-114">Akteurtyp</span><span class="sxs-lookup"><span data-stu-id="0fd70-114">Actor Type.</span></span>|
|<span data-ttu-id="0fd70-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="0fd70-115">userPermissions</span></span>|<span data-ttu-id="0fd70-116">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="0fd70-116">String collection</span></span>|<span data-ttu-id="0fd70-117">Liste der Benutzerberechtigungen, nachdem die Überwachung ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="0fd70-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="0fd70-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="0fd70-118">applicationId</span></span>|<span data-ttu-id="0fd70-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0fd70-119">String</span></span>|<span data-ttu-id="0fd70-120">AAD-Anwendungs-ID</span><span class="sxs-lookup"><span data-stu-id="0fd70-120">AAD Application Id.</span></span>|
|<span data-ttu-id="0fd70-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="0fd70-121">applicationDisplayName</span></span>|<span data-ttu-id="0fd70-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0fd70-122">String</span></span>|<span data-ttu-id="0fd70-123">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="0fd70-123">Name of the Application.</span></span>|
|<span data-ttu-id="0fd70-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0fd70-124">userPrincipalName</span></span>|<span data-ttu-id="0fd70-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0fd70-125">String</span></span>|<span data-ttu-id="0fd70-126">Benutzerprinzipalname (User Principal Name, UPN)</span><span class="sxs-lookup"><span data-stu-id="0fd70-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="0fd70-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="0fd70-127">servicePrincipalName</span></span>|<span data-ttu-id="0fd70-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0fd70-128">String</span></span>|<span data-ttu-id="0fd70-129">Dienstprinzipalnamen (Service Principal Name, SPN)</span><span class="sxs-lookup"><span data-stu-id="0fd70-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="0fd70-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="0fd70-130">ipAddress</span></span>|<span data-ttu-id="0fd70-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0fd70-131">String</span></span>|<span data-ttu-id="0fd70-132">IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="0fd70-132">IPAddress.</span></span>|
|<span data-ttu-id="0fd70-133">userId</span><span class="sxs-lookup"><span data-stu-id="0fd70-133">userId</span></span>|<span data-ttu-id="0fd70-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0fd70-134">String</span></span>|<span data-ttu-id="0fd70-135">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="0fd70-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fd70-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="0fd70-136">Relationships</span></span>
<span data-ttu-id="0fd70-137">Keine</span><span class="sxs-lookup"><span data-stu-id="0fd70-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fd70-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="0fd70-138">JSON Representation</span></span>
<span data-ttu-id="0fd70-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="0fd70-139">Here is a JSON representation of the resource.</span></span>
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




