---
title: FirewallCertificateRevocationListCheckMethodType Enum-Typ
description: Mögliche Werte für firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2beee8f7c4f049aa1918b7e1516c3ce586a8cad0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839949"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="15fa5-103">FirewallCertificateRevocationListCheckMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="15fa5-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="15fa5-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="15fa5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15fa5-105">Mögliche Werte für firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="15fa5-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="15fa5-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="15fa5-106">Members</span></span>
|<span data-ttu-id="15fa5-107">Element</span><span class="sxs-lookup"><span data-stu-id="15fa5-107">Member</span></span>|<span data-ttu-id="15fa5-108">Wert</span><span class="sxs-lookup"><span data-stu-id="15fa5-108">Value</span></span>|<span data-ttu-id="15fa5-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="15fa5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15fa5-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="15fa5-110">deviceDefault</span></span>|<span data-ttu-id="15fa5-111">0</span><span class="sxs-lookup"><span data-stu-id="15fa5-111">0</span></span>|<span data-ttu-id="15fa5-112">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="15fa5-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="15fa5-113">n/v</span><span class="sxs-lookup"><span data-stu-id="15fa5-113">none</span></span>|<span data-ttu-id="15fa5-114">1</span><span class="sxs-lookup"><span data-stu-id="15fa5-114">1</span></span>|<span data-ttu-id="15fa5-115">Zertifikatsperrliste nicht prüfen</span><span class="sxs-lookup"><span data-stu-id="15fa5-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="15fa5-116">Versuchen Sie</span><span class="sxs-lookup"><span data-stu-id="15fa5-116">attempt</span></span>|<span data-ttu-id="15fa5-117">2</span><span class="sxs-lookup"><span data-stu-id="15fa5-117">2</span></span>|<span data-ttu-id="15fa5-118">Versuchen Sie Zertifikatsperrlistenprüfung und zulassen Sie ein Zertifikat nur, wenn das Zertifikat mithilfe der Kontrollkästchen bestätigt wird</span><span class="sxs-lookup"><span data-stu-id="15fa5-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="15fa5-119">erfordern</span><span class="sxs-lookup"><span data-stu-id="15fa5-119">require</span></span>|<span data-ttu-id="15fa5-120">3</span><span class="sxs-lookup"><span data-stu-id="15fa5-120">3</span></span>|<span data-ttu-id="15fa5-121">Erfordern Sie eine erfolgreiche Zertifikatsperrlistenprüfung, bevor Sie ein Zertifikat</span><span class="sxs-lookup"><span data-stu-id="15fa5-121">Require a successful CRL check before allowing a certificate</span></span>|



