---
title: tiIndicator-Ressourcentyp
description: Indikatoren für Threat Intelligence (TI) stellen Daten dar, die zum Identifizieren schädlicher Aktivitäten verwendet werden. Wenn Ihre Organisation mit Bedrohungs Indikatoren arbeitet, indem Sie Ihre eigenen generieren, über Open Source Feeds, Freigabe mit Partnerorganisationen oder-Gemeinschaften oder durch den Erwerb von Datenfeeds, dann möchten, werden Sie oft diese Indikatoren in verschiedenen Sicherheitseinstellungen verwenden. Tools für den Abgleich mit Protokolldaten. Mit der tiIndicators-Entität "Graph Security" können Sie Ihre Bedrohungs Indikatoren für die Aktionen von allow, Block oder Alert in Microsoft-Sicherheitstools hochladen.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 8b8f3fe9b37021a9dd90dc03e861a8a1ed9d69de
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30367120"
---
# <a name="tiindicator-resource-type"></a>tiIndicator-Ressourcentyp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indikatoren für Threat Intelligence (TI) stellen Daten dar, die zum Identifizieren schädlicher Aktivitäten verwendet werden. Wenn Ihre Organisation mit Bedrohungs Indikatoren arbeitet, indem Sie Ihre eigenen generieren, Sie von Open-Source-Feeds abrufen, mit Partnerorganisationen oder-Gemeinschaften teilen oder Datenfeeds erwerben, können Sie diese Indikatoren in verschiedenen Sicherheitseinstellungen verwenden. Tools für den Abgleich mit Protokolldaten. Mit der Microsoft Graph Security API- **TIINDICATORS** -Entität können Sie Ihre Bedrohungs Indikatoren für die Aktionen von allow, Block oder Alert in Microsoft-Sicherheitstools hochladen.

Die über **tiIndicators** hochgeLadenen Bedrohungs Indikatoren werden in Verbindung mit Microsoft Threat Intelligence verwendet, um eine angepasste Sicherheitslösung für Ihre Organisation bereitzustellen. Bei Verwendung der **tiIndicators** -Entität Geben Sie die Microsoft-Sicherheitslösung an, für die Sie die Indikatoren über die **targetProduct** -Eigenschaft verwenden möchten, und geben die Aktion (Allow, Block oder Alert) an, auf die die Sicherheitslösung angewendet werden soll. Anwenden der Indikatoren über die **Action** -Eigenschaft.

## <a name="methods"></a>Methoden

| Methode       | Rückgabetyp | Beschreibung |
|:-------------|:------------|:------------|
| [TiIndicator abrufen](../api/tiindicator-get.md) | [tiIndicator](tiindicator.md) | Lesen von Eigenschaften und Beziehungen des tiIndicator-Objekts. |
| [TiIndicator erstellen](../api/tiindicators-post.md) | [tiIndicator](tiindicator.md) | Erstellen Sie eine neue tiIndicator durch Veröffentlichung in der tiIndicators-Auflistung. |
| [TiIndicators aufListen](../api/tiindicators-list.md) | [tiIndicator](tiindicator.md) -Sammlung | Rufen Sie eine tiIndicator-Objektsammlung ab. |
| [Update](../api/tiindicator-update.md) | [tiIndicator](tiindicator.md) | Aktualisieren des tiIndicator-Objekts. |
| [Delete](../api/tiindicator-delete.md) | Keine | TiIndicator-Objekt löschen. |
|[deleteTiIndicators](../api/tiindicator-deletetiindicators.md)|Keine| Löschen Sie mehrere tiIndicator-Objekte.|
|[deleteTiIndicatorsByExternalId](../api/tiindicator-deletetiindicatorsbyexternalid.md)|Keine| Löschen Sie mehrere tiIndicator-Objekte `externalId` nach der-Eigenschaft.|
|[submitTiIndicators](../api/tiindicator-submittiindicators.md)|[tiIndicator](tiindicator.md) -Sammlung|Erstellen Sie neue tiIndicators, indem Sie eine tiIndicators-Auflistung veröffentlichen.|
|[updateTiIndicators](../api/tiindicator-updatetiindicators.md)|[tiIndicator](tiindicator.md) -Sammlung| Aktualisieren Sie mehrere tiIndicator-Objekte.|

