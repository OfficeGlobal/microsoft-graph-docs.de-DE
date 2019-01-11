---
title: Verwenden der Graph-API für Intune
description: " Hybridbereitstellungen Intune werden nicht unterstützt. "
author: tfitzmac
localization_priority: Priority
ms.openlocfilehash: 606c2324476492f8dc9271646d0109bb3d57de99
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869713"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Arbeiten mit Intune in Microsoft Graph  

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Die Microsoft Graph-API für Intune ermöglicht Ihrem Mandanten den programmgesteuerten Zugriff auf Intune-Informationen; die API kann die gleichen Intune-Operationen ausführen, die auch im **Azure-Portal** verfügbar sind.  

Für mobiles Gerät Verwaltungsszenarien (MDM) unterstützt der Microsoft Graph-API für Intune Standalone-Bereitstellungen. Intune [hybridbereitstellungen](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) werden nicht unterstützt. 

## <a name="using-the-microsoft-graph-api-for-intune"></a>Verwenden das Microsoft Graph-API für Intune

Intune stellt Daten in Microsoft Graph die gleiche Weise wie andere Cloud-Dienste, mit umfassenden Entität Informationen und Beziehung Navigation.Verwenden Sie Microsoft Graph zum Kombinieren von Informationen aus anderen Dienste und Intune für IT-Experten oder Endbenutzer rich Cross-dienstanwendungen erstellen.     

Das folgende Beispiel zeigt, wie Sie ermitteln können, ob eine Anwendung auf das Gerät des Benutzers installiert ist: 

1. Rufen Sie aus Azure Active Directory eine Liste der Geräte ab, die auf den Benutzer registriert sind: 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. Rufen Sie dann die Liste der Anwendungen Ihres Mandanten ab: 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. Fügen Sie die ID der betreffenden Anwendung unten ein, um den Installationsstatus der Anwendung (und gleichzeitig den des Benutzers) zu ermitteln:

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a>Verwenden von Microsoft Graph-Berechtigungen

Microsoft Graph steuert den Zugriff auf Ressourcen über Berechtigungen. Als Entwickler müssen Sie die Berechtigungen angeben, die Sie Intune-Ressourcen zugreifen müssen. Geben Sie in der Regel die Berechtigungen im Azure Active Directory-Portal. Weitere Informationen finden Sie unter [Microsoft Graph Berechtigungen Verweis](https://docs.microsoft.com/en-us/graph/permissions-reference).

## <a name="next-steps"></a>Nächste Schritte

- Erfahren Sie, [wie Sie mit Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) , um die Microsoft Graph-API für Intune zugreifen.  
- Machen Sie sich die [PowerShell Intune Beispiele](https://github.com/microsoftgraph/powershell-intune-samples), die zeigen, wie die Microsoft Graph-API für Intune im Kontext des Beispiele verwenden.

