---
title: richtlinienressourcentyp
description: 'Stellt eine Azure AD-Richtlinie. Richtlinien sind benutzerdefinierte Regeln, die erzwungen werden können, klicken Sie auf Anwendungen, Dienstprinzipale, Gruppen oder die gesamte Organisation, den, der Sie zugeordnet sind. Derzeit nur einen Typ der Richtlinie zur Verfügung stehen:'
localization_priority: Normal
ms.openlocfilehash: cc82dc32056b9da5c2ca1144e58b5b9e1fe326f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830926"
---
# <a name="policy-resource-type"></a>richtlinienressourcentyp

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Stellt eine Azure AD-Richtlinie. Richtlinien sind benutzerdefinierte Regeln, die erzwungen werden können, klicken Sie auf Anwendungen, Dienstprinzipale, Gruppen oder die gesamte Organisation, den, der Sie zugeordnet sind. Derzeit nur einen Typ der Richtlinie zur Verfügung stehen:

- Richtlinien für die Gültigkeitsdauer Token – gibt die Dauer Lebensdauer für Anwendungen und Dienstprinzipale ausgestellten Token.

Mit dieser Richtlinie wird ausführlich beschrieben.

## <a name="methods"></a>Methoden
| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
| [Abrufen von Gruppenrichtlinien](../api/policy-get.md) |Richtlinie|Liest Eigenschaften und Beziehungen des Benutzerobjekts.|
|[Richtlinie erstellen](../api/policy-post.md)|Richtlinie|Erstellen Sie ein neues Gruppenrichtlinienobjekt.|
|[Update-Richtlinie](../api/policy-update.md)|Keine|Group Policy Object zu aktualisieren.|
|[Löschrichtlinie](../api/policy-delete.md)|Keine|Löschen Sie Richtlinienobjekt.|
|[Zuweisen der Richtlinie](../api/policy-assign.md)|Keine|Zuweisen einer Richtlinie zu einer Anwendung Dienstprinzipal.|
|[Listenrichtlinien](../api/policy-list.md)|Auflistung von Gruppenrichtlinien|Rufen Sie aller Gruppenrichtlinienobjekte in der Organisation ab.|
|[Zugewiesen-Listenrichtlinien](../api/policy-list-assigned.md)|Auflistung von Gruppenrichtlinien|Rufen Sie alle Richtlinienobjekte an eine Anwendung oder Dienstprinzipal zugewiesen.|

### <a name="common-properties"></a>Allgemeine Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|definition|String|Die Version der bestimmte Richtlinie Zeichenfolge. Siehe unten. Erforderlich.|
|displayName|String|Ein benutzerdefinierter Name für die Richtlinie ein. Erforderlich.|
|IsOrganizationDefault|Boolean|Wenn auf true ist, aktivieren Sie diese Richtlinie festgelegt. Viele Richtlinien für den gleichen Richtlinientyp kann, jedoch nur eine Organisation standardmäßig aktiviert werden kann. Optional, ist Standardwert false.|
|type|String|Gibt den Typ der Richtlinie an. Derzeit muss "TokenLifetimePolicy". Erforderlich.|

#### <a name="common-relationships"></a>Allgemeine Beziehungen
|Beziehung|Typ|Beschreibung|
|:-------------|:-----------|:-----------|
|appliesTo|[directoryObject](../resources/directoryobject.md)-Sammlung|Die Anwendungen, Dienstprinzipale, Gruppen oder Organisation wendet die Richtlinie an.|

## <a name="token-lifetime-policy"></a>Gültigkeitsdauer von Token-Richtlinie
Gibt die Lebensdauer der für verschiedene Zwecke ausgestellten Token an. Diese Art der Richtlinie kann Anwendungen und Dienstprinzipale [zugewiesen](../api/policy-assign.md) sein. Es gibt vier Arten von Token, deren Lebensdauer konfiguriert werden können. Access/aktualisieren token-Paare werden während der Authentifizierung über einen Client abgerufen, während die ID-Sitzung token-Paare während der Authentifizierung über einen Browser abgerufen werden.

