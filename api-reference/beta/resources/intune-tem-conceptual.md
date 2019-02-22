---
title: Telekom-Spesenverwaltung in Microsoft InTune – Microsoft Graph-API
description: Listet die Microsoft Graph-API für InTune-Endpunkte (REST) im Zusammenhang mit der Telekom-Spesenverwaltung für eine mandantenorganisation auf.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 5168ee7887ded7c850023744d8234daa8723fe03
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145640"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a>Verwalten von Telekommunikationsausgaben in Microsoft Intune

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Sie können den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben nutzen, um die Datennutzung und das Roaming auf unternehmenseigenen Geräten zu beschränken. Der Service ist mit Intune integriert. Er ermöglicht es Ihnen, Nutzungslimits festzulegen und durchzusetzen. Benutzern wird eine Benachrichtigung gesendet, sobald sie einen konfigurierten Schwellenwert überschreiten. Sie können den Dienst auch so konfigurieren, dass er bestimmte Aktionen ausführt, wenn Benutzer den Schwellenwert überschreiten. So kann er beispielsweise das Roaming deaktivieren. In der Saaswedo-Konsole stehen Berichte mit Informationen zur Datennutzung und Überwachungsinformationen zur Verfügung. Bevor Sie den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben mit Intune nutzen können, müssen Sie Einstellungen in einer Saaswedo-Konsole und in Intune konfigurieren. Die Verbindung muss sowohl aufseiten das Saaswedo-Diensts als auch aufseiten von Intune aktiviert sein. Falls die Verbindung aufseiten von Saaswedo aktiviert ist, nicht aber aufseiten von Intune, empfängt Intune Meldungen, ignoriert sie jedoch.

Zur Verwaltung von Telekommunikationsausgaben in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:

- [telecomExpenseManagementPartner](intune-tem-telecomexpensemanagementpartner.md)
