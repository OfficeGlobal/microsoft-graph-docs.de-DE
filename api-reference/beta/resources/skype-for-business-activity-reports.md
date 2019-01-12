---
title: Skype for Business-Aktivitätsberichte
description: Sie können ausführliche Informationen zum Aktivität innerhalb Ihrer Organisation erhalten. Diese Details können Ihnen bei der Suche, Planung und Durchführung anderer Geschäftsentscheidungen innerhalb Ihrer Organisation helfen.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: fcc40f0cba1e8a5f2304554088562af15c592964
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941674"
---
# <a name="skype-for-business-activity-reports"></a>Skype for Business-Aktivitätsberichte

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Sie können ausführliche Informationen zum Aktivität innerhalb Ihrer Organisation erhalten. Diese Details können Ihnen bei der Suche, Planung und Durchführung anderer Geschäftsentscheidungen innerhalb Ihrer Organisation helfen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Aktivität](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getskypeforbusinessactivityuserdetail.md) | Stream          | [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) | Rufen Sie Details der Skype for Business-Aktivität nach Benutzer ab. |
| [Aktivitätsanzahl abrufen](../api/reportroot-getskypeforbusinessactivitycounts.md) | Stream          | [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) | Rufen Sie die Trends dazu ab, wie viele Benutzer Konferenzsitzungen, die in Ihrem Unternehmen mit Skype for Business abgehalten wurden, organisiert und daran teilgenommen haben. Der Bericht enthält auch die Anzahl von Peer-to-Peer-Sitzungen. |
| [Benutzeranzahl abrufen](../api/reportroot-getskypeforbusinessactivityusercounts.md) | Stream          | [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) | Rufen Sie die Trends dazu ab, wie viele eindeutige Benutzer Konferenzsitzungen, die in Ihrem Unternehmen mit Skype for Business abgehalten wurden, organisiert und daran teilgenommen haben. Der Bericht enthält auch die Anzahl von Peer-to-Peer-Sitzungen. |
