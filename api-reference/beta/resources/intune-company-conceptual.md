---
title: Geschäftsbedingungen in Microsoft InTune – Microsoft Graph-API
description: Listet die Microsoft Graph-API für InTune-Endpunkte (REST) auf, die die Bedingungen für eine mandantenorganisation definieren.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 1277a6893ddd306b7050fafc70b815217d376b14
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172282"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="52454-103">Geschäftsbedingungen des Unternehmens in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="52454-103">Company terms and conditions in Microsoft Intune</span></span>

> <span data-ttu-id="52454-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="52454-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52454-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="52454-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="52454-106">**Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.</span><span class="sxs-lookup"><span data-stu-id="52454-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="52454-107">Sie können die allgemeinen Geschäftsbedingungen von Intune für Benutzergruppen bereitstellen, um zu erläutern, wie sich die Registrierung, der Zugriff auf Arbeitsressourcen und die Unternehmensportal-App auf Geräte und Benutzer auswirken.</span><span class="sxs-lookup"><span data-stu-id="52454-107">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="52454-108">Benutzer müssen die allgemeinen Geschäftsbedingungen akzeptieren, bevor sie das Unternehmensportal zum Registrieren und zum Zugriff auf ihre Arbeit nutzen können.</span><span class="sxs-lookup"><span data-stu-id="52454-108">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="52454-109">Sie können mehrere Richtlinien mit unterschiedlichen allgemeinen Geschäftsbedingungen erstellen und bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="52454-109">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="52454-110">Sie können auch Versionen derselben allgemeinen Geschäftsbedingungen in verschiedenen Sprachen erstellen und für die entsprechenden Gruppen bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="52454-110">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="52454-111">Die folgenden Graph-Ressourcen stehen zur Verfügung, um die allgemeinen Geschäftsbedingungen des Unternehmens in Intune zu verwalten:</span><span class="sxs-lookup"><span data-stu-id="52454-111">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="52454-112">Geschäftsbedingungen</span><span class="sxs-lookup"><span data-stu-id="52454-112">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="52454-113">Annahmestatus der Geschäftsbedingungen</span><span class="sxs-lookup"><span data-stu-id="52454-113">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="52454-114">Zuweisung für Geschäftsbedingungen</span><span class="sxs-lookup"><span data-stu-id="52454-114">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)
- [<span data-ttu-id="52454-115">Gruppenzuweisung der Geschäftsbedingungen</span><span class="sxs-lookup"><span data-stu-id="52454-115">Terms and conditions group assignment</span></span>](intune-companyterms-termsandconditionsgroupassignment.md)
