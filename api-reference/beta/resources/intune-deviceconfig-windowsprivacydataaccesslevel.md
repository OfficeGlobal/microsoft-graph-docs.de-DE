---
title: WindowsPrivacyDataAccessLevel Enum-Typ
description: Bestimmen Sie die Zugriffsebene für bestimmte Kategorie von Windows private Daten.
ms.openlocfilehash: 09db03706795cc2aba4cc0c93dce87dc7069cd3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065907"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="31d43-103">WindowsPrivacyDataAccessLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="31d43-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="31d43-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="31d43-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31d43-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="31d43-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="31d43-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="31d43-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="31d43-107">Bestimmen Sie die Zugriffsebene für bestimmte Kategorie von Windows private Daten.</span><span class="sxs-lookup"><span data-stu-id="31d43-107">Determine the access level to specific Windows privacy data category.</span></span>
## <a name="members"></a><span data-ttu-id="31d43-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="31d43-108">Members</span></span>
|<span data-ttu-id="31d43-109">Element</span><span class="sxs-lookup"><span data-stu-id="31d43-109">Member</span></span>|<span data-ttu-id="31d43-110">Wert</span><span class="sxs-lookup"><span data-stu-id="31d43-110">Value</span></span>|<span data-ttu-id="31d43-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="31d43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31d43-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="31d43-112">notConfigured</span></span>|<span data-ttu-id="31d43-113">0</span><span class="sxs-lookup"><span data-stu-id="31d43-113">0</span></span>|<span data-ttu-id="31d43-114">Keine Zugriffsebene angegeben, keine Intents.</span><span class="sxs-lookup"><span data-stu-id="31d43-114">No access level specified, no intents.</span></span> <span data-ttu-id="31d43-115">Gerät kann entweder wie in UserInControl oder ForceAllow Verhalten.</span><span class="sxs-lookup"><span data-stu-id="31d43-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="31d43-116">Es kann die private Daten abhängen wurde Zugriff auf Windows-Versionen und anderen Faktoren.</span><span class="sxs-lookup"><span data-stu-id="31d43-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="31d43-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="31d43-117">forceAllow</span></span>|<span data-ttu-id="31d43-118">1</span><span class="sxs-lookup"><span data-stu-id="31d43-118">1</span></span>|<span data-ttu-id="31d43-119">Apps dürfen die angegebenen private Daten zugreifen.</span><span class="sxs-lookup"><span data-stu-id="31d43-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="31d43-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="31d43-120">forceDeny</span></span>|<span data-ttu-id="31d43-121">2</span><span class="sxs-lookup"><span data-stu-id="31d43-121">2</span></span>|<span data-ttu-id="31d43-122">Apps werden für den angegebenen Datenschutzinformationen Zugriff auf verweigert.</span><span class="sxs-lookup"><span data-stu-id="31d43-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="31d43-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="31d43-123">userInControl</span></span>|<span data-ttu-id="31d43-124">3</span><span class="sxs-lookup"><span data-stu-id="31d43-124">3</span></span>|<span data-ttu-id="31d43-125">Benutzer werden aufgefordert, wenn apps auf angegebenen Datenschutzinformationen zugreifen.</span><span class="sxs-lookup"><span data-stu-id="31d43-125">Users will be prompted when apps try to access specified privacy data.</span></span>|





