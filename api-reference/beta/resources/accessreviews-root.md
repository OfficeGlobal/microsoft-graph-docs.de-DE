---
title: Prüft Azure AD-Zugriff
description: Sie können die Azure AD Bewertungen zum Konfigurieren der einmaligen oder wiederkehrenden Access Bewertungen für Konformitätsbescheinigungssysteme Zugriffsrechte des Benutzers zuzugreifen.
ms.openlocfilehash: 33722c68429729e3996ad289d07146c95ee219ca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062663"
---
# <a name="azure-ad-access-reviews"></a>Prüft Azure AD-Zugriff

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Sie können [Azure AD Access überprüft](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) einmalige konfigurieren oder wiederkehrenden Zugriff für Konformitätsbescheinigungssysteme Zugriffsrechte des Benutzers überprüft.

Typische Kundenszenarien für den Zugriff von Gruppenmitgliedschaften überprüft und Anwendungszugriff sind:
   
- Kunden können prüfen und bestätigen Gast Benutzerzugriff mithilfe von Access Überprüfung des Zugriffs für Clientanwendungen und Mitgliedschaften von Gruppen. Bearbeiter können die Insights, die effizient entscheiden, ob es sich bei Gäste sollte Access weiterhin bereitgestellt werden.
      
- Kunden können prüfen und bestätigen Mitarbeiterzugriff auf Anwendungen und Gruppenmitgliedschaften mit Access Reviews (engl.).
   
- Kunden können zugreifen auf Steuerelemente von Überprüfung in Programme sammeln, die für Ihre Organisation zum Nachverfolgen von Bewertungen für Compliance oder Risiko vertrauliche Applications relevant sind.

Es gibt auch eine verwandte Funktion für Kunden um zu prüfen und bestätigen die rollenzuweisungen der Admin-Benutzer, die Azure AD-Rollen wie globaler Administrator oder Azure-Abonnement Rollen zugewiesen sind.  Diese Funktion ist in [Azure AD privilegierten Identitätsmanagement](privilegedidentitymanagement-root.md)enthalten.

Beachten Sie, dass das Feature Access Reviews (engl.), einschließlich der API in Azure AD Premium P2 enthalten ist. 

## <a name="methods"></a>Methoden

Hier wird die Liste der Methoden, die von Azure Active Directory bereitgestellt werden Bewertungen zugreifen.  

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Rufen Sie eine Access-Überprüfung mit einer bestimmten Id ab. |
|[Erstellen von accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Erstellen Sie eine neue AccessReview. |
|[AccessReview löschen](../api/accessreview-delete.md) | Keine.   | Löschen einer AccessReview. |
|[AccessReview aktualisieren](../api/accessreview-update.md) | [accessReview](accessreview.md) | Aktualisieren einer AccessReview. |
|[Liste AccessReview Bearbeiter](../api/accessreview-listreviewers.md) |      [Benutzeridentität](useridentity.md) -Auflistung| Rufen Sie die Bearbeiter ein AccessReview. |
|[AccessReview Bearbeiter hinzufügen](../api/accessreview-addreviewer.md) |      Keine.   |   Fügen Sie einem Bearbeiter ein AccessReview hinzu. |
|[AccessReview Reviewer entfernen](../api/accessreview-removereviewer.md) | Keine.  |   Entfernen Sie einen Prüfer aus einer AccessReview. |
|[Liste AccessReview Entscheidungen](../api/accessreview-listdecisions.md) |      [AccessReviewDecision](accessreviewdecision.md) -Auflistung| Rufen Sie die Entscheidungen des ein AccessReview.|
|[Meine AccessReview Entscheidungen auflisten](../api/accessreview-listmydecisions.md) |     [AccessReviewDecision](accessreviewdecision.md) -Auflistung| Rufen Sie als "Leser" Mein Entscheidungen von einer AccessReview.|
|[AccessReview Erinnerung senden](../api/accessreview-sendreminder.md) |        Keine.   |   Senden Sie eine Erinnerung an die Bearbeiter ein AccessReview. |
|[AccessReview beenden](../api/accessreview-stop.md) |     Keine.   |   Beenden einer AccessReview. |
|[AccessReview Entscheidungen zurücksetzen](../api/accessreview-reset.md) |     Keine.   |   Setzen Sie die Entscheidungen in einer laufenden AccessReview zurück.|
|[Anwenden von AccessReview Entscheidungen](../api/accessreview-apply.md) |     Keine.   |   Gelten Sie die Entscheidungen aus einer abgeschlossenen AccessReview.|
|[Liste businessFlowTemplates](../api/businessflowtemplate-list.md) | [BusinessFlowTemplate](businessflowtemplate.md) -Auflistung| Rufen Sie die Vorlagen für Unternehmen Fluss Bewertungen Zugriff auf entsprechende.|
|[Erstellen der Anwendung](../api/program-create.md) |   [Programm](program.md)   |   Erstellen Sie ein neues Programm.|
|[Programm löschen](../api/program-delete.md) |   Keine.   |   Löschen eines Programms.|
|[Programme auflisten](../api/program-list.md) |  [Programm](program.md) -Auflistung|   Rufen Sie eine Auflistung aller Programme.|
|[Liste ProgramControls eines Programms](../api/program-listcontrols.md) |      [ProgramControl](programcontrol.md) -Auflistung| Rufen Sie eine Auflistung der Steuerelemente eines Programms.|
|[Update-Programm](../api/program-update.md) |   [Programm](program.md)|  Aktualisieren eines Programms.|
|[Erstellen von programControl](../api/programcontrol-create.md) |     [programControl](programcontrol.md) |   Fügen Sie ein Programm ein ProgramControl hinzu.|
|[ProgramControl löschen](../api/programcontrol-delete.md) |     Keine.   |   Entfernen einer ProgramControl aus einem Programm.|
|[Liste programControls](../api/programcontrol-list.md) | [ProgramControl](programcontrol.md) -Auflistung| Von Listensteuerelementen in allen Programmen im Mandanten.|
|[Liste programControlTypes](../api/programcontroltype-list.md) | [ProgramControlType](programcontroltype.md) -Auflistung| Programm Steuerelement Listentypen. |


## <a name="see-also"></a>Siehe auch

- [Prüft wie ein Administrator des Benutzerzugriffs mit Azure AD-Zugriff verwalten kann](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Prüft wie ein Administrator Gastzugriff mit Azure AD-Zugriff verwalten kann](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
- [Wie kann ein Administrator Programme verwalten und Steuerelemente für Azure Active Directory zugreifen Reviews (engl.)](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-manage-programs-controls)


<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
