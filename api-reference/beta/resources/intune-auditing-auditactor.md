---
title: auditActor-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f7d93f3a14f3f6fd1515de9232d26718b7ec0af6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971431"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="80f2f-103">auditActor-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="80f2f-103">auditActor resource type</span></span>

> <span data-ttu-id="80f2f-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="80f2f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80f2f-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="80f2f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80f2f-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="80f2f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80f2f-107">Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.</span><span class="sxs-lookup"><span data-stu-id="80f2f-107">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="80f2f-108">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="80f2f-108">Properties</span></span>
|<span data-ttu-id="80f2f-109">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="80f2f-109">Property</span></span>|<span data-ttu-id="80f2f-110">Typ</span><span class="sxs-lookup"><span data-stu-id="80f2f-110">Type</span></span>|<span data-ttu-id="80f2f-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="80f2f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80f2f-112">type</span><span class="sxs-lookup"><span data-stu-id="80f2f-112">type</span></span>|<span data-ttu-id="80f2f-113">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80f2f-113">String</span></span>|<span data-ttu-id="80f2f-114">Akteurtyp</span><span class="sxs-lookup"><span data-stu-id="80f2f-114">Actor Type.</span></span>|
|<span data-ttu-id="80f2f-115">userPermissions</span><span class="sxs-lookup"><span data-stu-id="80f2f-115">userPermissions</span></span>|<span data-ttu-id="80f2f-116">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="80f2f-116">String collection</span></span>|<span data-ttu-id="80f2f-117">Liste der Benutzerberechtigungen, nachdem die Überwachung ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="80f2f-117">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="80f2f-118">applicationId</span><span class="sxs-lookup"><span data-stu-id="80f2f-118">applicationId</span></span>|<span data-ttu-id="80f2f-119">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80f2f-119">String</span></span>|<span data-ttu-id="80f2f-120">AAD-Anwendungs-ID</span><span class="sxs-lookup"><span data-stu-id="80f2f-120">AAD Application Id.</span></span>|
|<span data-ttu-id="80f2f-121">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="80f2f-121">applicationDisplayName</span></span>|<span data-ttu-id="80f2f-122">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80f2f-122">String</span></span>|<span data-ttu-id="80f2f-123">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="80f2f-123">Name of the Application.</span></span>|
|<span data-ttu-id="80f2f-124">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="80f2f-124">userPrincipalName</span></span>|<span data-ttu-id="80f2f-125">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80f2f-125">String</span></span>|<span data-ttu-id="80f2f-126">Benutzerprinzipalname (User Principal Name, UPN)</span><span class="sxs-lookup"><span data-stu-id="80f2f-126">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="80f2f-127">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="80f2f-127">servicePrincipalName</span></span>|<span data-ttu-id="80f2f-128">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80f2f-128">String</span></span>|<span data-ttu-id="80f2f-129">Dienstprinzipalnamen (Service Principal Name, SPN)</span><span class="sxs-lookup"><span data-stu-id="80f2f-129">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="80f2f-130">ipAddress</span><span class="sxs-lookup"><span data-stu-id="80f2f-130">ipAddress</span></span>|<span data-ttu-id="80f2f-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80f2f-131">String</span></span>|<span data-ttu-id="80f2f-132">IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="80f2f-132">IPAddress.</span></span>|
|<span data-ttu-id="80f2f-133">userId</span><span class="sxs-lookup"><span data-stu-id="80f2f-133">userId</span></span>|<span data-ttu-id="80f2f-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="80f2f-134">String</span></span>|<span data-ttu-id="80f2f-135">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="80f2f-135">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80f2f-136">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="80f2f-136">Relationships</span></span>
<span data-ttu-id="80f2f-137">Keine</span><span class="sxs-lookup"><span data-stu-id="80f2f-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80f2f-138">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="80f2f-138">JSON Representation</span></span>
<span data-ttu-id="80f2f-139">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="80f2f-139">Here is a JSON representation of the resource.</span></span>
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





