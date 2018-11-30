---
title: Ressourcentyp windowsKioskLocalUser
description: Die Klasse verwendet, um ein lokales Konto für die Konfiguration Kiosk identifizieren
ms.openlocfilehash: 1b5b8837f4f93005dabf839a7fc20e3b05b1fbf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059726"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="23b40-103">Ressourcentyp windowsKioskLocalUser</span><span class="sxs-lookup"><span data-stu-id="23b40-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="23b40-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="23b40-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23b40-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="23b40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23b40-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="23b40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23b40-107">Die Klasse verwendet, um ein lokales Konto für die Konfiguration Kiosk identifizieren</span><span class="sxs-lookup"><span data-stu-id="23b40-107">The class used to identify a local account for the kiosk configuration</span></span>

<span data-ttu-id="23b40-108">Erbt vom [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="23b40-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23b40-109">Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="23b40-109">Properties</span></span>
|<span data-ttu-id="23b40-110">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="23b40-110">Property</span></span>|<span data-ttu-id="23b40-111">Typ</span><span class="sxs-lookup"><span data-stu-id="23b40-111">Type</span></span>|<span data-ttu-id="23b40-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="23b40-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23b40-113">userName</span><span class="sxs-lookup"><span data-stu-id="23b40-113">userName</span></span>|<span data-ttu-id="23b40-114">String</span><span class="sxs-lookup"><span data-stu-id="23b40-114">String</span></span>|<span data-ttu-id="23b40-115">Der lokale Benutzer, der mit dieser Konfiguration Kiosk gesperrt wird</span><span class="sxs-lookup"><span data-stu-id="23b40-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="23b40-116">Beziehungen</span><span class="sxs-lookup"><span data-stu-id="23b40-116">Relationships</span></span>
<span data-ttu-id="23b40-117">Keine</span><span class="sxs-lookup"><span data-stu-id="23b40-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23b40-118">JSON-Darstellung</span><span class="sxs-lookup"><span data-stu-id="23b40-118">JSON Representation</span></span>
<span data-ttu-id="23b40-119">Es folgt eine JSON-Darstellung der Ressource.</span><span class="sxs-lookup"><span data-stu-id="23b40-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```





