---
title: Berichte über aktive Office 365-Benutzer
description: Sie können den Office 365 aktive Benutzer Bericht verwenden, um zu ermitteln, wie viele Lizenzen von Personen in Ihrer Organisation verwendet werden und Ausführen eines Drilldowns Informationen darüber, welche Benutzer welche Produkte verwenden. In diesem Bericht hilft Administratoren nicht ausgelastete Produkte oder Benutzer, die möglicherweise zusätzliche Schulungen oder Informationen zu identifizieren.
localization_priority: Normal
ms.openlocfilehash: d52588630dcb18a146f34ad66c154e3a64752266
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837156"
---
# <a name="office-365-active-users-reports"></a>Berichte über aktive Office 365-Benutzer

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Sie können den Office 365 aktive Benutzer Bericht verwenden, um zu ermitteln, wie viele Lizenzen von Personen in Ihrer Organisation verwendet werden und Ausführen eines Drilldowns Informationen darüber, welche Benutzer welche Produkte verwenden. In diesem Bericht hilft Administratoren nicht ausgelastete Produkte oder Benutzer, die möglicherweise zusätzliche Schulungen oder Informationen zu identifizieren.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Aktive Benutzer](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).

## <a name="reports"></a>Berichte
| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getoffice365activeuserdetail.md) | Stream          | [office365ActiveUserDetail](../resources/office365activeuserdetail.md) | Rufen Sie Details zu aktiven Office 365-Benutzern ab. |
| [Benutzeranzahl abrufen](../api/reportroot-getoffice365activeusercounts.md) | Stream          | [office365ActiveUserCounts](../resources/office365activeusercounts.md) | Rufen Sie die Anzahl der im Berichtszeitraum täglich aktiven Benutzer nach Produkt ab. |
| [Benutzeranzahl für Dienste abrufen](../api/reportroot-getoffice365servicesusercounts.md) | Stream          | [office365ServicesUserCounts](../resources/office365servicesusercounts.md) | Rufen Sie die Anzahl der Benutzer nach Aktivitätstyp und Dienst ab. |
