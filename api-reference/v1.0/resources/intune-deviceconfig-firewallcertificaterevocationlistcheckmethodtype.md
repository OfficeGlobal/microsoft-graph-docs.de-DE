---
title: firewallCertificateRevocationListCheckMethodType-Enumerationstyp
description: Mögliche Werte für firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a475f32d4572b0aa8ed2a52befc7a58eb6077253
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257631"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="62c61-103">firewallCertificateRevocationListCheckMethodType-Enumerationstyp</span><span class="sxs-lookup"><span data-stu-id="62c61-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="62c61-104">**Hinweis:** Die Microsoft Graph-API für InTune benötigt eine [aktive INTUNE-Lizenz](https://go.microsoft.com/fwlink/?linkid=839381) für den Mandanten.</span><span class="sxs-lookup"><span data-stu-id="62c61-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62c61-105">Mögliche Werte für firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="62c61-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="62c61-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="62c61-106">Members</span></span>
|<span data-ttu-id="62c61-107">Element</span><span class="sxs-lookup"><span data-stu-id="62c61-107">Member</span></span>|<span data-ttu-id="62c61-108">Wert</span><span class="sxs-lookup"><span data-stu-id="62c61-108">Value</span></span>|<span data-ttu-id="62c61-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62c61-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62c61-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="62c61-110">deviceDefault</span></span>|<span data-ttu-id="62c61-111">0</span><span class="sxs-lookup"><span data-stu-id="62c61-111">0</span></span>|<span data-ttu-id="62c61-112">Kein von InTune konfigurierter Wert, außer Kraft setzen des Standardwerts des Benutzer konfigurierten Geräts</span><span class="sxs-lookup"><span data-stu-id="62c61-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="62c61-113">Keine</span><span class="sxs-lookup"><span data-stu-id="62c61-113">none</span></span>|<span data-ttu-id="62c61-114">1</span><span class="sxs-lookup"><span data-stu-id="62c61-114">1</span></span>|<span data-ttu-id="62c61-115">Zertifikatsperrliste nicht überprüfen</span><span class="sxs-lookup"><span data-stu-id="62c61-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="62c61-116">Versuch</span><span class="sxs-lookup"><span data-stu-id="62c61-116">attempt</span></span>|<span data-ttu-id="62c61-117">2</span><span class="sxs-lookup"><span data-stu-id="62c61-117">2</span></span>|<span data-ttu-id="62c61-118">Versuchen Sie die Zertifikatsperrlistenüberprüfung und lassen Sie ein Zertifikat nur zu, wenn es von der Prüfung bestätigt wird.</span><span class="sxs-lookup"><span data-stu-id="62c61-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="62c61-119">erfordern</span><span class="sxs-lookup"><span data-stu-id="62c61-119">require</span></span>|<span data-ttu-id="62c61-120">3</span><span class="sxs-lookup"><span data-stu-id="62c61-120">3</span></span>|<span data-ttu-id="62c61-121">Erfolgreiche CRL-Überprüfung erfordern, bevor ein Zertifikat zugelassen wird</span><span class="sxs-lookup"><span data-stu-id="62c61-121">Require a successful CRL check before allowing a certificate</span></span>|



