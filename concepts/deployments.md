---
title: Nationale Cloudbereitstellungen
description: Zusätzlich zu unserem globalen Netzwerk von Rechenzentren sind Microsoft Cloud Services in drei separaten nationalen Clouds verfügbar. Diese nationalen Cloudversionen sind physischen und logischen Netzwerk isoliert werden Instanzen des Microsoft Enterprise Cloud-Dienste, die vom lokalen Personal und innerhalb der geografischen Rahmen des bestimmten Ländern beschränkt.
ms.openlocfilehash: 06ca3c24cba17e2d18fc4755f00a2c754e508f88
ms.sourcegitcommit: 597dfc95a44e0f2354d056b5567bcff2bb2837f1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29892498"
---
# <a name="national-cloud-deployments"></a>Nationale Cloudbereitstellungen

Zusätzlich zu unserem globalen Netzwerk von Rechenzentren sind Microsoft Cloud Services in drei separaten nationalen Clouds verfügbar. Diese nationalen Cloudversionen sind physischen und logischen Netzwerk isoliert werden Instanzen des Microsoft Enterprise Cloud-Dienste, die vom lokalen Personal und innerhalb der geografischen Rahmen des bestimmten Ländern beschränkt.

Aktuelle nationale Wolken umfassen Folgendes:

- Microsoft Cloud for US Government
- Microsoft Cloud Deutschland
- Azure und Office 365, betrieben von 21Vianet in China

Jede Cloudumgebung national ist eindeutig und anderen als der globalen Microsoft-Umgebung. Es ist wichtig, dass einige der wichtigsten Unterschiede bei der Entwicklung von Anwendungen für national Cloud-Umgebungen. Registrierung von Anwendungen, dem Erwerb von Token und die Microsoft Graph-API aufrufen können beispielsweise anders lauten.

Dieser Artikel enthält Informationen zu den verschiedenen Microsoft Graph national Cloud-Bereitstellungen und die Funktionen, die innerhalb der einzelnen Entwicklern zur Verfügung stehen.

## <a name="app-registration-and-token-service-root-endpoints"></a>App-Registrierung und Token Stamm Dienstendpunkten

Vor dem Aufrufen der Microsoft Graph-APIs, sollten Sie zuerst registrieren Sie Ihre Anwendung und ein Token zu erwerben. Die folgende Tabelle enthält die Basis URLs für die Azure Active Directory (AD Azure) Endpunkte zum Registrieren der Anwendung und Token für die einzelnen nationalen Cloud zu erwerben.

| National cloud | Azure AD-Portal-Endpunkt| Dem Azure AD-Endpunkt|
|---------------------------|----------------|----------------|
|Azure AD für die US Regierung |https://portal.azure.us|`https://login.microsoftonline.us`|
|Azure AD Deutschland |https://portal.microsoftazure.de|`https://login.microsoftonline.de`|
|Azure AD China von 21vianet bedient |https://portal.azure.cn|`https://login.chinacloudapi.cn`|
|Azure AD (weltweiter Service)|https://portal.azure.com |`https://login.microsoftonline.com`|

Weitere Informationen zu Azure AD-Token und Microsoft Graph Zugriff finden Sie unter [Auth-Token abzurufen](./auth-overview.md). Azure AD-Authentifizierungsszenarien finden Sie unter [Grundlagen der Azure AD-Authentifizierung](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios).

> **Hinweis:** Die [Autorisierungs- und Tokenendpunkte von Azure AD, Version 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) sind nur für den globalen Dienst verfügbar. Sie werden noch nicht für die Verwendung mit nationalen Cloudbereitstellungen unterstützt.


## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Microsoft Graph und Diagramm Explorer Stamm Dienstendpunkten

In der folgenden Tabelle zeigt die Stamm-Endpunkte für Microsoft Graph und [Diagramm Explorer](https://developer.microsoft.com/graph/graph-explorer) für die einzelnen nationalen Cloud.

| Nationale Cloud | Microsoft Graph | Graph-Tester |
|---------------------------|----------------|----------------|
| Microsoft Graph für die US-Regierung | https://graph.microsoft.us | Nicht unterstützt. |
| Microsoft Graph Deutschland | https://graph.microsoft.de | Nicht unterstützt |
| Microsoft Graph China betrieben von 21Vianet | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Microsoft Graph weltweiter Service | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> **Vermerk**:Apps können nur über die nationalen Cloudendpunkte auf Organisationsdaten zugreifen. Dies bedeutet, dass apps nur Daten im Mandanten zugreifen können, die in der Cloud für bestimmte national registriert sind. Apps, die zugeordneten persönlicher Microsoft-Konten über einen Microsoft Graph Consumer-Daten zugreifen möchten, sollten den globalen Dienst verwenden `https://graph.microsoft.com`. Für eine Cloudbereitstellung national erworbene Zugriffstoken sind nicht mit den für die globalen Dienst oder eine beliebige andere national Cloud erworben austauschbar.

## <a name="supported-features"></a>Unterstützte Features

Die folgenden Features von Microsoft Graph stehen in der Regel auf der `/v1.0` Endpunkt über alle nationalen Cloud-Bereitstellungen, soweit nicht anders angegeben.

| Microsoft Graph-features | Microsoft Cloud for US Government | Microsoft Cloud China vom Dienst 21Vianet | Microsoft Cloud Deutschland |
|---------------------------|----------------|----------------|----------------|
| Benutzer | ✔ | ✔ | ✔ |
| Gruppen | ✔ | ✔ | ✔ |
| Excel | ✔| ✔* | ✔ |
| OneDrive | ✔ | ✔* | ✔ |
| Outlook Mail | ✔ | ✔ | ✔ |
| Outlook-Kalender | ✔ | ✔ | ✔ |
| Private Kontakte | ✔ | ✔ | ✔ |
| SharePoint| ✔ | ✔* | ✔ |
| Planner|✔ |✔ |✔ |
| Berichte  |➖| ✔ |➖|
| Delta-Abfrage | ➖ | ➖| ➖ |
| Webhooks  | ➖| ➖| ➖
|Verzeichnisschemaerweiterungen |➖|➖|➖|
| Offene Typerweiterungen|➖|➖|➖|
  
Die folgenden zusätzlichen Microsoft Graph-Funktionen stehen in der Vorschau (klicken Sie auf die `/beta` Endpunkt) über alle nationalen Cloud-Bereitstellungen, soweit nicht anders angegeben:

* Organisationskontakte
* Anwendungen
* Dienstprinzipale

(*) Eingeschränkte Unterstützung für diese API in dieser Cloud.

 > **Wichtig:** Bestimmte Dienste und Features, die in bestimmten Regionen des globalen Diensts sind möglicherweise nicht in allen nationalen Wolken verfügbar. Um herauszufinden, welche Dienste zur Verfügung stehen, finden Sie unter [Produkte nach Region zur Verfügung](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast).


Weitere Informationen zum National Wolken finden Sie in den folgenden Themen:
- [Microsoft National Wolken](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
- [Office 365 für US-Regierung](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
- [Office 365 handelt, das von 21Vianet](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
- [Office 365 Deutschland](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
- [Azure Behörden](https://azure.microsoft.com/global-infrastructure/government/)
- [Azure China 21Vianet](https://docs.microsoft.com/azure/china/)
- [Azure Deutschland](https://docs.microsoft.com/azure/germany/)
