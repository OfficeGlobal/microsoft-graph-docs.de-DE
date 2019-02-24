---
title: Verwenden der Intune Graph API – Microsoft Graph-API
description: Listet die Endpunkte der Microsoft Graph-API für Intune (REST) auf, mit denen Sie Ihre Mandantenorganisation, deren Geräte, Apps, Zugriff und Ressourcen verwalten können.
author: tfitzmac
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: fc254772a5b4db131a5cda45fc83b336bf12f993
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167445"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Arbeiten mit Intune in Microsoft Graph  

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/de-DE/cloud-platform/microsoft-intune-pricing) ist.

Die Microsoft Graph-API für Intune ermöglicht Ihrem Mandanten den programmgesteuerten Zugriff auf Intune-Informationen; die API kann die gleichen Intune-Operationen ausführen, die auch im **Azure-Portal** verfügbar sind.  

In Szenarien für die Verwaltung mobiler Geräte (MDM, Mobile Device Management) unterstützt die Microsoft Graph-API für Intune eigenständige Bereitstellungen. [Hybride Intune-Bereitstellungen](https://docs.microsoft.com/de-DE/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) werden nicht unterstützt. 

## <a name="using-the-microsoft-graph-api-for-intune"></a>Verwenden der Microsoft Graph-API für Intune

Intune stellt Daten auf die gleiche Weise für Microsoft Graph bereit, wie es auch andere Clouddienste tun, mit detaillierten Informationen zu Entitäten und Möglichkeiten zur Beziehungsnavigation.Mithilfe von Microsoft Graph können Sie Informationen aus anderen Diensten und aus Intune miteinander kombinieren und so funktionsreiche, dienstübergreifende Anwendungen für IT-Experten oder Endbenutzer erstellen.     

Das folgende Beispiel demonstriert, wie Sie herausfinden können, ob auf dem Gerät eines Benutzers eine bestimmte Anwendung installiert ist: 

1. Rufen Sie aus Azure Active Directory eine Liste der Geräte ab, die auf den Benutzer registriert sind: 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. Rufen Sie dann die Liste der Anwendungen Ihres Mandanten ab: 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. Fügen Sie die ID der betreffenden Anwendung unten ein, um den Installationsstatus der Anwendung (und gleichzeitig den des Benutzers) zu ermitteln:

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a>Verwenden von Microsoft Graph-Berechtigungen

Microsoft Graph steuert den Zugriff auf Ressourcen über Berechtigungen. Als Entwickler müssen Sie die Berechtigungen angeben, die Sie für den Zugriff auf Intune-Ressourcen benötigen. In der Regel geben Sie die Berechtigungen im Azure Active Directory-Portal an. Weitere Informationen finden Sie in der [Referenz zu den Microsoft Graph-Berechtigungen](https://docs.microsoft.com/de-DE/graph/permissions-reference).

## <a name="next-steps"></a>Nächste Schritte

- Erfahren Sie [wie Sie Azure AD verwenden](https://docs.microsoft.com/de-DE/intune/intune-graph-apis), um auf die Microsoft Graph-API für Intune zuzugreifen.  
- Erkunden Sie die [PowerShell Intune-Beispiele](https://github.com/microsoftgraph/powershell-intune-samples), die zeigen, wie Sie die Microsoft Graph-API für Intune im Kontext von Arbeitsbeispielen verwenden können.

