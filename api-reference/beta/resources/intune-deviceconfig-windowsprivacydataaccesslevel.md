---
title: WindowsPrivacyDataAccessLevel Enum-Typ
description: Bestimmen Sie die Zugriffsebene für bestimmte Kategorie von Windows private Daten.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5d6fed0897b22a6a6b478dc5d2b7954faca42b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410623"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="1bd0e-103">WindowsPrivacyDataAccessLevel Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="1bd0e-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="1bd0e-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="1bd0e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1bd0e-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="1bd0e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1bd0e-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1bd0e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1bd0e-107">Bestimmen Sie die Zugriffsebene für bestimmte Kategorie von Windows private Daten.</span><span class="sxs-lookup"><span data-stu-id="1bd0e-107">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="1bd0e-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="1bd0e-108">Members</span></span>
|<span data-ttu-id="1bd0e-109">Member</span><span class="sxs-lookup"><span data-stu-id="1bd0e-109">Member</span></span>|<span data-ttu-id="1bd0e-110">Wert</span><span class="sxs-lookup"><span data-stu-id="1bd0e-110">Value</span></span>|<span data-ttu-id="1bd0e-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1bd0e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bd0e-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="1bd0e-112">notConfigured</span></span>|<span data-ttu-id="1bd0e-113">0</span><span class="sxs-lookup"><span data-stu-id="1bd0e-113">0</span></span>|<span data-ttu-id="1bd0e-114">Keine Zugriffsebene angegeben, keine Intents.</span><span class="sxs-lookup"><span data-stu-id="1bd0e-114">No access level specified, no intents.</span></span> <span data-ttu-id="1bd0e-115">Gerät kann entweder wie in UserInControl oder ForceAllow Verhalten.</span><span class="sxs-lookup"><span data-stu-id="1bd0e-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="1bd0e-116">Es kann die private Daten abhängen wurde Zugriff auf Windows-Versionen und anderen Faktoren.</span><span class="sxs-lookup"><span data-stu-id="1bd0e-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="1bd0e-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="1bd0e-117">forceAllow</span></span>|<span data-ttu-id="1bd0e-118">1</span><span class="sxs-lookup"><span data-stu-id="1bd0e-118">1</span></span>|<span data-ttu-id="1bd0e-119">Apps dürfen die angegebenen private Daten zugreifen.</span><span class="sxs-lookup"><span data-stu-id="1bd0e-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="1bd0e-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="1bd0e-120">forceDeny</span></span>|<span data-ttu-id="1bd0e-121">2</span><span class="sxs-lookup"><span data-stu-id="1bd0e-121">2</span></span>|<span data-ttu-id="1bd0e-122">Apps werden für den angegebenen Datenschutzinformationen Zugriff auf verweigert.</span><span class="sxs-lookup"><span data-stu-id="1bd0e-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="1bd0e-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="1bd0e-123">userInControl</span></span>|<span data-ttu-id="1bd0e-124">3</span><span class="sxs-lookup"><span data-stu-id="1bd0e-124">3</span></span>|<span data-ttu-id="1bd0e-125">Benutzer werden aufgefordert, wenn apps auf angegebenen Datenschutzinformationen zugreifen.</span><span class="sxs-lookup"><span data-stu-id="1bd0e-125">Users will be prompted when apps try to access specified privacy data.</span></span>|




