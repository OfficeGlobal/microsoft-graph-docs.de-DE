---
title: Erste Schritte mit Microsoft Graph Data Connect (Vorschau)
description: 'Bevor Sie Microsoft Graph Data Connect verwenden können, muss ein Office 365-Administrator zwei Aktionen ausgeführt haben, die beide die Steuerung von Datenbewegungen durch den Administrator mithilfe von PAM (Privileged Access Management) aktivieren. '
ms.openlocfilehash: eb21f0d850f64694514c0ecd82f03de687606a56
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092177"
---
# <a name="get-started-with-microsoft-graph-data-connect-preview"></a>Erste Schritte mit Microsoft Graph Data Connect (Vorschau)

Bevor Sie Microsoft Graph Data Connect verwenden können, muss ein Office 365-Administrator zwei Aktionen ausgeführt haben, die beide die Steuerung von Datenbewegungen durch den Administrator mithilfe von PAM (Privileged Access Management) aktivieren. 

1. Zustimmung zu der Entscheidung für Microsoft Graph Data Connect über das Microsoft 365 Admin Portal auf der Seite **Dienste und Add-Ins**. Dadurch werden Anforderungen für Datenbewegungen an Microsoft Azure zugelassen (d. h., die vollständige Kontrolle über die Daten bleibt erhalten, Azure-Ressourcen wird jedoch Zugriffsberechtigung erteilt). Es werden keine Daten übertragen, sofern nicht später die Genehmigung für eine bestimmte Pipeline erteilt wird.
2. Festlegen einer Gruppe von genehmigenden Personen innerhalb des Office 365-Abonnements. Achten Sie darauf, dass die Gruppe der genehmigenden Personen nicht leer ist. Nur die Benutzer in der Gruppe können Anforderungen zu Datenbewegungen genehmigen.

Ausführliche Schritt-für-Schritt-Anweisungen finden Sie im [Microsoft Graph Data Connect-Schulungsmodul](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md).

## <a name="next-steps"></a>Nächste Schritte

Herzlichen Glückwunsch! Jetzt sind sie bereit, mit dem Erstellen intelligenter Anwendungen mit Azure-Tools zu beginnen. Eine Beispielanwendung und weiterführende Dokumentation finden Sie im [Microsoft Graph Data Connect-GitHub-Repository](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki). 
