---
title: EdgeTelemetryMode Enum-Typ
description: Typ der Suchdaten an Microsoft 365 Analytics gesendet
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 81d429f7629a5d6a6f2593785605902065d9f1c7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430092"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="adad2-103">EdgeTelemetryMode Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="adad2-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="adad2-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="adad2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="adad2-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="adad2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="adad2-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="adad2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adad2-107">Typ der Suchdaten an Microsoft 365 Analytics gesendet</span><span class="sxs-lookup"><span data-stu-id="adad2-107">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="adad2-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="adad2-108">Members</span></span>
|<span data-ttu-id="adad2-109">Member</span><span class="sxs-lookup"><span data-stu-id="adad2-109">Member</span></span>|<span data-ttu-id="adad2-110">Wert</span><span class="sxs-lookup"><span data-stu-id="adad2-110">Value</span></span>|<span data-ttu-id="adad2-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="adad2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adad2-112">nicht konfiguriert</span><span class="sxs-lookup"><span data-stu-id="adad2-112">notConfigured</span></span>|<span data-ttu-id="adad2-113">0</span><span class="sxs-lookup"><span data-stu-id="adad2-113">0</span></span>|<span data-ttu-id="adad2-114">Standard – keine Telemetriedaten gesammelt oder gesendet</span><span class="sxs-lookup"><span data-stu-id="adad2-114">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="adad2-115">Intranet</span><span class="sxs-lookup"><span data-stu-id="adad2-115">intranet</span></span>|<span data-ttu-id="adad2-116">1</span><span class="sxs-lookup"><span data-stu-id="adad2-116">1</span></span>|<span data-ttu-id="adad2-117">Senden von Intranet Verlauf nur zugelassen: nur Organisations-Browser Verlaufsdaten für Intranetwebsites senden</span><span class="sxs-lookup"><span data-stu-id="adad2-117">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="adad2-118">internet</span><span class="sxs-lookup"><span data-stu-id="adad2-118">internet</span></span>|<span data-ttu-id="adad2-119">2</span><span class="sxs-lookup"><span data-stu-id="adad2-119">2</span></span>|<span data-ttu-id="adad2-120">Senden von Internet-Verlauf nur zugelassen: nur senden durchsuchen Verlaufsdaten für Internetsites</span><span class="sxs-lookup"><span data-stu-id="adad2-120">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="adad2-121">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="adad2-121">intranetAndInternet</span></span>|<span data-ttu-id="adad2-122">3</span><span class="sxs-lookup"><span data-stu-id="adad2-122">3</span></span>|<span data-ttu-id="adad2-123">Senden von Intranet und Internet Verlauf zugelassen: Durchsuchen Verlaufsdaten für Intranet-und Internet senden</span><span class="sxs-lookup"><span data-stu-id="adad2-123">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|




