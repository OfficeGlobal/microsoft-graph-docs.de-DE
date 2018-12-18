---
title: FirewallCertificateRevocationListCheckMethodType Enum-Typ
description: Mögliche Werte für firewallCertificateRevocationListCheckMethod
author: tfitzmac
ms.openlocfilehash: ab496b5deb8f096bdc48a2b50a1af994c8ec8d5b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353662"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="62a73-103">FirewallCertificateRevocationListCheckMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="62a73-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="62a73-104">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="62a73-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62a73-105">Mögliche Werte für firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="62a73-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="62a73-106">Elemente</span><span class="sxs-lookup"><span data-stu-id="62a73-106">Members</span></span>
|<span data-ttu-id="62a73-107">Member</span><span class="sxs-lookup"><span data-stu-id="62a73-107">Member</span></span>|<span data-ttu-id="62a73-108">Wert</span><span class="sxs-lookup"><span data-stu-id="62a73-108">Value</span></span>|<span data-ttu-id="62a73-109">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="62a73-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a73-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="62a73-110">deviceDefault</span></span>|<span data-ttu-id="62a73-111">0</span><span class="sxs-lookup"><span data-stu-id="62a73-111">0</span></span>|<span data-ttu-id="62a73-112">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="62a73-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="62a73-113">Keine</span><span class="sxs-lookup"><span data-stu-id="62a73-113">none</span></span>|<span data-ttu-id="62a73-114">1</span><span class="sxs-lookup"><span data-stu-id="62a73-114">1</span></span>|<span data-ttu-id="62a73-115">Zertifikatsperrliste nicht prüfen</span><span class="sxs-lookup"><span data-stu-id="62a73-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="62a73-116">Versuchen Sie</span><span class="sxs-lookup"><span data-stu-id="62a73-116">attempt</span></span>|<span data-ttu-id="62a73-117">2</span><span class="sxs-lookup"><span data-stu-id="62a73-117">2</span></span>|<span data-ttu-id="62a73-118">Versuchen Sie Zertifikatsperrlistenprüfung und zulassen Sie ein Zertifikat nur, wenn das Zertifikat mithilfe der Kontrollkästchen bestätigt wird</span><span class="sxs-lookup"><span data-stu-id="62a73-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="62a73-119">erfordern</span><span class="sxs-lookup"><span data-stu-id="62a73-119">require</span></span>|<span data-ttu-id="62a73-120">3</span><span class="sxs-lookup"><span data-stu-id="62a73-120">3</span></span>|<span data-ttu-id="62a73-121">Erfordern Sie eine erfolgreiche Zertifikatsperrlistenprüfung, bevor Sie ein Zertifikat</span><span class="sxs-lookup"><span data-stu-id="62a73-121">Require a successful CRL check before allowing a certificate</span></span>|



