---
title: ClonableTeamParts Enum-Typ
description: 'Beschreibt, welche Teil eines Teams geklont werden soll. '
localization_priority: Normal
ms.openlocfilehash: 7eb71de266ea4f0ed9f94900dd03a47da1a24cc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860557"
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
