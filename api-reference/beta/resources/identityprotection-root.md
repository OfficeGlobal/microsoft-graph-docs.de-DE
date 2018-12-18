---
title: Verwenden Sie den Azure AD-Schutz API (Preview)
description: Microsoft Graph können Sie Abfragen die IdentityRiskEvent Ressource für jede Art von Risikoereignis von Azure AD-Schutz erkannt. Diese Ereignisse sind für Kunden mit Azure AD Premium P2 verfügbar. Eine Teilmenge von Ereignissen ist für Kunden mit Azure AD Premium P1 verfügbar.
author: cloudhandler
ms.openlocfilehash: 8afee9685d22dfaeea43a01f70a8b2834c8d4ff9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310374"
---
# <a name="use-the-azure-ad-identity-protection-api-preview"></a>Verwenden Sie den Azure AD-Schutz API (Preview)

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Microsoft Graph können Sie Abfragen die [IdentityRiskEvent](identityriskevent.md) Ressource für jede Art von Risikoereignis von [Azure AD-Schutz](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)erkannt. Diese Ereignisse sind für Kunden mit Azure AD Premium P2 verfügbar. Eine Teilmenge von Ereignissen ist für Kunden mit Azure AD Premium P1 verfügbar.

* [Anmeldungen von anonymen IP-Adressen](anonymousipriskevent.md)
* [Anmeldungen von Geräten Malware infiziert](malwareriskevent.md)
* [unmöglich Reisen zu untypischen Speicherorte](impossibletravelriskevent.md)
* [Benutzer mit verlorene Anmeldeinformationen](leakedcredentialsriskevent.md)
* [Anmeldungen von verdächtigen IP-Adressen](suspiciousipriskevent.md)
* [Anmeldungen von unbekannten Standorten](unfamiliarlocationriskevent.md)

Verwenden Sie die folgenden Vorgänge, um diese Ereignisse und die zugehörigen Informationen abzurufen:

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| IdentityRiskEvent-Auflistung abrufen. |
|[Abrufen von identityRiskEvent](../api/identityriskevent-get.md) |[identityRiskEvent](identityriskevent.md)| Rufen Sie IdentityRiskEvent-Objekt. |
|[Liste anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| AnonymousIpRiskEvent-Auflistung abrufen. |
|[Abrufen von anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) |[anonymousIpRiskEvent](anonymousipriskevent.md)| Rufen Sie AnonymousIpRiskEvent-Objekt. |
|[Liste impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| ImpossibleTravelRiskEvent-Auflistung abrufen. |
|[Abrufen von impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) |[impossibleTravelRiskEvent](impossibletravelriskevent.md)| Rufen Sie ImpossibleTravelRiskEvent-Objekt. |
|[Liste leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| LeakedCredentialsRiskEvent-Auflistung abrufen. |
|[Abrufen von leakedCredentialsRiskEvent](../api/leakedcredentialsriskevent-get.md) |[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md)| Rufen Sie LeakedCredentialsRiskEvent-Objekt. |
|[Liste malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| MalwareRiskEvent-Auflistung abrufen. |
|[Abrufen von malwareRiskEvent](../api/malwareriskevent-get.md) |[malwareRiskEvent](malwareriskevent.md)| Rufen Sie MalwareRiskEvent-Objekt. |
|[Liste suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| SuspiciousIpRiskEvent-Auflistung abrufen. |
|[Abrufen von suspiciousIpRiskEvent](../api/suspiciousipriskevent-get.md) |[suspiciousIpRiskEvent](suspiciousipriskevent.md)| Rufen Sie SuspiciousIpRiskEvent-Objekt. |
|[Liste unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| UnfamiliarLocationRiskEvent-Auflistung abrufen. |
|[Abrufen von unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) |[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md)| Rufen Sie UnfamiliarLocationRiskEvent-Objekt. |

# <a name="see-also"></a>Siehe auch

* [Informationen zum Schutz von Azure Active Directory-Identität](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection)
* [Erste Schritte mit Azure Active Directory-Schutz und Microsoft Graph](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started)
