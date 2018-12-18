---
title: Ressourcentyp educationSynchronizationConnectionSettings
description: 'Stellt die Einstellungen für die Anbieter-Verbindung dar. Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden. '
author: mmast-msft
ms.openlocfilehash: 4e8b62a46fa6d14508a9d57ffedc46411910433d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350624"
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