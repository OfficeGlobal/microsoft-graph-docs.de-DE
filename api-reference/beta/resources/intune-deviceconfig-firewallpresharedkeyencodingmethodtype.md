---
title: FirewallPreSharedKeyEncodingMethodType Enum-Typ
description: Mögliche Werte für firewallPreSharedKeyEncodingMethod
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 577925f141c6dd94b493664d3617df939d19c5c6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410952"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="978e3-103">FirewallPreSharedKeyEncodingMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="978e3-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="978e3-104">**Wichtig:** APIs unter der /beta Version von Microsoft Graph werden können geändert.</span><span class="sxs-lookup"><span data-stu-id="978e3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="978e3-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="978e3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="978e3-106">**Hinweis:** Die Microsoft Graph-API für Intune ist eine [aktive Intune-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten erforderlich.</span><span class="sxs-lookup"><span data-stu-id="978e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="978e3-107">Mögliche Werte für firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="978e3-107">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="978e3-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="978e3-108">Members</span></span>
|<span data-ttu-id="978e3-109">Member</span><span class="sxs-lookup"><span data-stu-id="978e3-109">Member</span></span>|<span data-ttu-id="978e3-110">Wert</span><span class="sxs-lookup"><span data-stu-id="978e3-110">Value</span></span>|<span data-ttu-id="978e3-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="978e3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="978e3-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="978e3-112">deviceDefault</span></span>|<span data-ttu-id="978e3-113">0</span><span class="sxs-lookup"><span data-stu-id="978e3-113">0</span></span>|<span data-ttu-id="978e3-114">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="978e3-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="978e3-115">Keine</span><span class="sxs-lookup"><span data-stu-id="978e3-115">none</span></span>|<span data-ttu-id="978e3-116">1</span><span class="sxs-lookup"><span data-stu-id="978e3-116">1</span></span>|<span data-ttu-id="978e3-117">Vorinstallierter Schlüssel ist nicht codiert.</span><span class="sxs-lookup"><span data-stu-id="978e3-117">Preshared key is not encoded.</span></span> <span data-ttu-id="978e3-118">Stattdessen wird es in seinem Breitzeichen-Format gespeichert</span><span class="sxs-lookup"><span data-stu-id="978e3-118">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="978e3-119">utF8</span><span class="sxs-lookup"><span data-stu-id="978e3-119">utF8</span></span>|<span data-ttu-id="978e3-120">2</span><span class="sxs-lookup"><span data-stu-id="978e3-120">2</span></span>|<span data-ttu-id="978e3-121">Vorinstallierten Schlüssel mit UTF-8-Codierung</span><span class="sxs-lookup"><span data-stu-id="978e3-121">Encode the preshared key using UTF-8</span></span>|




