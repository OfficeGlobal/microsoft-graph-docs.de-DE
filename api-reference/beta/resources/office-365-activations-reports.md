---
title: Office 365-Aktivierungsberichte
description: Der Office 365 Activation Bericht bietet eine Ansicht, von der Benutzer ihre Office 365-Abonnements auf mindestens ein Gerät aktiviert haben. Es bietet eine Aufschlüsselung der Office 365 ProPlus, Project und Visio Pro für Office 365-Abonnement Aktivierungen als auch die Aufgliederung der Aktivierungen über Desktop und Geräte. In diesem Bericht konnte können Sie die Benutzer zu identifizieren, die möglicherweise zusätzliche Unterstützung für ihre Office-Abonnement zu aktivieren.
localization_priority: Normal
ms.openlocfilehash: 2576579879e60573a9ed70f805fe07532bab8ad8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822218"
---
# <a name="office-365-activations-reports"></a>Office 365-Aktivierungsberichte

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Der Office 365 Activation Bericht bietet eine Ansicht, von der Benutzer ihre Office 365-Abonnements auf mindestens ein Gerät aktiviert haben. Es bietet eine Aufschlüsselung der Office 365 ProPlus, Project und Visio Pro für Office 365-Abonnement Aktivierungen als auch die Aufgliederung der Aktivierungen über Desktop und Geräte. In diesem Bericht konnte können Sie die Benutzer zu identifizieren, die möglicherweise zusätzliche Unterstützung für ihre Office-Abonnement zu aktivieren.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Berichte
| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getoffice365activationsuserdetail.md) | Stream          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Erhalten Sie detaillierte Informationen über Benutzer, die Office 365 aktiviert haben. |
| [Aktivierungsanzahl abrufen](../api/reportroot-getoffice365activationcounts.md) | Stream          | [office365ActivationCounts](../resources/office365activationcounts.md) | Erfahren Sie, wie viele Office 365-Aktivierungen auf Desktops und Geräten durchgeführt wurden. |
| [Benutzeranzahl abrufen](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | Rufen Sie die Anzahl der aktivierten Benutzer ab und erfahren Sie, wie viele Benutzer das Office-Abonnement auf dem Desktop oder einem Gerät aktiviert haben. |
