---
title: E-Mail-Aktivitätsberichte
description: Sie können eine Ansicht der e-Mail-Verkehr auf oberster Ebene innerhalb Ihrer Organisation über die Seite Berichte abrufen. Sie können auch in der e-Mail-Aktivität-Widget zu verstehen, die Trends und Details pro Benutzer, der die e-Mail-Aktivität in Ihrer Organisation anzeigen.
ms.openlocfilehash: 47ff9017216fa3fd333b383f7a603354775d1023
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066058"
---
# <a name="email-activity-reports"></a>E-Mail-Aktivitätsberichte

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Sie können eine Ansicht der e-Mail-Verkehr auf oberster Ebene innerhalb Ihrer Organisation über die Seite Berichte abrufen. Sie können auch in der e-Mail-Aktivität-Widget zu verstehen, die Trends und Details pro Benutzer, der die e-Mail-Aktivität in Ihrer Organisation anzeigen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – E-Mail-Aktivität](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getemailactivityuserdetail.md) | Stream          | [emailActivityUserDetail](../resources/emailactivityuserdetail.md) | Erhalten Sie detaillierte Informationen über die von Benutzern ausgeführten E-Mail-Aktivitäten. |
| [Aktivitätsanzahl abrufen](../api/reportroot-getemailactivitycounts.md) | Stream          | [emailActivitySummary](../resources/emailactivitysummary.md) | Ermöglicht es Ihnen, einen Überblick über die E-Mail-Aktivitäten (z. B. wie viele E-Mails versendet, gelesen und empfangen wurden) in Ihrer Organisation zu gewinnen. |
| [Benutzeranzahl abrufen](../api/reportroot-getemailactivityusercounts.md) | Stream          | [emailActivitySummary](../resources/emailactivitysummary.md) | Ermöglicht es Ihnen, sich anhand der Anzahl eindeutiger Benutzer, die E-Mail-Aktivitäten wie Senden, Lesen und Empfangen ausführen, über Trends zu informieren. |