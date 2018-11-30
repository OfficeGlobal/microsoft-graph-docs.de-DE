---
title: Verwenden Sie den Azure AD-Schutz API (Preview)
description: Microsoft Graph können Sie Abfragen die IdentityRiskEvent Ressource für jede Art von Risikoereignis von Azure AD-Schutz erkannt. Diese Ereignisse sind für Kunden mit Azure AD Premium P2 verfügbar. Eine Teilmenge von Ereignissen ist für Kunden mit Azure AD Premium P1 verfügbar.
ms.openlocfilehash: 10b2e7dc59c8a9aeef25aa4ed5e27667b12a8eee
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063122"
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
