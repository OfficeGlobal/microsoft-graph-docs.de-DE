---
title: Verwenden Sie die Benachrichtigungen REST-API in Microsoft Graph
description: Die API-Benachrichtigungen in Microsoft Graph können Sie um Pushbenachrichtigungen an einen Benutzer zu senden. Einfach Adressieren eines Benutzerkontos, um eine Benachrichtigung gesendet, und die Plattform bietet, die Benachrichtigung an alle Geräte Endpunkte. Benachrichtigungen API Anfragen werden ausgeführt, im Auftrag eines Benutzers über delegierten Berechtigungen und die [Benachrichtigung über die Berechtigung]( /graph/permissions_reference), der mit einer Microsoft-Konten verwendet werden kann oder Arbeit oder Schule Konten.
localization_priority: Priority
ms.openlocfilehash: 04787cb9a9b589036020651934041b4fc399adb1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853025"
---
# <a name="use-the-notifications-rest-api-in-microsoft-graph"></a>Verwenden Sie die Benachrichtigungen REST-API in Microsoft Graph

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Die API-Benachrichtigungen in Microsoft Graph können Sie um Pushbenachrichtigungen an einen Benutzer zu senden. Einfach Adressieren eines Benutzerkontos, um eine Benachrichtigung gesendet, und die Plattform bietet, die Benachrichtigung an alle Geräte Endpunkte. Benachrichtigungen API Anfragen werden ausgeführt, im Auftrag eines Benutzers über [Berechtigungen delegiert](/graph/permissions-reference#delegated-permissions-application-permissions-and-effective-permissions) und die [Benachrichtigung über die Berechtigung]( /graph/permissions_reference), der mit einer Microsoft-Konten verwendet werden kann oder Arbeit oder Schule Konten.
Diese Art von Benutzer-centric Benachrichtigung wird durch die [Benachrichtigung](../resources/projectrome-notification.md) Ressource dargestellt und in Microsoft Graph gespeichert ist. Es kann dann zugegriffen und verwaltet werden von der Veröffentlichung app über die [Project-ROM-SDK-APIs](https://github.com/Microsoft/project-rome). 

## <a name="next-steps"></a>Nächste Schritte
- Finden Sie in der [Benachrichtigung Ressource](../resources/projectrome-notification.md) und erstellen Sie Benachrichtigungen ausschließlich für die Benutzer zu. 
- Probieren Sie die API im [Graph-Tester](https://developer.microsoft.com/graph/graph-explorer) aus.
