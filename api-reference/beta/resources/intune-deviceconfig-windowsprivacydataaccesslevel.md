---
title: WindowsPrivacyDataAccessLevel Enum-Typ
description: Bestimmen Sie die Zugriffsebene für bestimmte Kategorie von Windows private Daten.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 64db5eb78708a0cfa835bd695ba01b2c267fc4fd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959316"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="9bf8c-103">WindowsPrivacyDataAccessLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="9bf8c-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="9bf8c-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="9bf8c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bf8c-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="9bf8c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9bf8c-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="9bf8c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9bf8c-107">Bestimmen Sie die Zugriffsebene für bestimmte Kategorie von Windows private Daten.</span><span class="sxs-lookup"><span data-stu-id="9bf8c-107">Determine the access level to specific Windows privacy data category.</span></span>
## <a name="members"></a><span data-ttu-id="9bf8c-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="9bf8c-108">Members</span></span>
|<span data-ttu-id="9bf8c-109">Element</span><span class="sxs-lookup"><span data-stu-id="9bf8c-109">Member</span></span>|<span data-ttu-id="9bf8c-110">Wert</span><span class="sxs-lookup"><span data-stu-id="9bf8c-110">Value</span></span>|<span data-ttu-id="9bf8c-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="9bf8c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bf8c-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="9bf8c-112">notConfigured</span></span>|<span data-ttu-id="9bf8c-113">0</span><span class="sxs-lookup"><span data-stu-id="9bf8c-113">0</span></span>|<span data-ttu-id="9bf8c-114">Keine Zugriffsebene angegeben, keine Intents.</span><span class="sxs-lookup"><span data-stu-id="9bf8c-114">No access level specified, no intents.</span></span> <span data-ttu-id="9bf8c-115">Gerät kann entweder wie in UserInControl oder ForceAllow Verhalten.</span><span class="sxs-lookup"><span data-stu-id="9bf8c-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="9bf8c-116">Es kann die private Daten abhängen wurde Zugriff auf Windows-Versionen und anderen Faktoren.</span><span class="sxs-lookup"><span data-stu-id="9bf8c-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="9bf8c-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="9bf8c-117">forceAllow</span></span>|<span data-ttu-id="9bf8c-118">1</span><span class="sxs-lookup"><span data-stu-id="9bf8c-118">1</span></span>|<span data-ttu-id="9bf8c-119">Apps dürfen die angegebenen private Daten zugreifen.</span><span class="sxs-lookup"><span data-stu-id="9bf8c-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="9bf8c-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="9bf8c-120">forceDeny</span></span>|<span data-ttu-id="9bf8c-121">2</span><span class="sxs-lookup"><span data-stu-id="9bf8c-121">2</span></span>|<span data-ttu-id="9bf8c-122">Apps werden für den angegebenen Datenschutzinformationen Zugriff auf verweigert.</span><span class="sxs-lookup"><span data-stu-id="9bf8c-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="9bf8c-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="9bf8c-123">userInControl</span></span>|<span data-ttu-id="9bf8c-124">3</span><span class="sxs-lookup"><span data-stu-id="9bf8c-124">3</span></span>|<span data-ttu-id="9bf8c-125">Benutzer werden aufgefordert, wenn apps auf angegebenen Datenschutzinformationen zugreifen.</span><span class="sxs-lookup"><span data-stu-id="9bf8c-125">Users will be prompted when apps try to access specified privacy data.</span></span>|





