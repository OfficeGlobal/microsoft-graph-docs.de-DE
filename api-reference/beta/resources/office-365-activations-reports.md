---
title: Office 365-Aktivierungsberichte
description: Der Office 365 Activation Bericht bietet eine Ansicht, von der Benutzer ihre Office 365-Abonnements auf mindestens ein Gerät aktiviert haben. Es bietet eine Aufschlüsselung der Office 365 ProPlus, Project und Visio Pro für Office 365-Abonnement Aktivierungen als auch die Aufgliederung der Aktivierungen über Desktop und Geräte. In diesem Bericht konnte können Sie die Benutzer zu identifizieren, die möglicherweise zusätzliche Unterstützung für ihre Office-Abonnement zu aktivieren.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 345ab500ef5986471bb801a88ee5886473a3dd60
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/26/2019
ms.locfileid: "29573678"
---
# <a name="office-365-activations-reports"></a>Office 365-Aktivierungsberichte

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Der Office 365 Activation Bericht bietet eine Ansicht, von der Benutzer ihre Office 365-Abonnements auf mindestens ein Gerät aktiviert haben. Es bietet eine Aufschlüsselung der Office 365 ProPlus, Project und Visio Pro für Office 365-Abonnement Aktivierungen als auch die Aufgliederung der Aktivierungen über Desktop und Geräte. In diesem Bericht konnte können Sie die Benutzer zu identifizieren, die möglicherweise zusätzliche Unterstützung für ihre Office-Abonnement zu aktivieren.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Microsoft Office-Aktivierungen](https://support.office.com/client/Office-activations-87c24ae2-82e0-4d1e-be01-c3bcc3f18c60).

## <a name="reports"></a>Berichte
| Function                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getoffice365activationsuserdetail.md) | Stream          | [office365ActivationsUserDetail](../resources/office365activationsuserdetail.md) | Erhalten Sie detaillierte Informationen über Benutzer, die Office 365 aktiviert haben. |
| [Aktivierungsanzahl abrufen](../api/reportroot-getoffice365activationcounts.md) | Stream          | [office365ActivationCounts](../resources/office365activationcounts.md) | Erfahren Sie, wie viele Office 365-Aktivierungen auf Desktops und Geräten durchgeführt wurden. |
| [Benutzeranzahl abrufen](../api/reportroot-getoffice365activationsusercounts.md) | Stream          | [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) | Rufen Sie die Anzahl der aktivierten Benutzer ab und erfahren Sie, wie viele Benutzer das Office-Abonnement auf dem Desktop oder einem Gerät aktiviert haben. |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/office-365-activations-reports.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
