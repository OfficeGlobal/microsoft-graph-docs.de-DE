---
title: Ressourcentyp educationSynchronizationConnectionSettings
description: 'Stellt die Einstellungen für die Anbieter-Verbindung dar. Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden. '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 17fedb5094016bd3df3bd8262390eaa7eeb37537
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841769"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a>Ressourcentyp educationSynchronizationConnectionSettings

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt die Einstellungen für die Anbieter-Verbindung dar. Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden. 

> **Hinweis:** Dieser komplexe Typ ist abstrakt. Verweisen Sie auf die bestimmten Arten von Verbindungseinstellungen aufgeführt.

## <a name="derived-types"></a>Abgeleitete Typen
| Typ | Beschreibung | 
|:-|:-|
| [**educationSynchronizationOAuth1ConnectionSettings**](educationsynchronizationoauth1connectionsettings.md) | Verwenden Sie diesen Typ OAuth1 Verbindungseinstellungen bereitstellen. |
| [**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | Verwenden Sie diesen Typ OAuth2 Client Anmeldeinformationen Grant-Verbindungseinstellungen bereitstellen. |

## <a name="properties"></a>Eigenschaften

| Eigenschaft | Typ | Beschreibung |
|:-|:-|:-|
| **clientId** | Zeichenfolge |  Client-ID für die Verbindung an den Anbieter verwendet. |
| **clientSecret** | Zeichenfolge |  Geheimer Clientschlüssel zum Authentifizieren der Verbindungs an den Anbieter. |
