---
title: ClonableTeamParts Enum-Typ
description: 'Beschreibt, welche Teil eines Teams geklont werden soll. '
localization_priority: Normal
ms.openlocfilehash: e7f7b1e8fa73bdd4a188e8d8f5d40635d302a023
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824129"
---
# <a name="clonableteamparts-enum-type"></a>ClonableTeamParts Enum-Typ



Beschreibt, welche Teil eines [Team](../resources/team.md) geklont werden soll. 

## <a name="members"></a>Elemente

| Element | Wert| Beschreibung |
|:---------------|:--------|:----------|
|Apps|1|Kopieren Sie die Liste der installierten apps.|
|Registerkarten|2|die Registerkarten in den Kanälen kopiert.|
|settings|4|Kopiert alle Einstellungen im Team, zusammen mit den wichtigsten gruppeneinstellungen.|
|Kanäle|8|kopiert die Struktur DDE-Kanal (jedoch nicht die Nachrichten im Kanal).|
|Elemente|16|kopiert die Elemente und Besitzer des Teams.|
