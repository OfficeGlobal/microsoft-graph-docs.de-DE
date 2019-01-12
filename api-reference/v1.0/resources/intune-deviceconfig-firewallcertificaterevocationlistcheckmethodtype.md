---
title: FirewallCertificateRevocationListCheckMethodType Enum-Typ
description: Mögliche Werte für firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e479b10339ab515a17f67d85de0c8d43c1507825
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940057"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="cd751-103">FirewallCertificateRevocationListCheckMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="cd751-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="cd751-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="cd751-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd751-105">Mögliche Werte für firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="cd751-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="cd751-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="cd751-106">Members</span></span>
|<span data-ttu-id="cd751-107">Element</span><span class="sxs-lookup"><span data-stu-id="cd751-107">Member</span></span>|<span data-ttu-id="cd751-108">Wert</span><span class="sxs-lookup"><span data-stu-id="cd751-108">Value</span></span>|<span data-ttu-id="cd751-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="cd751-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd751-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="cd751-110">deviceDefault</span></span>|<span data-ttu-id="cd751-111">0</span><span class="sxs-lookup"><span data-stu-id="cd751-111">0</span></span>|<span data-ttu-id="cd751-112">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="cd751-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="cd751-113">n/v</span><span class="sxs-lookup"><span data-stu-id="cd751-113">none</span></span>|<span data-ttu-id="cd751-114">1</span><span class="sxs-lookup"><span data-stu-id="cd751-114">1</span></span>|<span data-ttu-id="cd751-115">Zertifikatsperrliste nicht prüfen</span><span class="sxs-lookup"><span data-stu-id="cd751-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="cd751-116">Versuchen Sie</span><span class="sxs-lookup"><span data-stu-id="cd751-116">attempt</span></span>|<span data-ttu-id="cd751-117">2</span><span class="sxs-lookup"><span data-stu-id="cd751-117">2</span></span>|<span data-ttu-id="cd751-118">Versuchen Sie Zertifikatsperrlistenprüfung und zulassen Sie ein Zertifikat nur, wenn das Zertifikat mithilfe der Kontrollkästchen bestätigt wird</span><span class="sxs-lookup"><span data-stu-id="cd751-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="cd751-119">erfordern</span><span class="sxs-lookup"><span data-stu-id="cd751-119">require</span></span>|<span data-ttu-id="cd751-120">3</span><span class="sxs-lookup"><span data-stu-id="cd751-120">3</span></span>|<span data-ttu-id="cd751-121">Erfordern Sie eine erfolgreiche Zertifikatsperrlistenprüfung, bevor Sie ein Zertifikat</span><span class="sxs-lookup"><span data-stu-id="cd751-121">Require a successful CRL check before allowing a certificate</span></span>|



