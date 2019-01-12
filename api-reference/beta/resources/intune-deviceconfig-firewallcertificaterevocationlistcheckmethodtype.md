---
title: FirewallCertificateRevocationListCheckMethodType Enum-Typ
description: Mögliche Werte für firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 915fab77e7a2c28ab9d6902f3e1cb7d2d05cb2b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958411"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="acea8-103">FirewallCertificateRevocationListCheckMethodType Enum-Typ</span><span class="sxs-lookup"><span data-stu-id="acea8-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="acea8-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="acea8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="acea8-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="acea8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="acea8-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://go.microsoft.com/fwlink/?linkid=839381) ist.</span><span class="sxs-lookup"><span data-stu-id="acea8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="acea8-107">Mögliche Werte für firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="acea8-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="acea8-108">Elemente</span><span class="sxs-lookup"><span data-stu-id="acea8-108">Members</span></span>
|<span data-ttu-id="acea8-109">Element</span><span class="sxs-lookup"><span data-stu-id="acea8-109">Member</span></span>|<span data-ttu-id="acea8-110">Wert</span><span class="sxs-lookup"><span data-stu-id="acea8-110">Value</span></span>|<span data-ttu-id="acea8-111">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="acea8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="acea8-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="acea8-112">deviceDefault</span></span>|<span data-ttu-id="acea8-113">0</span><span class="sxs-lookup"><span data-stu-id="acea8-113">0</span></span>|<span data-ttu-id="acea8-114">Überschreiben Sie keinen Wert von Intune, konfiguriert nicht den Standardwert für den Benutzer konfigurierten Gerät</span><span class="sxs-lookup"><span data-stu-id="acea8-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="acea8-115">n/v</span><span class="sxs-lookup"><span data-stu-id="acea8-115">none</span></span>|<span data-ttu-id="acea8-116">1</span><span class="sxs-lookup"><span data-stu-id="acea8-116">1</span></span>|<span data-ttu-id="acea8-117">Zertifikatsperrliste nicht prüfen</span><span class="sxs-lookup"><span data-stu-id="acea8-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="acea8-118">Versuchen Sie</span><span class="sxs-lookup"><span data-stu-id="acea8-118">attempt</span></span>|<span data-ttu-id="acea8-119">2</span><span class="sxs-lookup"><span data-stu-id="acea8-119">2</span></span>|<span data-ttu-id="acea8-120">Versuchen Sie Zertifikatsperrlistenprüfung und zulassen Sie ein Zertifikat nur, wenn das Zertifikat mithilfe der Kontrollkästchen bestätigt wird</span><span class="sxs-lookup"><span data-stu-id="acea8-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="acea8-121">erfordern</span><span class="sxs-lookup"><span data-stu-id="acea8-121">require</span></span>|<span data-ttu-id="acea8-122">3</span><span class="sxs-lookup"><span data-stu-id="acea8-122">3</span></span>|<span data-ttu-id="acea8-123">Erfordern Sie eine erfolgreiche Zertifikatsperrlistenprüfung, bevor Sie ein Zertifikat</span><span class="sxs-lookup"><span data-stu-id="acea8-123">Require a successful CRL check before allowing a certificate</span></span>|





