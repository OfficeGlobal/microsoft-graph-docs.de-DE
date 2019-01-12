---
title: Verwendungsberichte für Yammer-Gerät
description: Die Verwendungsberichte für das Yammer-Gerät geben Aufschluss darüber, welche Geräte Ihre Benutzer für die Nutzung von Yammer verwenden. Sie können sich die Anzahl der Benutzer nach Gerätetyp für einen gewählten Zeitraum ansehen und Details für einzelne Benutzer anzeigen.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: a68b1decf0690a07db07c880cec25a1bf2c01cfa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991958"
---
# <a name="yammer-device-usage-reports"></a>Verwendungsberichte für Yammer-Gerät

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt. Diese APIs werden in Microsoft Graph China vom Dienst 21Vianet nicht unterstützt.

Die Verwendungsberichte für das Yammer-Gerät geben Aufschluss darüber, welche Geräte Ihre Benutzer für die Nutzung von Yammer verwenden. Sie können sich die Anzahl der Benutzer nach Gerätetyp für einen gewählten Zeitraum ansehen und Details für einzelne Benutzer anzeigen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Yammer-Gerätenutzung](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getyammerdeviceusageuserdetail.md) | Stream          | [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) | Rufen Sie Details zur Yammer-Gerätenutzung nach Benutzer ab. |
| [Benutzeranzahl für Verteilung abrufen](../api/reportroot-getyammerdeviceusagedistributionusercounts.md) | Stream          | [yammerDeviceUsageDistributionUserCounts](../resources/yammerdeviceusagedistributionusercounts.md) | Erhalten Sie die Anzahl der Benutzer nach Gerätetyp.  |
| [Benutzeranzahl abrufen](../api/reportroot-getyammerdeviceusageusercounts.md) | Stream          | [yammerDeviceUsageUserCounts](../resources/yammerdeviceusageusercounts.md) | Erhalten Sie die Anzahl der täglichen Benutzer nach Gerätetyp. |
