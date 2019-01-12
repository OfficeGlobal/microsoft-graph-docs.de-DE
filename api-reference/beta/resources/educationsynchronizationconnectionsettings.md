---
title: Ressourcentyp educationSynchronizationConnectionSettings
description: 'Stellt die Einstellungen für die Anbieter-Verbindung dar. Dadurch wird das System wissen, wie Sie mit der Anbieter APIs verbinden. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f9bb19ec9c09b06dd007eb2031f3dbb176eb12d3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978228"
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
