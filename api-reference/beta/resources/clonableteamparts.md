---
title: ClonableTeamParts Enum-Typ
description: 'Beschreibt, welche Teil eines Teams geklont werden soll. '
ms.openlocfilehash: 123cdb5ff7fd4a4291df5d9352b0db466908cc3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27059479"
---
# <a name="clonableteamparts-enum-type"></a>ClonableTeamParts Enum-Typ

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Beschreibt, welche Teil eines [Team](../resources/team.md) geklont werden soll. 

## <a name="members"></a>Elemente

| Element | Wert| Beschreibung |
|:---------------|:--------|:----------|
|Apps|1|Kopieren Sie die Liste der installierten apps.|
|Registerkarten|2|die Registerkarten in den Kanälen kopiert.|
|settings|4|Kopiert alle Einstellungen im Team, zusammen mit den wichtigsten gruppeneinstellungen.|
|Kanäle|8|kopiert die Struktur DDE-Kanal (jedoch nicht die Nachrichten im Kanal).|
|Elemente|16|kopiert die Elemente und Besitzer des Teams.|
