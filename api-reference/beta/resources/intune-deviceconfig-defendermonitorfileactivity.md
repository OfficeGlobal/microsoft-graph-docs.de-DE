---
title: DefenderMonitorFileActivity Enum-Typ
description: Mögliche Werte für die Überwachung von Dateiaktivität.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d9b0f91d0a2d802fd573d7825da016dc8850e941
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414956"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="a28bb-103">DefenderMonitorFileActivity Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="a28bb-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="a28bb-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="a28bb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a28bb-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="a28bb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a28bb-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a28bb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a28bb-107">Mögliche Werte für die Überwachung von Dateiaktivität.</span><span class="sxs-lookup"><span data-stu-id="a28bb-107">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="a28bb-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="a28bb-108">Members</span></span>
|<span data-ttu-id="a28bb-109">Member</span><span class="sxs-lookup"><span data-stu-id="a28bb-109">Member</span></span>|<span data-ttu-id="a28bb-110">Wert</span><span class="sxs-lookup"><span data-stu-id="a28bb-110">Value</span></span>|<span data-ttu-id="a28bb-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a28bb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a28bb-112">vom Typ userDefined</span><span class="sxs-lookup"><span data-stu-id="a28bb-112">userDefined</span></span>|<span data-ttu-id="a28bb-113">0</span><span class="sxs-lookup"><span data-stu-id="a28bb-113">0</span></span>|<span data-ttu-id="a28bb-114">User-Defined, Standardwert, keine beabsichtigt.</span><span class="sxs-lookup"><span data-stu-id="a28bb-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="a28bb-115">disable</span><span class="sxs-lookup"><span data-stu-id="a28bb-115">disable</span></span>|<span data-ttu-id="a28bb-116">1</span><span class="sxs-lookup"><span data-stu-id="a28bb-116">1</span></span>|<span data-ttu-id="a28bb-117">Überwachen der Dateiaktivität zu deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="a28bb-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="a28bb-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="a28bb-118">monitorAllFiles</span></span>|<span data-ttu-id="a28bb-119">2</span><span class="sxs-lookup"><span data-stu-id="a28bb-119">2</span></span>|<span data-ttu-id="a28bb-120">Überwachen Sie alle Dateien.</span><span class="sxs-lookup"><span data-stu-id="a28bb-120">Monitor all files.</span></span>|
|<span data-ttu-id="a28bb-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="a28bb-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="a28bb-122">3</span><span class="sxs-lookup"><span data-stu-id="a28bb-122">3</span></span>| <span data-ttu-id="a28bb-123">Nur eingehende Dateien zu überwachen.</span><span class="sxs-lookup"><span data-stu-id="a28bb-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="a28bb-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="a28bb-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="a28bb-125">4</span><span class="sxs-lookup"><span data-stu-id="a28bb-125">4</span></span>|<span data-ttu-id="a28bb-126">Nur ausgehende Dateien zu überwachen.</span><span class="sxs-lookup"><span data-stu-id="a28bb-126">Monitor outgoing files only.</span></span>|




