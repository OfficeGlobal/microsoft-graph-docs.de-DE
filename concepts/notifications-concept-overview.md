---
title: 'Verwenden der Benachrichtigungs-API in Microsoft Graph zur Realisierung von auf den Benutzer ausgerichteten Benachrichtigungsfunktionen '
description: 'Benachrichtigungen stellen die wirksamste Möglichkeit dar, Benutzer wieder an sich zu binden. Sie können die Aufmerksamkeit Ihres Benutzers erregen und bringen ihn wieder zu Ihrer App zurück. In einer Welt der vielen Geräte können Ihre Benutzer von überall auf Ihre Apps und Dienste zugreifen, auf verschiedenen Plattformen und Geräten, auf denen Ihre Apps präsent sind. '
ms.openlocfilehash: 7ff36d7e0d406cb7918e2999812e3c756ae3b5bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092202"
---
# <a name="using-the-notifications-api-in-microsoft-graph-to-enable-human-centric-notification-experiences"></a>Verwenden der Benachrichtigungs-API in Microsoft Graph zur Realisierung von auf den Benutzer ausgerichteten Benachrichtigungsfunktionen 

Benachrichtigungen stellen die wirksamste Möglichkeit dar, Benutzer wieder an sich zu binden. Sie können die Aufmerksamkeit Ihres Benutzers erregen und bringen ihn wieder zu Ihrer App zurück. In einer Welt der vielen Geräte können Ihre Benutzer von überall auf Ihre Apps und Dienste zugreifen, auf verschiedenen Plattformen und Geräten, auf denen Ihre Apps präsent sind. 

Ihre Benachrichtigungsszenarien sollten "benutzerzentriert" ausgelegt sein, mit dem primären Ziel, den Benutzer zu benachrichtigen, gleich wo er oder sie sich aufhält. Die von den großen Plattformen angebotenen Benachrichtigungslösungen eignen sich toll für die Ansteuerung von Geräten. Microsoft Graph-Benachrichtigungen gehen darüber hinaus und erlauben es Ihnen, gezielt Benutzer anzusprechen. Microsoft Graph-Benachrichtigungen nehmen Ihnen den komplizierten Teil der Arbeit ab, einschließlich der Zuordnung von Benutzern und Endpunkten, der Synchronisierung des Benachrichtigungsstatus zwischen verschiedenen Endpunkten und mehr. 

## <a name="why-integrate-with-microsoft-graph-notifications"></a>Vorteile der Integration von Microsoft Graph-Benachrichtigungen
### <a name="deliver-notifications-to-a-user-across-different-endpoints"></a>Zustellen von Benachrichtigungen an einen Benutzer über verschiedene Endpunkte hinweg
Als Teil von Microsoft Graph ermöglicht Ihnen die Benachrichtigungs-API, ein Microsoft-Konto oder ein Geschäfts-, Schul- oder Unikonto (Azure AD) anzusteuern, um eine Benachrichtigung zuzustellen. Die Plattform verteilt diese Benachrichtigung an alle Endpunkte des Benutzers, einschließlich Windows UWP, Android und iOS. 

### <a name="manage-notifications-across-endpoints"></a>Übergreifendes Verwalten von Benachrichtigungen über Endpunkte hinweg
Mithilfe der Microsoft Graph-Benachrichtigungs-API können Sie den Status einer Benachrichtigung aktualisieren und diesen Status übergreifend auf allen Endpunkten synchronisieren. Wenn ein Benutzer aufgrund einer Benachrichtigung auf einem Gerät aktiv wird, können Sie den Status dieser Benachrichtigung aktualisieren (etwa indem sie sie als gelesen oder geschlossen markieren), und diese Statusaktualisierung wird an alle anderen Endpunkte verteilt. Die Microsoft Graph-Benachrichtigungs-API verfolgt den Status der Benachrichtigungen Ihres Benutzers zentral nach, wodurch Sie auf einfache Weise sicherstellen können, dass Ihre Benachrichtigungen einmal verarbeitet und dann überall geschlossen werden.

### <a name="retrieve-notification-history"></a>Abrufen des Benachrichtigungsverlaufs
Sie können die Benachrichtigungs-API verwenden, um den Benachrichtigungsverlauf basierend auf einer von Ihnen festgelegten Ablaufzeit (bis zu 30 Tage) abzurufen. Benachrichtigungen, die als gelesen oder geschlossen gekennzeichnet wurden, können trotzdem aus dem Verlauf abgerufen werden, was eine In-App-Ansicht des Benachrichtigungsverlaufs und weitere Szenarien ermöglicht. 

## <a name="integrating-with-the-notifications-api-in-microsoft-graph"></a>Integration mit der Benachrichtigungs-API in Microsoft Graph

Sie können Microsoft Graph-Benachrichtigungen in einigen einfachen Schritten in Ihre Apps integrieren – führen Sie ein Onboarding Ihrer App mithilfe von Windows Dev Center durch, verwenden Sie die Methode [Benachrichtigung erstellen](/graph/api/projectrome-notification-post?view=graph-rest-beta) zum Veröffentlichen von Benachrichtigungen, und nutzen Sie das Project Rome-SDK, um Benachrichtigungen auf Ihren App-Clients zu empfangen und zu verwalten.  

Weitere Informationen zum Veröffentlichen von Benutzerbenachrichtigungen mithilfe von Microsoft Graph finden Sie in der [Benachrichtigungs-API-Referenz](/graph/api/resources/notifications-api-overview?view=graph-rest-beta).
 
Weitere Informationen zum Empfang und der Verwaltung von Benachrichtigungen durch Integration des Project Rome-SDKs finden Sie in der [Dokumentation zum Project Rome-SDK](https://docs.microsoft.com/de-DE/windows/project-rome/). 

## <a name="see-also"></a>Siehe auch

- [Geräteübergreifende Oberflächen in Microsoft Graph](cross-device-concept-overview.md)
- [Project Rome Dev Center](https://aka.ms/projectrome)
