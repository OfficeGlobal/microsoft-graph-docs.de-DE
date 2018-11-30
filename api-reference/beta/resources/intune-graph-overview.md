---
title: Verwenden der Graph-API für Intune
description: " Hybridbereitstellungen Intune werden nicht unterstützt. "
ms.openlocfilehash: 2502b5209e9935fc923570947c38c0467534f4ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062985"
---
# <a name="working-with-intune-in-microsoft-graph"></a>Arbeiten mit Intune in Microsoft Graph  

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Die Microsoft Graph-API für Intune ermöglicht Ihrem Mandanten den programmgesteuerten Zugriff auf Intune-Informationen; die API kann die gleichen Intune-Operationen ausführen, die auch im **Azure-Portal** verfügbar sind.  

In Szenarien für die Verwaltung mobiler Geräte (MDM, Mobile Device Management) unterstützt die Graph-API für Intune eigenständige Bereitstellungen. [Hybride Intune-Bereitstellungen](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) werden nicht unterstützt. 

## <a name="using-the-intune-graph-api"></a>Verwenden der Graph-API für Intune

Intune stellt Daten in der Microsoft Graph die gleiche Weise wie andere Cloud-Dienste, mit umfassenden Entität Informationen und Beziehung Navigation.Verwenden Sie Microsoft Graph zum Kombinieren von Informationen aus anderen Dienste und Intune für IT-Experten oder Endbenutzer rich Cross-dienstanwendungen erstellen.     

Das Beispiel unten demonstriert, wie Sie herausfinden können, ob auf dem Gerät eines Benutzers eine bestimmte Anwendung installiert ist: 

1. Rufen Sie aus Azure Active Directory eine Liste der Geräte ab, die auf den Benutzer registriert sind: 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. Rufen Sie dann die Liste der Anwendungen Ihres Mandanten ab: 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. Fügen Sie die ID der betreffenden Anwendung unten ein, um den Installationsstatus der Anwendung (und gleichzeitig den des Benutzers) zu ermitteln:

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-graph-permission-scopes"></a>Verwenden von berechtigungsbereiche Diagramm

Microsoft Graph steuert den Zugriff auf Ressourcen unter Verwendung von berechtigungsbereiche. Als Entwickler müssen Sie die Berechtigungsbereiche angeben, die Sie für den Zugriff auf Intune-Ressourcen benötigen. In der Regel geben Sie die benötigten Berechtigungsbereiche im Azure Active Directory-Portal an. Weitere Informationen finden Sie im Artikel zu den Themen [Microsoft Graph-Berechtigungsbereiche](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) und [Intune-Berechtigungsbereiche](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).

## <a name="to-use-the-table-of-contents-on-the-microsoft-graph-site"></a>Mithilfe des Inhaltsverzeichnisses auf der Website Microsoft Graph
  
Sie können das Inhaltsverzeichnis (im linken Bereich der Website) durchsuchen, um die Teile der Dokumentation Intune Diagramm-API und Ressource zu suchen, die Sie anzeigen möchten.

1. Klicken Sie auf **/Beta Verweis** um Beta-Dokumente zu öffnen.
2. Führen Sie einen Bildlauf nach unten, und klicken Sie auf **Intune**.
3. Unterabschnitten unter **Intune** für die Teile der API klicken Sie weiterhin auf Sie 
