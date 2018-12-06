---
title: Nationale Cloudbereitstellungen
description: Zusätzlich zu unserem globalen Netzwerk von Rechenzentren sind Microsoft Cloud Services in drei separaten nationalen Clouds verfügbar. Diese nationalen Cloudversionen sind physische und logische netzwerkisolierte Instanzen von Microsoft Enterprise Cloud Services, die an die geografischen Grenzen von bestimmten Ländern gebunden sind und von lokalen Mitarbeitern betrieben werden. Weitere Informationen hierzu finden Sie unter „Nationale Clouds von Microsoft“.
ms.openlocfilehash: b0f2ab257773faa14fe59566992bb1ed0dd77959
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092162"
---
# <a name="national-cloud-deployments"></a>Nationale Cloudbereitstellungen


Zusätzlich zu unserem globalen Netzwerk von Rechenzentren sind Microsoft Cloud Services in drei separaten nationalen Clouds verfügbar. Diese nationalen Cloudversionen sind physische und logische netzwerkisolierte Instanzen von Microsoft Enterprise Cloud Services, die an die geografischen Grenzen von bestimmten Ländern gebunden sind und von lokalen Mitarbeitern betrieben werden. Weitere Informationen hierzu finden Sie unter [Nationale Clouds von Microsoft](https://www.microsoft.com/de-DE/TrustCenter/CloudServices/NationalCloud).

Aktuelle nationale Wolken umfassen Folgendes:

- Microsoft Cloud for US Government
- Microsoft Cloud Deutschland
- Azure und Office 365, betrieben von 21Vianet in China

Dieser Artikel enthält Informationen über die unterschiedlichen nationalen Cloudbereitstellungen von Microsoft Graph und die Features in jeder Bereitstellung, die Entwicklern zur Verfügung stehen.

## <a name="microsoft-graph-and-microsoft-graph-explorer-service-root-endpoints"></a>Dienststammendpunkte von Microsoft Graph und Microsoft Graph-Tester

Die folgende Tabelle zeigt die Dienststammendpunkte für Microsoft Graph und Microsoft Graph-Tester für jede nationale Cloud.

| Nationale Cloud | Microsoft Graph | Microsoft Graph-Tester
|---------------------------|----------------|----------------|
| Microsoft Graph China betrieben von 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Microsoft Graph Deutschland | https://graph.microsoft.de | Nicht unterstützt. |
| Microsoft Graph für die US-Regierung | https://graph.microsoft.com | Nicht unterstützt. |
| Microsoft Graph weltweiter Service | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> **Vermerk**:Apps können nur über die nationalen Cloudendpunkte auf Organisationsdaten zugreifen. Dies bedeutet, dass nur auf Daten in Mandanten zugegriffen werden kann, die in der jeweiligen nationalen Cloud registriert sind. Apps, die versuchen, über Microsoft Graph auf Benutzerdaten zuzugreifen, denen persönliche Microsoft-Konten zugeordnet sind, sollten den weltweiten Service verwenden (https://graph.microsoft.com). Zugriffstoken, die für eine nationale Cloudbereitstellung erworben wurden, können nicht mit Token ausgetauscht werden, die für den weltweiten Service erworben wurden.

## <a name="azure-ad-openid-connect-and-oauth20-endpoints"></a>Endpunkte für Azure AD OpenID Connect und OAuth2.0

In der folgenden Tabelle sind die Basis-URLs für die Azure Active Directory (Azure AD)-Endpunkte aufgeführt, die zum Erwerben von Token zum Aufrufen von Microsoft Graph für jede nationale Cloud verwendet werden.

| Nationale Cloud | Azure AD-Stammendpunkt |
|---------------------------|----------------|
| Azure AD China von 21vianet bedient |https://login.chinacloudapi.cn |
| Azure AD Deutschland | https://login.microsoftonline.de |
| Azure AD für die US Regierung | https://login.microsoftonline.us |
| Azure AD (weltweiter Service) | https://login.microsoftonline.com |

Anforderungen an die Azure AD-Autorisierungs- oder Tokenendpunkte können mit der entsprechenden regionsspezifischen Basis-URL gebildet werden. Zum Beispiel für Deutschland:

- Der allgemeine Endpunkt für die Autorisierung ist https://login.microsoftonline.de/common/oauth2/authorize.
- Der allgemeine Endpunkt für das Token ist https://login.microsoftonline.de/common/oauth2/token.

Mandantenspezifische Endpunkte können gebildet werden, indem die allgemeine Variable in den URLs oben entweder durch die Mandanten-ID oder durch eine verifizierte Domäne für den Mandanten ersetzt wird. Ob Sie die allgemeinen oder mandantenspezifischen Endpunkte verwenden, ist von den Anforderungen Ihrer App und dem Authentifizierungsfluss abhängig, den Sie zum Abrufen von Token verwenden. Weitere Informationen zu Azure AD-Zugriffstoken und Microsoft Graph finden Sie unter [Authentifizierungstoken abrufen](./auth-overview.md).

> **Hinweis:** Die [Autorisierungs- und Tokenendpunkte von Azure AD, Version 2.0](https://azure.microsoft.com/de-DE/documentation/articles/active-directory-appmodel-v2-overview/) sind nur für den globalen Dienst verfügbar. Sie werden noch nicht für die Verwendung mit nationalen Cloudbereitstellungen unterstützt.

## <a name="supported-features"></a>Unterstützte Features

Die folgenden Microsoft Graph-Features sind im Allgemeinen in allen nationalen Cloudbereitstellungen (im `/v1.0`-Endpunkt) verfügbar, sofern nicht anders angegeben:

* Benutzer
* Gruppen
* Excel (wird nur beschränkt auf Microsoft Graph, betrieben von 21Vianet in China, unterstützt)
* OneDrive (wird nur beschränkt auf Microsoft Graph, betrieben von 21Vianet in China, unterstützt)
* Outlook Mail
* Outlook-Kalender
* Private Kontakte 
* SharePoint (wird nur beschränkt auf Microsoft Graph, betrieben von 21Vianet in China, unterstützt)
* Delta-Abfrage (Support variiert bei verschiedenen Ressourcen in jeder nationalen Cloudbereitstellung).
* Webhooks (Support variiert bei verschiedenen Ressourcen in jeder nationalen Cloudbereitstellung).

Die folgenden zusätzlichen Microsoft Graph-Features sind in allen nationalen Cloudbereitstellungen (im `/beta`-Endpunkt) in der Vorschau verfügbar, sofern nicht anders angegeben:

* Organisationskontakte
* Anwendungen
* Dienstprinzipale

Die folgenden Microsoft Graph-Features werden in nationalen Cloudbereitstellungen noch nicht unterstützt:

* Microsoft Planner
* Verzeichnisschemaerweiterungen
* Offene Typerweiterungen
