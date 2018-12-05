---
title: E-Mail-App-Verwendungsbericht
description: Sie können sehen, wie viele e-Mail-apps für die Verbindung zu Exchange Online verwendet werden. Sie können auch nachsehen, welche Versionen von Outlook-Apps verwendet werden, sodass Sie Benutzer informieren können, die auf unterstützte Outlook-Versionen upgraden sollten.
ms.openlocfilehash: 0511bfb2832bac761ed1e56dfb18a41fc93beb01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063553"
---
# <a name="email-app-usage-reports"></a>E-Mail-App-Verwendungsbericht

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Sie können sehen, wie viele e-Mail-apps für die Verbindung zu Exchange Online verwendet werden. Sie können auch nachsehen, welche Versionen von Outlook-Apps verwendet werden, sodass Sie Benutzer informieren können, die auf unterstützte Outlook-Versionen upgraden sollten.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Nutzung von E-Mail-Apps](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getemailappusageuserdetail.md) | Stream          | [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) | Erhalten Sie detaillierte Informationen darüber, welche Aktivitäten Benutzer mit den verschiedenen E-Mail-Apps ausgeführt haben. |
| [Benutzeranzahl für Apps abrufen](../api/reportroot-getemailappusageappsusercounts.md) | Stream          | [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) | Rufen Sie die Anzahl der eindeutigen Benutzer pro E-Mail-App ab. |
| [Benutzeranzahl abrufen](../api/reportroot-getemailappusageusercounts.md) | Stream          | [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) | Rufen Sie die Anzahl der eindeutigen Benutzer ab, die über eine E-Mail-App mit Exchange Online verbunden sind. |
| [Benutzeranzahl für Versionen abrufen](../api/reportroot-getemailappusageversionsusercounts.md) | Stream          | [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) | Rufen Sie die Anzahl der eindeutigen Benutzer der Desktopversion von Outlook ab. |