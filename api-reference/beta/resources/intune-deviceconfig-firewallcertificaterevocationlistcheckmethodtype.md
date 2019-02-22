---
title: firewallCertificateRevocationListCheckMethodType-Enumerationstyp
description: Mögliche Werte für firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74989961978ddd10f2c14e57cfe31e25ac831703
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170077"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="3df8c-103">firewallCertificateRevocationListCheckMethodType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="3df8c-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="3df8c-104">**Wichtig:** Microsoft Graph-APIs unter der/Beta-Version können geändert werden; die Produktion wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="3df8c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3df8c-105">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="3df8c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3df8c-106">Mögliche Werte für firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="3df8c-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="3df8c-107">Elemente</span><span class="sxs-lookup"><span data-stu-id="3df8c-107">Members</span></span>
|<span data-ttu-id="3df8c-108">Element</span><span class="sxs-lookup"><span data-stu-id="3df8c-108">Member</span></span>|<span data-ttu-id="3df8c-109">Wert</span><span class="sxs-lookup"><span data-stu-id="3df8c-109">Value</span></span>|<span data-ttu-id="3df8c-110">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="3df8c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3df8c-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3df8c-111">deviceDefault</span></span>|<span data-ttu-id="3df8c-112">0</span><span class="sxs-lookup"><span data-stu-id="3df8c-112">0</span></span>|<span data-ttu-id="3df8c-113">Kein von InTune konfigurierter Wert, außer Kraft setzen des Standardwerts des Benutzer konfigurierten Geräts</span><span class="sxs-lookup"><span data-stu-id="3df8c-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="3df8c-114">Keine</span><span class="sxs-lookup"><span data-stu-id="3df8c-114">none</span></span>|<span data-ttu-id="3df8c-115">1</span><span class="sxs-lookup"><span data-stu-id="3df8c-115">1</span></span>|<span data-ttu-id="3df8c-116">Zertifikatsperrliste nicht überprüfen</span><span class="sxs-lookup"><span data-stu-id="3df8c-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="3df8c-117">Versuch</span><span class="sxs-lookup"><span data-stu-id="3df8c-117">attempt</span></span>|<span data-ttu-id="3df8c-118">2</span><span class="sxs-lookup"><span data-stu-id="3df8c-118">2</span></span>|<span data-ttu-id="3df8c-119">Versuchen Sie die Zertifikatsperrlistenüberprüfung und lassen Sie ein Zertifikat nur zu, wenn es von der Prüfung bestätigt wird.</span><span class="sxs-lookup"><span data-stu-id="3df8c-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="3df8c-120">erfordern</span><span class="sxs-lookup"><span data-stu-id="3df8c-120">require</span></span>|<span data-ttu-id="3df8c-121">3</span><span class="sxs-lookup"><span data-stu-id="3df8c-121">3</span></span>|<span data-ttu-id="3df8c-122">Erfolgreiche CRL-Überprüfung erfordern, bevor ein Zertifikat zugelassen wird</span><span class="sxs-lookup"><span data-stu-id="3df8c-122">Require a successful CRL check before allowing a certificate</span></span>|




