---
title: FirewallCertificateRevocationListCheckMethodType Enum-Typ
description: Mögliche Werte für firewallCertificateRevocationListCheckMethod
ms.openlocfilehash: b6a7d702b1156598387c204d9e42b15f3066598d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27018758"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="8df27-103">FirewallCertificateRevocationListCheckMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="8df27-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="8df27-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="8df27-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8df27-105">Mögliche Werte für firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="8df27-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="8df27-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="8df27-106">Members</span></span>
|<span data-ttu-id="8df27-107">Element</span><span class="sxs-lookup"><span data-stu-id="8df27-107">Member</span></span>|<span data-ttu-id="8df27-108">Wert</span><span class="sxs-lookup"><span data-stu-id="8df27-108">Value</span></span>|<span data-ttu-id="8df27-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="8df27-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8df27-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="8df27-110">deviceDefault</span></span>|<span data-ttu-id="8df27-111">0</span><span class="sxs-lookup"><span data-stu-id="8df27-111">0</span></span>|<span data-ttu-id="8df27-112">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="8df27-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="8df27-113">n/v</span><span class="sxs-lookup"><span data-stu-id="8df27-113">none</span></span>|<span data-ttu-id="8df27-114">1</span><span class="sxs-lookup"><span data-stu-id="8df27-114">1</span></span>|<span data-ttu-id="8df27-115">Zertifikatsperrliste nicht prüfen</span><span class="sxs-lookup"><span data-stu-id="8df27-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="8df27-116">Versuchen Sie</span><span class="sxs-lookup"><span data-stu-id="8df27-116">attempt</span></span>|<span data-ttu-id="8df27-117">2</span><span class="sxs-lookup"><span data-stu-id="8df27-117">2</span></span>|<span data-ttu-id="8df27-118">Versuchen Sie Zertifikatsperrlistenprüfung und zulassen Sie ein Zertifikat nur, wenn das Zertifikat mithilfe der Kontrollkästchen bestätigt wird</span><span class="sxs-lookup"><span data-stu-id="8df27-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="8df27-119">erfordern</span><span class="sxs-lookup"><span data-stu-id="8df27-119">require</span></span>|<span data-ttu-id="8df27-120">3</span><span class="sxs-lookup"><span data-stu-id="8df27-120">3</span></span>|<span data-ttu-id="8df27-121">Erfordern Sie eine erfolgreiche Zertifikatsperrlistenprüfung, bevor Sie ein Zertifikat</span><span class="sxs-lookup"><span data-stu-id="8df27-121">Require a successful CRL check before allowing a certificate</span></span>|



