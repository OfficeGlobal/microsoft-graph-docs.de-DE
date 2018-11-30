---
title: Verwalten von Telekommunikationsausgaben in Microsoft Intune
description: Sie können den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben nutzen, um die Datennutzung und das Roaming auf unternehmenseigenen Geräten zu beschränken. Der Service ist mit Intune integriert. Er ermöglicht es Ihnen, Nutzungslimits festzulegen und durchzusetzen. Benutzern wird eine Benachrichtigung gesendet, sobald sie einen konfigurierten Schwellenwert überschreiten. Sie können den Dienst auch so konfigurieren, dass er bestimmte Aktionen ausführt, wenn Benutzer den Schwellenwert überschreiten. So kann er beispielsweise das Roaming deaktivieren. In der Saaswedo-Konsole stehen Berichte mit Informationen zur Datennutzung und Überwachungsinformationen zur Verfügung. Bevor Sie den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben mit Intune nutzen können, müssen Sie Einstellungen in einer Saaswedo-Konsole und in Intune konfigurieren. Die Verbindung muss sowohl aufseiten das Saaswedo-Diensts als auch aufseiten von Intune aktiviert sein. Falls die Verbindung aufseiten von Saaswedo aktiviert ist, nicht aber aufseiten von Intune, empfängt Intune Meldungen, ignoriert sie jedoch.
ms.openlocfilehash: b7b5eab316b0ad1f9e4cc25a42e7f36de7981ea5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27063966"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a>Verwalten von Telekommunikationsausgaben in Microsoft Intune

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

> **Hinweis:** Die Verwendung der Microsoft Graph-APIs zum Konfigurieren von Intune-Steuerelementen und -Richtlinien erfordert dennoch, dass der Intune-Dienst vom Kunden [ordnungsgemäß lizenziert](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) ist.

Sie können den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben nutzen, um die Datennutzung und das Roaming auf unternehmenseigenen Geräten zu beschränken. Der Service ist mit Intune integriert. Er ermöglicht es Ihnen, Nutzungslimits festzulegen und durchzusetzen. Benutzern wird eine Benachrichtigung gesendet, sobald sie einen konfigurierten Schwellenwert überschreiten. Sie können den Dienst auch so konfigurieren, dass er bestimmte Aktionen ausführt, wenn Benutzer den Schwellenwert überschreiten. So kann er beispielsweise das Roaming deaktivieren. In der Saaswedo-Konsole stehen Berichte mit Informationen zur Datennutzung und Überwachungsinformationen zur Verfügung. Bevor Sie den Saaswedo-Dienst zur Verwaltung von Telekommunikationsausgaben mit Intune nutzen können, müssen Sie Einstellungen in einer Saaswedo-Konsole und in Intune konfigurieren. Die Verbindung muss sowohl aufseiten das Saaswedo-Diensts als auch aufseiten von Intune aktiviert sein. Falls die Verbindung aufseiten von Saaswedo aktiviert ist, nicht aber aufseiten von Intune, empfängt Intune Meldungen, ignoriert sie jedoch.

Zur Verwaltung von Telekommunikationsausgaben in Intune stehen die folgenden Graph-Ressourcen zur Verfügung:

- [telecomExpenseManagementPartner](intune-tem-telecomexpensemanagementpartner.md)
