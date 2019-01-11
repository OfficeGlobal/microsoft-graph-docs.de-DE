---
title: auditActor-Ressourcentyp
description: Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 14b4ce53d46897a84da8fab468ba2ad6aa99b30e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820048"
---
# <a name="auditactor-resource-type"></a><span data-ttu-id="b97e7-103">auditActor-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b97e7-103">auditActor resource type</span></span>

> <span data-ttu-id="b97e7-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b97e7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b97e7-105">Eine Klasse, die die Eigenschaften für den Audit-Akteur enthält.</span><span class="sxs-lookup"><span data-stu-id="b97e7-105">A class containing the properties for Audit Actor.</span></span>
## <a name="properties"></a><span data-ttu-id="b97e7-106">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="b97e7-106">Properties</span></span>
|<span data-ttu-id="b97e7-107">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b97e7-107">Property</span></span>|<span data-ttu-id="b97e7-108">Typ</span><span class="sxs-lookup"><span data-stu-id="b97e7-108">Type</span></span>|<span data-ttu-id="b97e7-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b97e7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b97e7-110">type</span><span class="sxs-lookup"><span data-stu-id="b97e7-110">type</span></span>|<span data-ttu-id="b97e7-111">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b97e7-111">String</span></span>|<span data-ttu-id="b97e7-112">Akteurtyp</span><span class="sxs-lookup"><span data-stu-id="b97e7-112">Actor Type.</span></span>|
|<span data-ttu-id="b97e7-113">userPermissions</span><span class="sxs-lookup"><span data-stu-id="b97e7-113">userPermissions</span></span>|<span data-ttu-id="b97e7-114">Zeichenfolgenauflistung</span><span class="sxs-lookup"><span data-stu-id="b97e7-114">String collection</span></span>|<span data-ttu-id="b97e7-115">Liste der Benutzerberechtigungen, nachdem die Überwachung ausgeführt wurde.</span><span class="sxs-lookup"><span data-stu-id="b97e7-115">List of user permissions when the audit was performed.</span></span>|
|<span data-ttu-id="b97e7-116">applicationId</span><span class="sxs-lookup"><span data-stu-id="b97e7-116">applicationId</span></span>|<span data-ttu-id="b97e7-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b97e7-117">String</span></span>|<span data-ttu-id="b97e7-118">AAD-Anwendungs-ID</span><span class="sxs-lookup"><span data-stu-id="b97e7-118">AAD Application Id.</span></span>|
|<span data-ttu-id="b97e7-119">applicationDisplayName</span><span class="sxs-lookup"><span data-stu-id="b97e7-119">applicationDisplayName</span></span>|<span data-ttu-id="b97e7-120">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b97e7-120">String</span></span>|<span data-ttu-id="b97e7-121">Anwendungsname</span><span class="sxs-lookup"><span data-stu-id="b97e7-121">Name of the Application.</span></span>|
|<span data-ttu-id="b97e7-122">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b97e7-122">userPrincipalName</span></span>|<span data-ttu-id="b97e7-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b97e7-123">String</span></span>|<span data-ttu-id="b97e7-124">Benutzerprinzipalname (User Principal Name, UPN)</span><span class="sxs-lookup"><span data-stu-id="b97e7-124">User Principal Name (UPN).</span></span>|
|<span data-ttu-id="b97e7-125">servicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="b97e7-125">servicePrincipalName</span></span>|<span data-ttu-id="b97e7-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b97e7-126">String</span></span>|<span data-ttu-id="b97e7-127">Dienstprinzipalnamen (Service Principal Name, SPN)</span><span class="sxs-lookup"><span data-stu-id="b97e7-127">Service Principal Name (SPN).</span></span>|
|<span data-ttu-id="b97e7-128">ipAddress</span><span class="sxs-lookup"><span data-stu-id="b97e7-128">ipAddress</span></span>|<span data-ttu-id="b97e7-129">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b97e7-129">String</span></span>|<span data-ttu-id="b97e7-130">IP-Adresse</span><span class="sxs-lookup"><span data-stu-id="b97e7-130">IPAddress.</span></span>|
|<span data-ttu-id="b97e7-131">userId</span><span class="sxs-lookup"><span data-stu-id="b97e7-131">userId</span></span>|<span data-ttu-id="b97e7-132">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b97e7-132">String</span></span>|<span data-ttu-id="b97e7-133">Benutzer-ID</span><span class="sxs-lookup"><span data-stu-id="b97e7-133">User Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b97e7-134">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="b97e7-134">Relationships</span></span>
<span data-ttu-id="b97e7-135">Keine</span><span class="sxs-lookup"><span data-stu-id="b97e7-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b97e7-136">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="b97e7-136">JSON Representation</span></span>
<span data-ttu-id="b97e7-137">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="b97e7-137">Here is a JSON representation of the resource.</span></span>
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



