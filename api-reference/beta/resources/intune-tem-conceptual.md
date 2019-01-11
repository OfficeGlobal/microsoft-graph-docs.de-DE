---
title: Verwalten von Telekommunikationsausgaben in Microsoft Intune
description: Sie können den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben nutzen, um die Datennutzung und das Roaming auf unternehmenseigenen Geräten zu beschränken. Der Service ist mit Intune integriert. Er ermöglicht es Ihnen, Nutzungslimits festzulegen und durchzusetzen. Benutzern wird eine Benachrichtigung gesendet, sobald sie einen konfigurierten Schwellenwert überschreiten. Sie können den Dienst auch so konfigurieren, dass er bestimmte Aktionen ausführt, wenn Benutzer den Schwellenwert überschreiten. So kann er beispielsweise das Roaming deaktivieren. In der Saaswedo-Konsole stehen Berichte mit Informationen zur Datennutzung und Überwachungsinformationen zur Verfügung. Bevor Sie den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben mit Intune nutzen können, müssen Sie Einstellungen in einer Saaswedo-Konsole und in Intune konfigurieren. Die Verbindung muss sowohl aufseiten das Saaswedo-Diensts als auch aufseiten von Intune aktiviert sein. Falls die Verbindung aufseiten von Saaswedo aktiviert ist, nicht aber aufseiten von Intune, empfängt Intune Meldungen, ignoriert sie jedoch.
localization_priority: Normal
ms.openlocfilehash: 010aa8203090522ac6071211eed0fb3e6b2f242d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813461"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a>Verwalten von Telekommunikationsausgaben in Microsoft Intune

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Sie können den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben nutzen, um die Datennutzung und das Roaming auf unternehmenseigenen Geräten zu beschränken. Der Service ist mit Intune integriert. Er ermöglicht es Ihnen, Nutzungslimits festzulegen und durchzusetzen. Benutzern wird eine Benachrichtigung gesendet, sobald sie einen konfigurierten Schwellenwert überschreiten. Sie können den Dienst auch so konfigurieren, dass er bestimmte Aktionen ausführt, wenn Benutzer den Schwellenwert überschreiten. So kann er beispielsweise das Roaming deaktivieren. In der Saaswedo-Konsole stehen Berichte mit Informationen zur Datennutzung und Überwachungsinformationen zur Verfügung. Bevor Sie den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben mit Intune nutzen können, müssen Sie Einstellungen in einer Saaswedo-Konsole und in Intune konfigurieren. Die Verbindung muss sowohl aufseiten das Saaswedo-Diensts als auch aufseiten von Intune aktiviert sein. Falls die Verbindung aufseiten von Saaswedo aktiviert ist, nicht aber aufseiten von Intune, empfängt Intune Meldungen, ignoriert sie jedoch.

Zur Verwaltung von Telekommunikationsausgaben in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:

- [telecomExpenseManagementPartner](intune-tem-telecomexpensemanagementpartner.md)
