---
title: Ressourcentyp windowsKioskAzureADUser
description: Die Klasse verwendet, um ein Benutzerkonto AzureAD für die Konfiguration Kiosk identifizieren
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08c5b53e8e208abac2801146ff70df6023eaedff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420185"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="da40c-103">Ressourcentyp windowsKioskAzureADUser</span><span class="sxs-lookup"><span data-stu-id="da40c-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="da40c-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="da40c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da40c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="da40c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da40c-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="da40c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da40c-107">Die Klasse verwendet, um ein Benutzerkonto AzureAD für die Konfiguration Kiosk identifizieren</span><span class="sxs-lookup"><span data-stu-id="da40c-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="da40c-108">Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="da40c-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="da40c-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="da40c-109">Properties</span></span>
|<span data-ttu-id="da40c-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="da40c-110">Property</span></span>|<span data-ttu-id="da40c-111">Typ</span><span class="sxs-lookup"><span data-stu-id="da40c-111">Type</span></span>|<span data-ttu-id="da40c-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="da40c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da40c-113">userId</span><span class="sxs-lookup"><span data-stu-id="da40c-113">userId</span></span>|<span data-ttu-id="da40c-114">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da40c-114">String</span></span>|<span data-ttu-id="da40c-115">Die ID des Benutzers, die mit dieser Konfiguration Kiosk gesperrt werden AzureAD</span><span class="sxs-lookup"><span data-stu-id="da40c-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="da40c-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="da40c-116">userPrincipalName</span></span>|<span data-ttu-id="da40c-117">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="da40c-117">String</span></span>|<span data-ttu-id="da40c-118">Die Benutzerkonten, die mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="da40c-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="da40c-119">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="da40c-119">Relationships</span></span>
<span data-ttu-id="da40c-120">Keine</span><span class="sxs-lookup"><span data-stu-id="da40c-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da40c-121">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="da40c-121">JSON Representation</span></span>
<span data-ttu-id="da40c-122">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="da40c-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```




