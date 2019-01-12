---
title: Nationale Cloudbereitstellungen
description: Zusätzlich zu unserem globalen Netzwerk von Rechenzentren sind Microsoft Cloud Services in drei separaten nationalen Clouds verfügbar. Diese nationalen Cloudversionen sind physische und logische netzwerkisolierte Instanzen von Microsoft Enterprise Cloud Services, die an die geografischen Grenzen von bestimmten Ländern gebunden sind und von lokalen Mitarbeitern betrieben werden. Weitere Informationen hierzu finden Sie unter „Nationale Clouds von Microsoft“.
localization_priority: Priority
ms.openlocfilehash: b22fce675bc97d0f22833d89dab01afd18e06032
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840418"
---
# <a name="national-cloud-deployments"></a><span data-ttu-id="868d9-105">Nationale Cloudbereitstellungen</span><span class="sxs-lookup"><span data-stu-id="868d9-105">National cloud deployments</span></span>


<span data-ttu-id="868d9-106">Zusätzlich zu unserem globalen Netzwerk von Rechenzentren sind Microsoft Cloud Services in drei separaten nationalen Clouds verfügbar.</span><span class="sxs-lookup"><span data-stu-id="868d9-106">In addition to our global network of datacenters, Microsoft cloud services are available in three separate national clouds.</span></span> <span data-ttu-id="868d9-107">Diese nationalen Cloudversionen sind physische und logische netzwerkisolierte Instanzen von Microsoft Enterprise Cloud Services, die an die geografischen Grenzen von bestimmten Ländern gebunden sind und von lokalen Mitarbeitern betrieben werden.</span><span class="sxs-lookup"><span data-stu-id="868d9-107">These national cloud versions are physical and logical network-isolated instances of Microsoft enterprise cloud services, which are confined within the geographic borders of specific countries and operated by local personnel.</span></span> <span data-ttu-id="868d9-108">Weitere Informationen hierzu finden Sie unter [Nationale Clouds von Microsoft](https://www.microsoft.com/de-DE/TrustCenter/CloudServices/NationalCloud).</span><span class="sxs-lookup"><span data-stu-id="868d9-108">To learn more, see [Microsoft National Clouds](https://www.microsoft.com/de-DE/TrustCenter/CloudServices/NationalCloud).</span></span>

<span data-ttu-id="868d9-109">Aktuelle nationale Wolken umfassen Folgendes:</span><span class="sxs-lookup"><span data-stu-id="868d9-109">Current national clouds include:</span></span>

- <span data-ttu-id="868d9-110">Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="868d9-110">Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="868d9-111">Microsoft Cloud Deutschland</span><span class="sxs-lookup"><span data-stu-id="868d9-111">Microsoft Cloud Germany</span></span>
- <span data-ttu-id="868d9-112">Azure und Office 365, betrieben von 21Vianet in China</span><span class="sxs-lookup"><span data-stu-id="868d9-112">Azure and Office 365 operated by 21Vianet in China</span></span>

<span data-ttu-id="868d9-113">Dieser Artikel enthält Informationen über die unterschiedlichen nationalen Cloudbereitstellungen von Microsoft Graph und die Features in jeder Bereitstellung, die Entwicklern zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="868d9-113">This article provides information about the different national cloud deployments of Microsoft Graph and the capabilities within each deployment that are available to developers.</span></span>

## <a name="microsoft-graph-and-microsoft-graph-explorer-service-root-endpoints"></a><span data-ttu-id="868d9-114">Dienststammendpunkte von Microsoft Graph und Microsoft Graph-Tester</span><span class="sxs-lookup"><span data-stu-id="868d9-114">Microsoft Graph and Microsoft Graph Explorer service root endpoints</span></span>

<span data-ttu-id="868d9-115">Die folgende Tabelle zeigt die Dienststammendpunkte für Microsoft Graph und Microsoft Graph-Tester für jede nationale Cloud.</span><span class="sxs-lookup"><span data-stu-id="868d9-115">The following table shows the service root endpoints for Microsoft Graph and Microsoft Graph Explorer for each National cloud.</span></span>

| <span data-ttu-id="868d9-116">Nationale Cloud</span><span class="sxs-lookup"><span data-stu-id="868d9-116">National Cloud</span></span> | <span data-ttu-id="868d9-117">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="868d9-117">Microsoft Graph</span></span> | <span data-ttu-id="868d9-118">Microsoft Graph-Tester</span><span class="sxs-lookup"><span data-stu-id="868d9-118">Microsoft Graph Explorer</span></span>
|---------------------------|----------------|----------------|
| <span data-ttu-id="868d9-119">Microsoft Graph China betrieben von 21Vianet</span><span class="sxs-lookup"><span data-stu-id="868d9-119">Microsoft Graph China operated by 21Vianet</span></span> | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| <span data-ttu-id="868d9-120">Microsoft Graph Deutschland</span><span class="sxs-lookup"><span data-stu-id="868d9-120">Microsoft Graph Germany</span></span> | https://graph.microsoft.de | <span data-ttu-id="868d9-121">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="868d9-121">Not supported.</span></span> |
| <span data-ttu-id="868d9-122">Microsoft Graph für die US-Regierung</span><span class="sxs-lookup"><span data-stu-id="868d9-122">Microsoft Graph for US Government</span></span> | https://graph.microsoft.com | <span data-ttu-id="868d9-123">Nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="868d9-123">Not supported.</span></span> |
| <span data-ttu-id="868d9-124">Microsoft Graph weltweiter Service</span><span class="sxs-lookup"><span data-stu-id="868d9-124">Microsoft Graph global service</span></span> | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> <span data-ttu-id="868d9-125">**Vermerk**:Apps können nur über die nationalen Cloudendpunkte auf Organisationsdaten zugreifen.</span><span class="sxs-lookup"><span data-stu-id="868d9-125">**Note**: Apps can only access organizational data through the national cloud endpoints.</span></span> <span data-ttu-id="868d9-126">Dies bedeutet, dass nur auf Daten in Mandanten zugegriffen werden kann, die in der jeweiligen nationalen Cloud registriert sind.</span><span class="sxs-lookup"><span data-stu-id="868d9-126">This means that only data in tenants registered in the specific national cloud can be accessed.</span></span> <span data-ttu-id="868d9-127">Apps, die versuchen, über Microsoft Graph auf Benutzerdaten zuzugreifen, denen persönliche Microsoft-Konten zugeordnet sind, sollten den weltweiten Service verwenden (https://graph.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="868d9-127">Apps that are trying to access consumer data associated with personal Microsoft accounts through Microsoft Graph should use the global service (https://graph.microsoft.com).</span></span> <span data-ttu-id="868d9-128">Zugriffstoken, die für eine nationale Cloudbereitstellung erworben wurden, können nicht mit Token ausgetauscht werden, die für den weltweiten Service erworben wurden.</span><span class="sxs-lookup"><span data-stu-id="868d9-128">Access tokens acquired for a national cloud deployment are not interchangeable with those acquired for the global service.</span></span>

## <a name="azure-ad-openid-connect-and-oauth20-endpoints"></a><span data-ttu-id="868d9-129">Endpunkte für Azure AD OpenID Connect und OAuth2.0</span><span class="sxs-lookup"><span data-stu-id="868d9-129">Azure AD OpenID Connect and OAuth2.0 endpoints</span></span>

<span data-ttu-id="868d9-130">In der folgenden Tabelle sind die Basis-URLs für die Azure Active Directory (Azure AD)-Endpunkte aufgeführt, die zum Erwerben von Token zum Aufrufen von Microsoft Graph für jede nationale Cloud verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="868d9-130">The following table lists the base URLs for the Azure Active Directory (Azure AD) endpoints used to acquire tokens to call Microsoft Graph for each national cloud.</span></span>

| <span data-ttu-id="868d9-131">Nationale Cloud</span><span class="sxs-lookup"><span data-stu-id="868d9-131">National Cloud</span></span> | <span data-ttu-id="868d9-132">Azure AD-Stammendpunkt</span><span class="sxs-lookup"><span data-stu-id="868d9-132">Azure AD root endpoint</span></span> |
|---------------------------|----------------|
| <span data-ttu-id="868d9-133">Azure AD China von 21vianet bedient</span><span class="sxs-lookup"><span data-stu-id="868d9-133">Azure AD China operated by 21Vianet</span></span> |https://login.chinacloudapi.cn |
| <span data-ttu-id="868d9-134">Azure AD Deutschland</span><span class="sxs-lookup"><span data-stu-id="868d9-134">Azure AD Germany</span></span> | https://login.microsoftonline.de |
| <span data-ttu-id="868d9-135">Azure AD für die US Regierung</span><span class="sxs-lookup"><span data-stu-id="868d9-135">Azure AD for US Government</span></span> | https://login.microsoftonline.us |
| <span data-ttu-id="868d9-136">Azure AD (weltweiter Service)</span><span class="sxs-lookup"><span data-stu-id="868d9-136">Azure AD (global service)</span></span> | https://login.microsoftonline.com |

<span data-ttu-id="868d9-p104">Anforderungen an die Azure AD-Autorisierungs- oder Tokenendpunkte können mit der entsprechenden regionsspezifischen Basis-URL gebildet werden. Zum Beispiel für Deutschland:</span><span class="sxs-lookup"><span data-stu-id="868d9-p104">Requests to the Azure AD authorization or token endpoints can be formed using the appropriate region-specific base URL. For example, for Germany:</span></span>

- <span data-ttu-id="868d9-139">Der allgemeine Endpunkt für die Autorisierung ist https://login.microsoftonline.de/common/oauth2/authorize.</span><span class="sxs-lookup"><span data-stu-id="868d9-139">The authorization common endpoint is https://login.microsoftonline.de/common/oauth2/authorize.</span></span>
- <span data-ttu-id="868d9-140">Der allgemeine Endpunkt für das Token ist https://login.microsoftonline.de/common/oauth2/token.</span><span class="sxs-lookup"><span data-stu-id="868d9-140">The token common endpoint is https://login.microsoftonline.de/common/oauth2/token.</span></span>

<span data-ttu-id="868d9-p105">Mandantenspezifische Endpunkte können gebildet werden, indem die allgemeine Variable in den URLs oben entweder durch die Mandanten-ID oder durch eine verifizierte Domäne für den Mandanten ersetzt wird. Ob Sie die allgemeinen oder mandantenspezifischen Endpunkte verwenden, ist von den Anforderungen Ihrer App und dem Authentifizierungsfluss abhängig, den Sie zum Abrufen von Token verwenden. Weitere Informationen zu Azure AD-Zugriffstoken und Microsoft Graph finden Sie unter [Authentifizierungstoken abrufen](./auth-overview.md).</span><span class="sxs-lookup"><span data-stu-id="868d9-p105">Tenant-specific endpoints can be formed by replacing "common" in the URLs above with either the tenant ID or a verified domain for the tenant. Whether you use the common or tenant-specific endpoints will depend upon the requirements of your app and the authentication flow you are using to get tokens. To learn more about Azure AD access tokens and Microsoft Graph, see [Get auth tokens](./auth-overview.md).</span></span>

> <span data-ttu-id="868d9-144">**Hinweis:** Die [Autorisierungs- und Tokenendpunkte von Azure AD, Version 2.0](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-appmodel-v2-overview/) sind nur für den globalen Dienst verfügbar. Sie werden noch nicht für die Verwendung mit nationalen Cloudbereitstellungen unterstützt.</span><span class="sxs-lookup"><span data-stu-id="868d9-144">**Note:** The [Azure AD v2.0 authorization and token endpoints](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-appmodel-v2-overview/) are available on the global service only; they are not yet supported for use with national cloud deployments.</span></span>

## <a name="supported-features"></a><span data-ttu-id="868d9-145">Unterstützte Features</span><span class="sxs-lookup"><span data-stu-id="868d9-145">Supported features</span></span>

<span data-ttu-id="868d9-146">Die folgenden Microsoft Graph-Features sind im Allgemeinen in allen nationalen Cloudbereitstellungen (im `/v1.0`-Endpunkt) verfügbar, sofern nicht anders angegeben:</span><span class="sxs-lookup"><span data-stu-id="868d9-146">The following Microsoft Graph features are generally available (on the `/v1.0` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="868d9-147">Benutzer</span><span class="sxs-lookup"><span data-stu-id="868d9-147">Users</span></span>
* <span data-ttu-id="868d9-148">Gruppen</span><span class="sxs-lookup"><span data-stu-id="868d9-148">Groups</span></span>
* <span data-ttu-id="868d9-149">Excel (wird nur beschränkt auf Microsoft Graph, betrieben von 21Vianet in China, unterstützt)</span><span class="sxs-lookup"><span data-stu-id="868d9-149">Excel (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="868d9-150">OneDrive (wird nur beschränkt auf Microsoft Graph, betrieben von 21Vianet in China, unterstützt)</span><span class="sxs-lookup"><span data-stu-id="868d9-150">OneDrive (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="868d9-151">Outlook Mail</span><span class="sxs-lookup"><span data-stu-id="868d9-151">Outlook Mail</span></span>
* <span data-ttu-id="868d9-152">Outlook-Kalender</span><span class="sxs-lookup"><span data-stu-id="868d9-152">Outlook Calendar</span></span>
* <span data-ttu-id="868d9-153">Private Kontakte</span><span class="sxs-lookup"><span data-stu-id="868d9-153">Personal Contacts</span></span> 
* <span data-ttu-id="868d9-154">SharePoint (wird nur beschränkt auf Microsoft Graph, betrieben von 21Vianet in China, unterstützt)</span><span class="sxs-lookup"><span data-stu-id="868d9-154">SharePoint (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="868d9-155">Delta-Abfrage (Support variiert bei verschiedenen Ressourcen in jeder nationalen Cloudbereitstellung).</span><span class="sxs-lookup"><span data-stu-id="868d9-155">Delta query (Support varies across different resources on each national cloud deployment.)</span></span>
* <span data-ttu-id="868d9-156">Webhooks (Support variiert bei verschiedenen Ressourcen in jeder nationalen Cloudbereitstellung).</span><span class="sxs-lookup"><span data-stu-id="868d9-156">Webhooks (Support varies across different resources on each national cloud deployment.)</span></span>

<span data-ttu-id="868d9-157">Die folgenden zusätzlichen Microsoft Graph-Features sind in allen nationalen Cloudbereitstellungen (im `/beta`-Endpunkt) in der Vorschau verfügbar, sofern nicht anders angegeben:</span><span class="sxs-lookup"><span data-stu-id="868d9-157">The following addtional Microsoft Graph features are available in preview (on the `/beta` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="868d9-158">Organisationskontakte</span><span class="sxs-lookup"><span data-stu-id="868d9-158">Organizational Contacts</span></span>
* <span data-ttu-id="868d9-159">Anwendungen</span><span class="sxs-lookup"><span data-stu-id="868d9-159">Applications</span></span>
* <span data-ttu-id="868d9-160">Dienstprinzipale</span><span class="sxs-lookup"><span data-stu-id="868d9-160">Service Principals</span></span>

<span data-ttu-id="868d9-161">Die folgenden Microsoft Graph-Features werden in nationalen Cloudbereitstellungen noch nicht unterstützt:</span><span class="sxs-lookup"><span data-stu-id="868d9-161">The following Microsoft Graph features are not yet supported on national cloud deployments:</span></span>

* <span data-ttu-id="868d9-162">Microsoft Planner</span><span class="sxs-lookup"><span data-stu-id="868d9-162">Microsoft Planner</span></span>
* <span data-ttu-id="868d9-163">Verzeichnisschemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="868d9-163">Directory schema extensions</span></span>
* <span data-ttu-id="868d9-164">Offene Typerweiterungen</span><span class="sxs-lookup"><span data-stu-id="868d9-164">Open type extensions</span></span>