## <a name="properties"></a>Eigenschaften

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|Aktion|string| Die Aktion, die angewendet werden soll, wenn das Symbol im targetProduct-Sicherheitstool abgeglichen wird. Mögliche Werte: `unknown`, `allow`, `block`, `alert`. **Erforderlich**|
|activityGroupNames|String collection|Die Namen der Cyber Threat Intelligence für die Parteien, die für die bösartigen Aktivitäten verantwortlich sind, die vom Bedrohungs Indikator erfasst werden.|
|Zusatzinformationen|Zeichenfolge|Ein CatchAll Bereich, in dem zusätzliche Daten aus dem Indikator, die nicht von anderen tiIndicator-Eigenschaften abgedeckt werden, möglicherweise eingefügt werden. Daten, die in Zusatzinformationen werden, werden in der Regel nicht vom targetProduct-Sicherheitstool verwendet.|
|azureTenantId|Zeichenfolge| Wird vom System gestempelt, wenn das Symbol aufgenommen wird. Die Azure Active Directory-Mandanten-ID des übermittelnden Clients. **Erforderlich**|
|confidence|Int32|Eine ganze Zahl, die die Vertrauenswürdigkeit der Daten innerhalb des Indikators kennzeichnet. Zulässige Werte sind 0 – 100, wobei 100 der höchste Wert ist.|
|description|Zeichenfolge| Kurze Beschreibung (100 Zeichen oder kleiner) der Bedrohung, dargestellt durch den Indikator. **Erforderlich**|
|diamondModel|string|Der Bereich des Diamant Modells, in dem dieser Indikator vorhanden ist. Mögliche Werte: `unknown`, `adversary`, `capability`, `infrastructure`, `victim`.|
|expirationDateTime|DateTimeOffset| DateTime-Zeichenfolge, die angibt, wann das Symbol abläuft. Alle Indikatoren benötigen ein Ablaufdatum, um zu verhindern, dass veraltete Indikatoren im System beibehalten werden. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`. **Erforderlich**|
|externalId|String| Eine Identifikationsnummer, die den Indikator zurück an das System des Indikator Anbieters bindet (beispielsweise einen Fremdschlüssel). |
|id|string|Wird vom System erstellt, wenn das Symbol aufgenommen wird. Generierte GUID/eindeutiger Bezeichner. Schreibgeschützt.|
|ingestedDateTime|DateTimeOffset| Wird vom System gestempelt, wenn das Symbol aufgenommen wird. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|isActive|Boolean| Wird verwendet, um Indikatoren innerhalb von System zu deaktivieren. Standardmäßig werden alle übermittelten Indikatoren als aktiv festgelegt. Anbieter können jedoch vorhandene Indikatoren mit dieser Einstellung auf "false" übermitteln, um Indikatoren im System zu deaktivieren.|
|killChain|String collection|Ein JSON-Array von Zeichenfolgen, die beschreiben, welche Punkte auf der Killkette dieser Indikator erreicht. Genaue Werte finden Sie unten unter "killChain-Werte". |
|knownFalsePositives|Zeichenfolge|Szenarien, in denen das Symbol zu falsch positiven Ergebnissen führen kann. Dies sollte ein lesbarer Text sein.|
|lastReportedDateTime|DateTimeOffset|Der Zeitpunkt, zu dem der Indikator zuletzt angezeigt wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|malwareFamilyNames|String collection|Der Name der Schadsoftware-Familie, die mit einem Indikator verknüpft ist, falls vorhanden. Microsoft bevorzugt den Namen der Microsoft-Schadsoftware-Familie, falls möglich, der über die [Bedrohungs Enzyklopädie](https://www.microsoft.com/wdsi/threats)Windows Defender Security Intelligence gefunden werden kann.|
|passiveOnly|Boolean |Bestimmt, ob das Symbol ein Ereignis auslösen soll, das für einen Endbenutzer sichtbar ist. Bei Festlegung auf "true" werden vom Endbenutzer keine Sicherheitstools benachrichtigt, dass ein "Hit" aufgetreten ist. Diese wird am häufigsten von Sicherheitsprodukten als Überwachungs-oder Unbeaufsichtigter Modus behandelt, in dem Sie einfach protokollieren, ob eine Übereinstimmung aufgetreten ist, die Aktion jedoch nicht ausgeführt wird. Der Standardwert ist "false". |
|Schweregrad|Int32| Eine ganze Zahl, die den Schweregrad des böswilligen Verhaltens darstellt, das durch die Daten innerhalb des Indikators identifiziert wird. Zulässige Werte sind 0 – 5, wobei 5 der schwerste ist und NULL nicht schwerwiegend ist. Der Standardwert ist 3. |
|tags|String-Sammlung|Ein JSON-Array von Zeichenfolgen, in dem beliebige Tags/Schlüsselwörter gespeichert werden. |
|targetProduct|Zeichenfolge|Ein String-Wert, der ein einzelnes Sicherheitsprodukt darstellt, auf das das Symbol angewendet werden soll. Zulässige Werte: `Azure Sentinel`. **Erforderlich**|
|threattype|Zeichenfolge| Jeder Indikator muss einen gültigen Indikator Bedrohungs aufweisen. Mögliche Werte: `Botnet`, `C2`, `CryptoMining`, `Darknet`, `DDoS`, `MaliciousUrl`, `Malware`, `Phishing`, `Proxy`, `PUA`, `WatchList`. **Erforderlich** |
|tlpLevel|string| Ampel-Protokollwert für das Symbol. Mögliche Werte: `unknown`, `white`, `green`, `amber`, `red`. **Erforderlich**|

### <a name="indicator-observables---email"></a>Indikator beobachtbaren – E-Mail

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|emailEncoding|Zeichenfolge|Der in der e-Mail verwendete Text Codierungs.|
|emailLanguage|Zeichenfolge|Die Sprache der e-Mail.|
|emailRecipient|Zeichenfolge|E-Mail-Adresse des Empfängers.|
|emailSenderAddress|Zeichenfolge|E-Mail-Adresse des attacker& # 124; Victim.|
|emailSenderName|Zeichenfolge|Der angezeigte Name des attacker&-Opfers.|
|emailSourceDomain|Zeichenfolge|In der e-Mail verwendete Domäne.|
|emailSourceIpAddress|Zeichenfolge|Quell-IP-Adresse der e-Mail.|
|emailSubject|Zeichenfolge|Betreffzeile der e-Mail.|
|emailXMailer|Zeichenfolge|Der in der e-Mail verwendete X-Mailer-Wert.|

### <a name="indicator-observables---file"></a>Indikator ObservableCollection-file

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|fileCompileDateTime|DateTimeOffset|DateTime, als die Datei kompiliert wurde. Der Timestamp-Typ stellt die Datums- und Uhrzeitinformationen mithilfe des ISO 8601-Formats dar und wird immer in UTC-Zeit angegeben. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|fileCreatedDateTime|DateTimeOffset| DateTime, als die Datei erstellt wurde. Der timestamp-Typ stellt Datums-und Uhrzeitinformationen unter Verwendung des ISO 8601-Formats dar und ist immer in UTC-Zeit. Mitternacht UTC-Zeit am 1. Januar 2014 würde z. B. wie folgt aussehen: `'2014-01-01T00:00:00Z'`|
|fileHashType|string| Der in fileHashvalue gespeicherte Hashtyp. Mögliche Werte sind: `unknown`, `sha1`, `sha256`, `md5`, `authenticodeHash256`, `lsHash` und `ctph`.|
|fileHashvalue|Zeichenfolge| Der Datei Hash Wert.|
|fileMutexname|Zeichenfolge| Mutexname, der bei dateibasierten Ermittlungen verwendet wird.|
|fileName|String|Name der Datei, wenn das Symboldatei basiert ist. Mehrere Dateinamen können durch Kommata getrennt werden. |
|filePacker|Zeichenfolge|Der Packer, der zum Erstellen der fraglichen Datei verwendet wird.|
|filePath|Zeichenfolge|Pfad der Datei, die eine Gefährdung angibt. Kann ein Windows-oder * nix-Pfad sein.|
|Größe|Int64|Die Größe der Datei in Byte.|
|fileType|Zeichenfolge| Text Beschreibung des Dateityps. Beispiel: "Word-Dokument" oder "Binary".|

### <a name="indicator-observables---network"></a>Indikator beobachtbar-Network

| Eigenschaft     | Typ        | Beschreibung |
|:-------------|:------------|:------------|
|Domänname|Zeichenfolge|Domänenname, der diesem Indikator zugeordnet ist. Sollte das Format Subdomain. Domain. TopLevelDomain (beispielsweise baddomain.domain.net) aufweisen.|
|networkCidrBlock|Zeichenfolge| CIDR-Block Notation Darstellung des Netzwerks, auf das in diesem Indikator verwiesen wird. Nur verwenden, wenn Quelle und Ziel nicht identifiziert werden können. |
|networkDestinationAsn|Int32|Die Ziel autonome System-ID des Netzwerks, auf das im Indikator verwiesen wird.|
|networkDestinationCidrBlock|Zeichenfolge|CIDR-Block Notation Darstellung des Zielnetzwerks in diesem Indikator.|
|networkDestinationIPv4|Zeichenfolge|IPv4-IP-Adress Ziel.|
|networkDestinationIPv6|Zeichenfolge|IPv6-IP-Adress Ziel.|
|networkDestinationPort|Int32|TCP-Port Ziel.|
|networkIPv4|Zeichenfolge| IPv4-IP-Adresse. Nur verwenden, wenn Quelle und Ziel nicht identifiziert werden können. |
|networkIPv6|Zeichenfolge| IPv6-IP-Adresse. Nur verwenden, wenn Quelle und Ziel nicht identifiziert werden können. |
|networkPort|Int32| TCP-Anschluß. Nur verwenden, wenn Quelle und Ziel nicht identifiziert werden können. |
|networkProtocol|Int32|Dezimaldarstellung des Protokoll Felds im IPv4-Header.|
|networkSourceAsn|Int32|Die Quelle des autonomen Systembezeichners des Netzwerks, auf das im Indikator verwiesen wird.|
|networkSourceCidrBlock|Zeichenfolge|CIDR-Block Notations Darstellung des Quellnetzwerks in diesem Indikator|
|networkSourceIPv4|Zeichenfolge|IPv4-IP-Adressquelle.|
|networkSourceIPv6|Zeichenfolge|IPv6-IP-Adressquelle.|
|networkSourcePort|Int32|TCP-Anschluß Quelle.|
|url|Zeichenfolge|Uniform Resource Locator. Diese URL muss RFC 1738 entsprechen.|
|userAgent|Zeichenfolge|Benutzer-Agent-Zeichenfolge aus einer Webanforderung, die auf eine Gefährdung hindeuten könnte.|

### <a name="diamondmodel-values"></a>diamondModel-Werte

Informationen zu diesem Modell finden Sie unter [Diamond Model](http://diamondmodel.org).

| Werte | Beschreibung |
|:-------|:------------|
|Gegner|Der Indikator beschreibt den Gegner.|
|Fähigkeit|Indikator ist eine Funktion des Widersachers.|
|Infrastruktur|Der Indikator beschreibt die Infrastruktur des Gegners.|
|Opfer|Der Indikator beschreibt das Opfer des Gegners.|

### <a name="killchain-values"></a>killChain-Werte

| Werte | Beschreibung |
|:-------|:------------|
|Aktionen|Indcates, dass der Angreifer das kompromittierte System nutzt, um Aktionen wie einen verteilten Denial-of-Service-Angriff zu ergreifen.|
|C2 befindet|Stellt den Steuerelement Kanal dar, durch den ein kompromittiertes System bearbeitet wird.|
|Lieferung|Der Prozess der Verteilung des Exploit-Codes auf die Opfer (beispielsweise USB, e-Mail, Websites).|
|Ausbeutung|Der Exploitcode nutzt Sicherheitsrisiken aus (beispielsweise Codeausführung).|
|Installation|Installieren von Schadsoftware, nachdem eine Sicherheitsanfälligkeit ausgenutzt wurde.|
|Aufklärungs|Indikator ist ein Beweis für die Verwendung einer Aktivitätsgruppen-ernteinformationen, die bei zukünftigen Angriffen verwendet werden sollen.|
|Stationierung|Aktivieren einer Sicherheitsanfälligkeit in Exploitcode (beispielsweise Schadsoftware).|

### <a name="threattype-values"></a>threattype-Werte

| Werte | Beschreibung |
|:-------|:------------|
|Botnet| Indikator zeigt einen Botnet-Knoten/-Member an.|
|C2 befindet|Indicator beschreibt einen Befehl &-Steuerelementknoten eines Botnets.|
|CryptoMining|Datenverkehr mit dieser Netzwerkadresse/-URL ist ein Hinweis auf CyrptoMining/Ressourcen Missbrauch.|
|Darknet|Indikator ist der eines Darknet-Knotens/-Netzwerks.
|DDoS|Indikatoren für eine aktive oder bevorstehende DDoS-Kampagne.|
|MaliciousUrl|URL, die Schadsoftware dient.|
|Schadsoftware|Indikator, der eine bösartige Datei oder Dateien beschreibt.|
|Phishing|Indikatoren für eine Phishing-Kampagne.|
|Proxy|Indikator ist der eines Proxy Diensts.|
|PUA|Potenziell unerwünschte Anwendung.|
|WatchList|Dies ist der generische Bucket, in dem Indikatoren aufgestellt werden, wenn nicht genau ermittelt werden kann, was die Bedrohung ist oder die eine manuelle Interpretation erfordert. Dies sollte in der Regel nicht von Partnern verwendet werden, die Daten in das System übermitteln.|

### <a name="tlplevel-values"></a>tlpLevel-Werte

Jeder Indikator muss bei der Übermittlung auch einen Wert für das Ampel Protokoll aufweisen. Dieser Wert stellt die Vertraulichkeit und den freigabebereich eines bestimmten Indikators dar.

| Werte | Beschreibung |
|:-------|:------------|
|Weiß| Freigabebereich: unLimited. Indikatoren können frei freigegeben werden, ohne Einschränkungen.|
|Green| Freigabebereich: Community. Indikatoren können für die Sicherheitscommunity freigegeben werden.|
|Bernstein| Freigabebereich: Limited. Dies ist die Standardeinstellung für Indikatoren und schränkt die Freigabe nur für Personen ein, die über einen "need-to-Know"-Dienst verfügen, und Dienst Operatoren, die Threat Intelligence 2-Kunden implementieren, deren System (e) ein Verhalten im Einklang mit dem Indikator aufweisen.|
|Red| Freigabebereich: persönlich. Diese Indikatoren sollen nur direkt und, vorzugsweise persönlich, freigegeben werden. In der Regel werden TLP-rote Indikatoren aufgrund der vordefinierten Einschränkungen nicht aufgenommen. Wenn TLP-rote Indikatoren übermittelt werden, sollte die "PassiveOnly"- `True` Eigenschaft auch auf festgelegt werden. |

## <a name="relationships"></a>Beziehungen

Keine.

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tiIndicator",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "action": "string",
  "activityGroupNames": ["String"],
  "additionalInformation": "String",
  "azureTenantId": "String",
  "confidence": 1024,
  "description": "String",
  "diamondModel": "string",
  "domainName": "String",
  "emailEncoding": "String",
  "emailLanguage": "String",
  "emailRecipient": "String",
  "emailSenderAddress": "String",
  "emailSenderName": "String",
  "emailSourceDomain": "String",
  "emailSourceIpAddress": "String",
  "emailSubject": "String",
  "emailXMailer": "String",
  "expirationDateTime": "String (timestamp)",
  "externalId": "String",
  "fileCompileDateTime": "String (timestamp)",
  "fileCreatedDateTime": "String (timestamp)",
  "fileHashType": "string",
  "fileHashValue": "String",
  "fileMutexName": "String",
  "fileName": "String",
  "filePacker": "String",
  "filePath": "String",
  "fileSize": 1024,
  "fileType": "String",
  "id": "String (identifier)",
  "ingestedDateTime": "String (timestamp)",
  "isActive": true,
  "killChain": ["String"],
  "knownFalsePositives": "String",
  "lastReportedDateTime": "String (timestamp)",
  "malwareFamilyNames": ["String"],
  "networkCidrBlock": "String",
  "networkDestinationAsn": 1024,
  "networkDestinationCidrBlock": "String",
  "networkDestinationIPv4": "String",
  "networkDestinationIPv6": "String",
  "networkDestinationPort": 1024,
  "networkIPv4": "String",
  "networkIPv6": "String",
  "networkPort": 1024,
  "networkProtocol": 1024,
  "networkSourceAsn": 1024,
  "networkSourceCidrBlock": "String",
  "networkSourceIPv4": "String",
  "networkSourceIPv6": "String",
  "networkSourcePort": 1024,
  "passiveOnly": true,
  "severity": 1024,
  "tags": ["String"],
  "targetProduct": "String",
  "threatType": "String",
  "tlpLevel": "string",
  "url": "String",
  "userAgent": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "tiIndicator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