- **Access-Token** enthält Informationen über die Identität und die Berechtigungen für ein Benutzerkonto, das Zugriff auf geschützte Ressourcen wie Anwendungen von Clients verwendet wird.
- **Token aktualisieren** wird zusammen mit der Zugriffstoken abgerufen, wenn ein Benutzer mit Azure AD über einen Client Zugriff auf eine geschützte Ressource authentifiziert. Während es ist nicht gesperrt oder nicht verwendete von für mehr als die MaxInactiveTime (siehe unten links), können sie ein neues Access/aktualisieren Paar token erhalten, wenn das aktuelle Zugriffstoken läuft ab verwendet werden.
- **Token-ID** verhält sich wie ein Zugriffstoken, jedoch über den Browser abgerufen.
- **Sitzung Token** verhält sich wie ein Aktualisierungstoken, aber über den Browser abgerufen.

## <a name="properties"></a>Eigenschaften
Die folgenden Eigenschaften bilden das JSON-Objekt, das eine Richtlinie Gültigkeitsdauer von token darstellt. Diese JSON-Objekt muss **in eine Zeichenfolge mit Anführungszeichen Escapezeichen konvertiert** in der Eigenschaft "Definition" allgemeine Richtlinie eingefügt werden soll. Ein Beispiel ist unten aufgeführt:

>Hinweis: Es werden alle Zeitdauern in diese Eigenschaften im Format "TT.hh" angegeben.

>Hinweis: Max-Werte für Eigenschaften in "Tagen" gekennzeichnet sind 1 Sekunde kleiner als die bezeichnet Anzahl von Tagen. Beispielsweise wird der maximale Wert von 1 Tagen angegeben, als "23: 59:59".

| Eigenschaft     | Typ   |Beschreibung| Mindestwert | Max-Wert | Standardwert|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|Steuert, wie lange **Zugriff und ID-Token** als gültig betrachtet werden.|10 Minuten|1 Tag|1 Stunde|
|MaxInactiveTime|String|Steuert, wie ALT ein Aktualisierungstoken sein kann, bevor ein Client nicht mehr zum Abrufen eines neuen Access/aktualisieren token Paars Zugriff auf eine Ressource verwenden kann.|10 Minuten|90 Tage|14 Tage|
|MaxAgeSingleFactor|String|Steuerelemente wie lange kann Benutzer weiterhin Aktualisierungstoken verwenden, um neue Access/aktualisieren abzurufen token-Paare nach dem letzten Mal, das Sie authentifiziert, erfolgreich mit nur einem einzigen Faktor. Da einfache weniger als mehrstufige Authentifizierung sicher angesehen wird, wird empfohlen, dass diese Richtlinie auf einen Wert gleich oder kleiner als der MultiFactorRefreshTokenMaxAge festgelegt ist.|10 Minuten|erst gesperrt|365 Tage oder erst gesperrt|
|MaxAgeMultiFactor|String|Aktualisierungstoken verwenden, um neue Access/aktualisieren abzurufen token-Paare nach dem letzten Mal, das Sie authentifiziert, erfolgreich mit mehreren Faktoren kann Steuerelemente wie lange ein Benutzer weiterhin.|10 Minuten|erst gesperrt|365 Tage oder erst gesperrt|
|MaxAgeSessionSingleFactor|String|Steuerelemente wie lange kann Benutzer weiterhin Sitzungstoken verwenden, um neue ID-Sitzung-Token abzurufen, nach dem Zeitpunkt der letzten sie mit nur einem einzigen Faktor erfolgreich authentifiziert. Da einfache weniger als mehrstufige Authentifizierung sicher angesehen wird, wird empfohlen, dass diese Richtlinie auf einen Wert gleich oder kleiner als der MultiFactorSessionTokenMaxAge festgelegt ist|10 Minuten|erst gesperrt|365 oder erst gesperrt|
|MaxAgeSessionMultiFactor|String|Steuerelemente wie lange kann Benutzer weiterhin Sitzungstoken verwenden, um neue ID-Sitzung Token nach dem Zeitpunkt der letzten abrufen, die sie mit mehreren Faktoren erfolgreich authentifiziert.|10 Minuten|erst gesperrt|365 oder erst gesperrt|
|Version|Ganze Zahl|Der Wert 1 festgelegt. Erforderlich.|Keine|Keine|Keine|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

```json
{
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
  "displayName":"Test Policy",
  "isOrganizationDefault":false,
  "type":"TokenLifetimePolicy",
}
```
