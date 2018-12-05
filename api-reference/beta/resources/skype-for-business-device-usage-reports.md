---
title: Verwendungsberichte für Skype for Business-Gerät
description: Erhalten Sie Informationen über die Arten von Clients und Geräten, die verwendet werden in Ihrer Organisation. Diese Details sind sehr hilfreich, wenn Sie andere Geschäftsentscheidungen für Ihre Organisation in Erwägung ziehen, planen und durchführen.
ms.openlocfilehash: 7b77a78026475f8690f5ea47cc70db86b654450f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063542"
---
# <a name="skype-for-business-device-usage-reports"></a>Verwendungsberichte für Skype for Business-Gerät

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Erhalten Sie Informationen über die Arten von Clients und Geräten, die verwendet werden in Ihrer Organisation. Diese Details sind sehr hilfreich, wenn Sie andere Geschäftsentscheidungen für Ihre Organisation in Erwägung ziehen, planen und durchführen.

> **Hinweis:** Ausführliche Informationen zu anderen Berichtsansichten und -namen finden Sie unter [Office 365-Berichte – Verwendete Skype for Business-Clients](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).

## <a name="reports"></a>Berichte

| Funktion                                 | Rückgabetyp CSV | Rückgabetyp JSON                         | Beschreibung                              |
| :--------------------------------------- | :-------------- | :--------------------------------------- | ---------------------------------------- |
| [Benutzerdetails abrufen](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md) | Stream          | [skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md) | Rufen Sie Details der Skype for Business-Gerätenutzung nach Benutzer ab. |
| [Benutzeranzahl für Verteilung abrufen](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md) | Stream          | [skypeForBusinessDeviceUsageDistributionUserCounts](../resources/skypeforbusinessdeviceusagedistributionusercounts.md) | Rufen Sie die Anzahl der Benutzer ab, die eigene Geräte in Ihrer Organisation verwenden. Der Bericht enthält die Anzahl der Benutzer pro Gerät, einschließlich Windows, Windows Phone, Android-Smartphone, iPhone und iPad. |
| [Benutzeranzahl abrufen](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md) | Stream          | [skypeForBusinessDeviceUsageUserCounts](../resources/skypeforbusinessdeviceusageusercounts.md) | Erfahren Sie mehr über Auslastungstrends, indem Sie sich ansehen, wie viele Benutzer in Ihrer Organisation sich über die Skype for Business-App verbunden haben. Außerdem erhalten Sie eine Auflistung des Gerätetyps (Windows, Windows Phone, Android-Smartphone, iPhone oder iPad) auf dem die Skype for Business-Client-App installiert und in Ihrer Organisation verwendet wird. |