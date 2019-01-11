---
title: FirewallCertificateRevocationListCheckMethodType Enum-Typ
description: Mögliche Werte für firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c300b1d3c73cc4ae19ef1282c00d00800243b4b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889278"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="4a055-103">FirewallCertificateRevocationListCheckMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="4a055-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="4a055-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="4a055-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a055-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="4a055-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a055-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="4a055-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a055-107">Mögliche Werte für firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="4a055-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="4a055-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="4a055-108">Members</span></span>
|<span data-ttu-id="4a055-109">Element</span><span class="sxs-lookup"><span data-stu-id="4a055-109">Member</span></span>|<span data-ttu-id="4a055-110">Wert</span><span class="sxs-lookup"><span data-stu-id="4a055-110">Value</span></span>|<span data-ttu-id="4a055-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4a055-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a055-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="4a055-112">deviceDefault</span></span>|<span data-ttu-id="4a055-113">0</span><span class="sxs-lookup"><span data-stu-id="4a055-113">0</span></span>|<span data-ttu-id="4a055-114">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="4a055-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="4a055-115">n/v</span><span class="sxs-lookup"><span data-stu-id="4a055-115">none</span></span>|<span data-ttu-id="4a055-116">1</span><span class="sxs-lookup"><span data-stu-id="4a055-116">1</span></span>|<span data-ttu-id="4a055-117">Zertifikatsperrliste nicht prüfen</span><span class="sxs-lookup"><span data-stu-id="4a055-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="4a055-118">Versuchen Sie</span><span class="sxs-lookup"><span data-stu-id="4a055-118">attempt</span></span>|<span data-ttu-id="4a055-119">2</span><span class="sxs-lookup"><span data-stu-id="4a055-119">2</span></span>|<span data-ttu-id="4a055-120">Versuchen Sie Zertifikatsperrlistenprüfung und zulassen Sie ein Zertifikat nur, wenn das Zertifikat mithilfe der Kontrollkästchen bestätigt wird</span><span class="sxs-lookup"><span data-stu-id="4a055-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="4a055-121">erfordern</span><span class="sxs-lookup"><span data-stu-id="4a055-121">require</span></span>|<span data-ttu-id="4a055-122">3</span><span class="sxs-lookup"><span data-stu-id="4a055-122">3</span></span>|<span data-ttu-id="4a055-123">Erfordern Sie eine erfolgreiche Zertifikatsperrlistenprüfung, bevor Sie ein Zertifikat</span><span class="sxs-lookup"><span data-stu-id="4a055-123">Require a successful CRL check before allowing a certificate</span></span>|





