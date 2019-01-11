---
title: Yammer-Aktivitätsberichte
description: Wie viel Aktivität, über die Organisation und die Anzahl der eindeutigen Benutzer, die buchen generiert wird, like und Lesen von Nachrichten auf Yammer, können Sie die Ebene des Engagements mit Yammer Ihrer Organisation vertraut sein.
localization_priority: Normal
ms.openlocfilehash: 9895e37812b037b33f13682c3c56dacba5928d5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27823709"
---
# <a name="yammer-activity-reports"></a>Yammer-Aktivitätsberichte

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt. Diese APIs werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt.

Wie viel Aktivität, über die Organisation und die Anzahl der eindeutigen Benutzer, die buchen generiert wird, like und Lesen von Nachrichten auf Yammer, können Sie die Ebene des Engagements mit Yammer Ihrer Organisation vertraut sein.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Aktivität](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getyammeractivityuserdetail.md) | Stream          | [yammerActivityUserDetail](../resources/yammeractivityuserdetail.md) | Rufen Sie Details zu Yammer-Aktivitäten nach Benutzer ab. |
| [Aktivitätsanzahl abrufen](../api/reportroot-getyammeractivitycounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Gewinnen Sie einen Eindruck der Yammer-Aktivitäten in Ihrer Organisation, indem Sie erfahren, wie viele Nachrichten gepostet, gelesen und gelikt wurden. |
| [Benutzeranzahl abrufen](../api/reportroot-getyammeractivityusercounts.md) | Stream          | [yammerActivitySummary](../resources/yammeractivitysummary.md) | Erfahren Sie, wie viele eindeutige Benutzer Yammer-Nachrichten veröffentlicht, gelesen und gelikt haben. |
