---
title: E-Mail-App-Verwendungsbericht
description: Sie können sehen, wie viele e-Mail-apps für die Verbindung zu Exchange Online verwendet werden. Sie können auch nachsehen, welche Versionen von Outlook-Apps verwendet werden, sodass Sie Benutzer informieren können, die auf unterstützte Outlook-Versionen upgraden sollten.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: reports
ms.openlocfilehash: 6a75b494705c56e63d4b7d5b2f58d76de64b9bce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912918"
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
