---
title: Ressourcentyp educationSynchronizationConnectionSettings
description: 'Stellt die Einstellungen für die Anbieter-Verbindung dar. Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden. '
ms.openlocfilehash: 27cdd377318d3294be9802b7cf28e940d0ada31c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27062404"
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
| **clientId** | String |  Client-ID für die Verbindung an den Anbieter verwendet. |
| **clientSecret** | String |  Geheimer Clientschlüssel zum Authentifizieren der Verbindungs an den Anbieter. |