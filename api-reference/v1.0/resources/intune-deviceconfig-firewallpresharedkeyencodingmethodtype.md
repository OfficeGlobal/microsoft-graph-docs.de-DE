---
title: FirewallPreSharedKeyEncodingMethodType Enum-Typ
description: Mögliche Werte für firewallPreSharedKeyEncodingMethod
ms.openlocfilehash: 238d2b0845b0d79ea109cea5b326914815d600de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018216"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="b8aeb-103">FirewallPreSharedKeyEncodingMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="b8aeb-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="b8aeb-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="b8aeb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8aeb-105">Mögliche Werte für firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="b8aeb-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="b8aeb-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="b8aeb-106">Members</span></span>
|<span data-ttu-id="b8aeb-107">Element</span><span class="sxs-lookup"><span data-stu-id="b8aeb-107">Member</span></span>|<span data-ttu-id="b8aeb-108">Wert</span><span class="sxs-lookup"><span data-stu-id="b8aeb-108">Value</span></span>|<span data-ttu-id="b8aeb-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8aeb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8aeb-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="b8aeb-110">deviceDefault</span></span>|<span data-ttu-id="b8aeb-111">0</span><span class="sxs-lookup"><span data-stu-id="b8aeb-111">0</span></span>|<span data-ttu-id="b8aeb-112">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="b8aeb-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="b8aeb-113">n/v</span><span class="sxs-lookup"><span data-stu-id="b8aeb-113">none</span></span>|<span data-ttu-id="b8aeb-114">1</span><span class="sxs-lookup"><span data-stu-id="b8aeb-114">1</span></span>|<span data-ttu-id="b8aeb-115">Vorinstallierter Schlüssel ist nicht codiert.</span><span class="sxs-lookup"><span data-stu-id="b8aeb-115">Preshared key is not encoded.</span></span> <span data-ttu-id="b8aeb-116">Stattdessen wird es in seinem Breitzeichen-Format gespeichert</span><span class="sxs-lookup"><span data-stu-id="b8aeb-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="b8aeb-117">utF8</span><span class="sxs-lookup"><span data-stu-id="b8aeb-117">utF8</span></span>|<span data-ttu-id="b8aeb-118">2</span><span class="sxs-lookup"><span data-stu-id="b8aeb-118">2</span></span>|<span data-ttu-id="b8aeb-119">Vorinstallierten Schlüssel mit UTF-8-Codierung</span><span class="sxs-lookup"><span data-stu-id="b8aeb-119">Encode the preshared key using UTF-8</span></span>|



