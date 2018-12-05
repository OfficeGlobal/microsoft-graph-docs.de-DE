---
title: Skype for Business-Peer-zu-Peer-Aktivitätsberichte
description: Sie können Details für Peer-zu-Peer-Aktivität innerhalb Ihrer Organisation abrufen. Diese Details sind sehr hilfreich, wenn Sie andere Geschäftsentscheidungen für Ihre Organisation in Erwägung ziehen, planen und durchführen.
ms.openlocfilehash: c4f5397c31020d0fecd6e7cb68a3e39098349bb3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059716"
---
# <a name="skype-for-business-peer-to-peer-activity-reports"></a>Skype for Business-Peer-zu-Peer-Aktivitätsberichte

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Sie können Details für Peer-zu-Peer-Aktivität innerhalb Ihrer Organisation abrufen. Diese Details sind sehr hilfreich, wenn Sie andere Geschäftsentscheidungen für Ihre Organisation in Erwägung ziehen, planen und durchführen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Skype for Business-Peer-to-Peer-Aktivität](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Aktivitätsanzahl abrufen](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md) | Stream          | [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md) | Erhalten Sie Informationen über die Anzahl und Art der in Ihrem Unternehmen gehaltenen Sitzungen. Zu den Sitzungsarten gehören Chat, Audio, Video, Anwendungsfreigabe und Dateiübertragung. |
| [Benutzeranzahl abrufen](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md) | Stream          | [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md) | Erhalten Sie Informationen über die Anzahl der eindeutigen Benutzer und die Art der in Ihrem Unternehmen gehaltenen Peer-to-Peer-Sitzungen. Zu den Sitzungsarten gehören Chat, Audio, Video, Anwendungsfreigabe und Dateiübertragung in Peer-to-Peer-Sitzungen. |
| [Minutenanzahl abrufen](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md) | Stream          | [skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) | Erhalten Sie Informationen über die Dauer (in Minuten) und die Art der in Ihrem Unternehmen gehaltenen Peer-to-Peer-Sitzungen. Zu den Sitzungsarten gehören Audio und Video. |