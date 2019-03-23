---
title: Update tiIndicator
description: Aktualisieren der Eigenschaften eines tiIndicator-Objekts.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 55613e3c13695a502b43c127c1164d2adf9f6534
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789669"
---
# <a name="update-tiindicator"></a>Update tiIndicator

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aktualisieren der Eigenschaften eines [tiIndicator](../resources/tiindicator.md) -Objekts.

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten) |
|:---------------------------------------|:--------------------------------------------|
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | ThreatIndicators.ReadWrite.OwnedBy |
| Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
| Anwendung                            | ThreatIndicators.ReadWrite.OwnedBy |

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/tiIndicators/{id}
```

## <a name="request-headers"></a>Anforderungsheader

| Name       | Beschreibung|
|:-----------|:-----------|
| Authorization | Bearer {Code} **erforderlich** |
|Prefer | Return = Darstellung |

## <a name="request-body"></a>Anforderungstext

Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|action|Zeichenfolge| Die Aktion, die angewendet werden soll, wenn das Symbol im targetProduct-Sicherheitstool abgeglichen wird. Mögliche Werte sind: `unknown`, `allow`, `block` und `alert`.|
|activityGroupNames|String collection|Die Namen der Cyber Threat Intelligence für die Parteien, die für die bösartigen Aktivitäten verantwortlich sind, die vom Bedrohungs Indikator erfasst werden.|
|Zusatzinformationen|String|Ein CatchAll Bereich, in dem zusätzliche Daten aus dem Indikator, die nicht von anderen tiIndicator-Eigenschaften abgedeckt werden, möglicherweise eingefügt werden. Daten, die in Zusatzinformationen werden, werden in der Regel nicht vom targetProduct-Sicherheitstool verwendet.|
|confidence|Int32|Eine ganze Zahl, die die Vertrauenswürdigkeit der Daten innerhalb des Indikators kennzeichnet. Zulässige Werte sind 0 – 100, wobei 100 der höchste Wert ist.|
|description|Zeichenfolge|Kurze Beschreibung (100 Zeichen oder kleiner) der Bedrohung, dargestellt durch den Indikator.|
|diamondModel|[diamondModel](#diamondmodel-values)|Der Bereich des Diamant Modells, in dem dieser Indikator vorhanden ist. Mögliche Werte: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.|
|expirationDateTime|DateTimeOffset| DateTime-Zeichenfolge, die angibt, wann das Symbol abläuft. Alle Indikatoren benötigen ein Ablaufdatum, um zu verhindern, dass veraltete Indikatoren im System beibehalten werden. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`.|
|externalId|String|Eine Identifikationsnummer, die den Indikator zurück an das System des Indikator Anbieters bindet (beispielsweise einen Fremdschlüssel).|
|isActive|Boolesch|Wird verwendet, um Indikatoren innerhalb von System zu deaktivieren. Standardmäßig werden alle übermittelten Indikatoren als aktiv festgelegt. Anbieter können jedoch vorhandene Indikatoren mit dieser Einstellung auf "false" übermitteln, um Indikatoren im System zu deaktivieren.|
|killChain|[killChain](#killchain-values) -Sammlung|Ein JSON-Array von Zeichenfolgen, die beschreiben, welche Punkte auf der Killkette dieser Indikator erreicht. Genaue Werte finden Sie weiter unten unter "killChain-Werte".|
|knownFalsePositives|String|Szenarien, in denen das Symbol zu falsch positiven Ergebnissen führen kann. Dies sollte ein lesbarer Text sein.|
|lastReportedDateTime|DateTimeOffset|Der Zeitpunkt, zu dem der Indikator zuletzt angezeigt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `2014-01-01T00:00:00Z`|
|malwareFamilyNames|String collection|Der Name der Schadsoftware-Familie, die mit einem Indikator verknüpft ist, falls vorhanden. Microsoft bevorzugt den Namen der Microsoft-Schadsoftware-Familie, falls möglich, der über die [Bedrohungs Enzyklopädie](https://www.microsoft.com/wdsi/threats)Windows Defender Security Intelligence gefunden werden kann.|
|passiveOnly|Boolesch|Bestimmt, ob das Symbol ein Ereignis auslösen soll, das für einen Endbenutzer sichtbar ist. Bei Festlegung auf "true" werden vom Endbenutzer keine Sicherheitstools benachrichtigt, dass ein "Hit" aufgetreten ist. Diese wird am häufigsten von Sicherheitsprodukten als Überwachungs-oder Unbeaufsichtigter Modus behandelt, in dem Sie einfach protokollieren, ob eine Übereinstimmung aufgetreten ist, die Aktion jedoch nicht ausgeführt wird. Standardwert ist "false".|
|Schweregrad|Int32|Eine ganze Zahl, die den Schweregrad des böswilligen Verhaltens darstellt, das durch die Daten innerhalb des Indikators identifiziert wird. Zulässige Werte sind 0 – 5, wobei 5 der schwerste ist und NULL nicht schwerwiegend ist. Der Standardwert ist 3.|
|tags|String-Sammlung|Ein JSON-Array von Zeichenfolgen, in dem beliebige Tags/Schlüsselwörter gespeichert werden.|
|tlpLevel|[tlpLevel](#tlplevel-values)| Ampel-Protokollwert für das Symbol. Mögliche Werte: `unknown`, `white`, `green`, `amber`, `red`.|

### <a name="diamondmodel-values"></a>diamondModel-Werte

Informationen zu diesem Modell finden Sie unter [Diamond Model](http://diamondmodel.org).

| Werte | Beschreibung |
|:-------|:------------|
|Gegner|Der Indikator beschreibt den Gegner.|
|Fähigkeit|Das Symbol ist eine Funktion des Gegners.|
|Infrastruktur|Der Indikator beschreibt die Infrastruktur des Gegners.|
|Opfer|Der Indikator beschreibt das Opfer des Gegners.|

### <a name="killchain-values"></a>killChain-Werte

| Werte | Beschreibung |
|:-------|:------------|
|Aktionen|Stellt "Aktionen für Ziele" dar. Der Angreifer nutzt das kompromittierte System, um Aktionen wie einen verteilten Denial-of-Service-Angriff zu ergreifen.|
|C2 befindet|Stellt den Steuerelement Kanal dar, durch den ein kompromittiertes System bearbeitet wird.|
|Delivery|Der Prozess der Verteilung des Exploit-Codes auf die Opfer (beispielsweise USB, e-Mail, Websites).|
|Ausbeutung|Der Exploitcode nutzt Sicherheitsrisiken aus (beispielsweise Codeausführung).|
|Installation|Installieren von Schadsoftware, nachdem eine Sicherheitsanfälligkeit ausgenutzt wurde.|
|Aufklärungs|Indikator ist ein Beweis für die Verwendung einer Aktivitätsgruppen-ernteinformationen, die bei zukünftigen Angriffen verwendet werden sollen.|
|Stationierung|Aktivieren einer Sicherheitsanfälligkeit in Exploitcode (beispielsweise Schadsoftware).|

### <a name="tlplevel-values"></a>tlpLevel-Werte

Jeder Indikator muss einen TLP-Wert (Traffic Light Protocol) haben, wenn er übermittelt wird. Dieser Wert stellt die Vertraulichkeit und den freigabebereich eines bestimmten Indikators dar.

| Werte | Beschreibung |
|:-------|:------------|
|Weiß| Freigabebereich: unLimited. Indikatoren können frei freigegeben werden, ohne Einschränkungen.|
|Grün| Freigabebereich: Community. Indikatoren können für die Sicherheitscommunity freigegeben werden.|
|Bernstein| Freigabebereich: Limited. Dies ist die Standardeinstellung für Indikatoren und schränkt die Freigabe nur für Personen ein, die über einen need-to-Know: 1-Dienst verfügen, und die Dienst Operatoren, die Bedrohungs Intelligenz implementieren. 2) Kunden, deren System (s) Verhalten mit dem Indikator übereinstimmt.|
|Rot| Freigabebereich: persönlich. Diese Indikatoren sollen nur direkt und, vorzugsweise persönlich, freigegeben werden. In der Regel werden TLP-rote Indikatoren aufgrund der vordefinierten Einschränkungen nicht aufgenommen. Wenn TLP-rote Indikatoren übermittelt **** werden, sollte auch die passiveOnly `True` -Eigenschaft auf festgelegt werden. |

## <a name="response"></a>Antwort

Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.

Wenn der optionale Anforderungsheader verwendet wird, gibt die Methode `200 OK` den Antwortcode und das aktualisierte [tiIndicator](../resources/tiIndicator.md) -Objekt im Antworttext zurück.

## <a name="examples"></a>Beispiele

### <a name="example-1-request-without-prefer-header"></a>Beispiel 1: Anforderung ohne vorZugs Kopfzeile

#### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel für die Anforderung ohne `Prefer` den Header.
<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json

{
  "description": "description-updated",
}
```

#### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-request-with-prefer-header"></a>Beispiel 2: Anforderung mit vorZugs Kopfzeile

#### <a name="request"></a>Anforderung

Nachfolgend sehen Sie ein Beispiel für die Anforderung, die `Prefer` den Header enthält.

<!-- {
  "blockType": "request",
  "name": "update_tiIndicator"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/tiIndicators/{id}
Content-type: application/json
Prefer: return=representation

{
  "additionalInformation": "additionalInformation-after-update",
  "confidence": 42,
  "description": "description-after-update",
}
```

#### <a name="response"></a>Antwort

Nachfolgend sehen Sie ein Beispiel der Antwort.

> [!NOTE]
> Das hier gezeigte Antwortobjekt kann zur Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tiIndicator"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Security/tiIndicators/$entity",
    "id": "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
    "azureTenantId": "XXXXXXXXXXXXXXXXXXXXXXXXX",
    "action": null,
    "additionalInformation": "additionalInformation-after-update",
    "activityGroupNames": [],
    "confidence": 42,
    "description": "description-after-update",
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
