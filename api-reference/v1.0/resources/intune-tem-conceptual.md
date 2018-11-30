---
title: Verwalten von Telekommunikationsausgaben in Microsoft Intune
description: Sie können den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben nutzen, um die Datennutzung und das Roaming auf unternehmenseigenen Geräten zu beschränken. Der Service ist mit Intune integriert. Er ermöglicht es Ihnen, Nutzungslimits festzulegen und durchzusetzen. Benutzern wird eine Benachrichtigung gesendet, sobald sie einen konfigurierten Schwellenwert überschreiten. Sie können den Dienst auch so konfigurieren, dass er bestimmte Aktionen ausführt, wenn Benutzer den Schwellenwert überschreiten. So kann er beispielsweise das Roaming deaktivieren. In der Saaswedo-Konsole stehen Berichte mit Informationen zur Datennutzung und Überwachungsinformationen zur Verfügung. Bevor Sie den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben mit Intune nutzen können, müssen Sie Einstellungen in einer Saaswedo-Konsole und in Intune konfigurieren. Die Verbindung muss sowohl aufseiten das Saaswedo-Diensts als auch aufseiten von Intune aktiviert sein. Falls die Verbindung aufseiten von Saaswedo aktiviert ist, nicht aber aufseiten von Intune, empfängt Intune Meldungen, ignoriert sie jedoch.
ms.openlocfilehash: ccd917fbddec623aa590ef3b94cb561244bccd99
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27019291"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a><span data-ttu-id="f71bc-109">Verwalten von Telekommunikationsausgaben in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f71bc-109">Telecom expense management in Microsoft Intune</span></span>

> <span data-ttu-id="f71bc-110">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="f71bc-110">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="f71bc-111">Sie können den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben nutzen, um die Datennutzung und das Roaming auf unternehmenseigenen Geräten zu beschränken. Der Service ist mit Intune integriert.</span><span class="sxs-lookup"><span data-stu-id="f71bc-111">You can limit data usage and roaming on corporate-owned devices when you use the Saaswedo telecom expense management service, which integrates with Intune.</span></span> <span data-ttu-id="f71bc-112">Er ermöglicht es Ihnen, Nutzungslimits festzulegen und durchzusetzen. Benutzern wird eine Benachrichtigung gesendet, sobald sie einen konfigurierten Schwellenwert überschreiten.</span><span class="sxs-lookup"><span data-stu-id="f71bc-112">The service enables you to set and enforce usage limits and to send users an alert when they exceed a configured threshold.</span></span> <span data-ttu-id="f71bc-113">Sie können den Dienst auch so konfigurieren, dass er bestimmte Aktionen ausführt, wenn Benutzer den Schwellenwert überschreiten. So kann er beispielsweise das Roaming deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="f71bc-113">You can also configure the service to take different actions, such as disabling roaming, when users exceed the threshold.</span></span> <span data-ttu-id="f71bc-114">In der Saaswedo-Konsole stehen Berichte mit Informationen zur Datennutzung und Überwachungsinformationen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="f71bc-114">Reports that provide data usage and monitoring information are available in the Saaswedo console.</span></span> <span data-ttu-id="f71bc-115">Bevor Sie den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben mit Intune nutzen können, müssen Sie Einstellungen in einer Saaswedo-Konsole und in Intune konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="f71bc-115">Before you can use the Saaswedo telecom expense management service with Intune, you need to configure settings in a Saaswedo console and in Intune.</span></span> <span data-ttu-id="f71bc-116">Die Verbindung muss sowohl aufseiten das Saaswedo-Diensts als auch aufseiten von Intune aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="f71bc-116">The connection must be turned on for the Saaswedo service and for Intune.</span></span> <span data-ttu-id="f71bc-117">Falls die Verbindung aufseiten von Saaswedo aktiviert ist, nicht aber aufseiten von Intune, empfängt Intune Meldungen, ignoriert sie jedoch.</span><span class="sxs-lookup"><span data-stu-id="f71bc-117">If the Saaswedo side of the connection is enabled, but not the Intune side, Intune receives the communication, but ignores it.</span></span>

<span data-ttu-id="f71bc-118">Zur Verwaltung von Telekommunikationsausgaben in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:</span><span class="sxs-lookup"><span data-stu-id="f71bc-118">The following Graph resources are available to manage telecom expenses in Intune:</span></span>  

- [<span data-ttu-id="f71bc-119">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="f71bc-119">Telecom expense management partner</span></span>](intune-tem-telecomexpensemanagementpartner.md)