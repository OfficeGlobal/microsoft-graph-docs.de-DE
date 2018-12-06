---
title: Verwenden von Abfrageparametern zum Anpassen von Antworten
description: Microsoft Graph stellt optionale Abfrageparameter bereit, die Sie zum Festlegen und Steuern der in einer Antwort zurückgegebenen Datenmenge verwenden können. Die folgenden Abfrageparameter werden unterstützt.
ms.openlocfilehash: e41a6e8d9cc42506985bd82f00bcdc4efaec8add
ms.sourcegitcommit: 2532b8dd7f2533d956e2600855b3daeabdd9b8ff
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/30/2018
ms.locfileid: "27092347"
---
# <a name="use-query-parameters-to-customize-responses"></a>Verwenden von Abfrageparametern zum Anpassen von Antworten

Microsoft Graph stellt optionale Abfrageparameter bereit, die Sie zum Festlegen und Steuern der in einer Antwort zurückgegebenen Datenmenge verwenden können. Die folgenden Abfrageparameter werden unterstützt.

>**Hinweis:** Klicken Sie auf die Beispiele, um sie im [Graph-Tester][graph-explorer] auszuprobieren.

| Name                     | Beschreibung | Beispiel
|:-------------------------|:------------|:---------|
| [$count](#count-parameter)         | Dient zum Abrufen der Gesamtzahl übereinstimmender Ressourcen. | [`/me/messages?$top=2&$count=true`][count-example]
| [$expand](#expand-parameter)       | Dient zum Abrufen von verwandten Ressourcen.|[`/groups?$expand=members`][expand-example]
| [$filter](#filter-parameter)       | Dient zum Filtern von Ergebnissen (Zeilen).|[`/users?$filter=startswith(givenName,'J')`][filter-example]
| [$format](#format-parameter)       | Dient zum Zurückgeben der Ergebnisse im angegebenen Medienformat.|[`/users?$format=json`][format-example]
| [$orderby](#orderby-parameter)     | Dient zum Sortieren von Ergebnissen.|[`/users?$orderby=displayName desc`][orderby-example]
| [$search](#search-parameter)       | Dient zum Zurückgeben von Ergebnissen basierend auf Suchkriterien. Wird derzeit in **messages**- und **person**-Sammlungen unterstützt.|[`/me/messages?$search=pizza`][search-example]
| [$select](#select-parameter)       | Dient zum Filtern von Eigenschaften (Spalten).|[`/users?$select=givenName,surname`][select-example]
| [$skip](#skip-parameter)           | Dient zum Indizieren in einem Resultset. Wird auch von einigen APIs zum Implementieren von Paging verwendet und kann zusammen mit `$top` zum manuellen Auslagern von Ergebnissen verwendet werden. | [`/me/messages?$skip=11`][skip-example]
| [$skipToken](#skiptoken-parameter) | Dient zum Abrufen der nächsten Seite von Ergebnissen aus Resultsets, die mehrere Seiten umfassen. (Einige APIs verwenden stattdessen `$skip`.) | `/users?$skiptoken=X%274453707402000100000017...`|
| [$top](#top-parameter)             | Dient zum Festlegen der Seitengröße von Ergebnissen. |[`/users?$top=2`][top-example]



Diese Parameter sind mit der [OData V4-Abfragesprache][odata-query] kompatibel. Nicht alle Parameter werden über alle Microsoft Graph-APIs hinweg unterstützt, und die Unterstützung kann zwischen dem `v1.0`- und dem `beta`-Endpunkt erheblich abweichen. 

> **Hinweis: **Am `beta`- und `v1.0`-Endpunkt ist das `$`-Präfix optional. Sie können z. B. `filter` anstelle von `$filter` verwenden. 

## <a name="encoding-query-parameters"></a>Codieren von Abfrageparametern

Die Werte von Abfrageparametern sollten als Prozentwert codiert werden. Viele HTTP-Clients, Browser und Tools (z. B. der [Graph-Tester][graph-explorer]) sind Ihnen dabei behilflich. Wenn bei einer Abfrage ein Fehler auftritt, kann eine der möglichen Ursachen dafür sein, dass die Werte von Abfrageparametern nicht ordnungsgemäß codiert wurden.

Eine nicht codierte URL sieht folgendermaßen aus:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName, 'J')
```

Eine korrekt codierte URL sieht folgendermaßen aus:

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(givenName%2C+'J')
```

## <a name="count-parameter"></a>count-Parameter

Verwenden Sie `$count` als Abfrageparameter, um die Gesamtzahl der Elemente in einer Sammlung zusammen mit der Seite der Datenwerte anzugeben, die von Microsoft Graph zurückgegeben werden. 

Die folgende Anforderung gibt beispielsweise sowohl die **contact**-Sammlung des aktuellen Benutzers sowie die Anzahl von Elementen in der **contact**-Sammlung in der `@odata.count`-Eigenschaft zurück.

```http
GET  https://graph.microsoft.com/v1.0/me/contacts?$count=true
```

[Im Graph-Tester ausprobieren](https://developer.microsoft.com/graph/graph-explorer?request=me/contacts?$count=true&method=GET&version=v1.0)


>**Hinweis:** `$count` wird für Sammlungen von Ressourcen, die von [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) abgeleitet werden, wie Sammlungen von [Benutzern](/graph/api/resources/user?view=graph-rest-1.0) oder [Gruppen](/graph/api/resources/group?view=graph-rest-1.0), nicht unterstützt.

## <a name="expand-parameter"></a>expand-Parameter

Viele Microsoft Graph-Ressourcen machen sowohl deklarierte Eigenschaften der Ressource als auch deren Beziehungen zu anderen Ressourcen verfügbar. Diese Beziehungen werden auch als Verweiseigenschaften oder Navigationseigenschaften bezeichnet und können auf eine einzelne Ressource oder auf eine Sammlung von Ressourcen verweisen. Beispielsweise werden die E-Mail-Ordner, die Vorgesetzten und die direkten Mitarbeiter eines Benutzers alle als Beziehungen verfügbar gemacht. 

Normalerweise können Sie die Eigenschaften einer Ressource oder eine ihrer Beziehungen in einer einzelnen Anforderung abfragen, aber nicht beides gleichzeitig. Sie können den `$expand`-Zeichenfolgen-Abfrageparameter verwenden, um die erweiterte Ressource oder die Sammlung, auf die von einer einzigen Beziehung verwiesen wird (Navigationseigenschaft) in Ihre Ergebnisse einzuschließen.

Im folgenden Beispiel werden Informationen des Stammlaufwerks zusammen mit den untergeordneten Elementen der obersten Ebene in einem Laufwerk abgerufen:

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children
```

[Im Graph-Tester ausprobieren](https://developer.microsoft.com/graph/graph-explorer?request=me/drive/root?$expand=children&method=GET&version=v1.0)

Bei einigen Ressourcensammlungen können Sie auch die Eigenschaften angeben, die in den erweiterten Ressourcen zurückgegeben werden sollen, indem Sie einen `$select`-Parameter hinzufügen. Im folgenden Beispiel wird die gleiche Abfrage wie im vorherigen Beispiel ausgeführt, hier wird jedoch eine [`$select`](#select-parameter)-Anweisung verwendet, um die für die erweiterten untergeordneten Elemente zurückgegebenen Eigenschaften auf die **id**- und **name**-Eigenschaften einzuschränken.

```http
GET https://graph.microsoft.com/v1.0/me/drive/root?$expand=children($select=id,name)
```

[Ausprobieren im Graph-Tester][expand-example]

> **Hinweis:** Nicht alle Beziehungen und Ressourcen unterstützen den `$expand`-Abfrageparameter. Sie können z. B. die Beziehungen **directReports**, **manager** und **memberOf** für einen Benutzer erweitern, aber Sie können nicht seine Beziehungen **events**, **messages** oder **photo** erweitern. Nicht alle Ressourcen oder Beziehungen unterstützen die Verwendung von `$select` in erweiterten Elementen. 
> 
> Bei Azure AD-Ressourcen, die von [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) abgeleitet werden, z. B. [Benutzer](/graph/api/resources/user?view=graph-rest-1.0) und [Gruppe](/graph/api/resources/group?view=graph-rest-1.0), wird `$expand` nur für `beta` unterstützt, und es werden maximal 20 Elemente für die erweiterte Beziehung zurückgegeben.

## <a name="filter-parameter"></a>filter-Parameter

Verwenden Sie den `$filter`-Abfrageparameter, um nur eine Teilmenge einer Sammlung abzurufen. 

Um beispielsweise Benutzer zu suchen, deren Anzeigename mit dem Buchstaben „J“ beginnt, verwenden Sie `startswith`.

```http
GET https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'J')
```

[Ausprobieren im Graph-Tester][filter-example]

Die Unterstützung für `$filter`-Operatoren variiert je nach Microsoft Graph-API. Im Allgemeinen werden die folgenden logischen Operatoren unterstützt: 

- gleich (`eq`)
- ungleich (`ne`)
- größer als (`gt`)
- größer als oder gleich (`ge`)
- kleiner als (`lt`), kleiner als oder gleich (`le`)
- und (`and`)
- oder (`or`)
- nicht (`not`)
 
Der Zeichenfolgenoperator `startswith` wird häufig unterstützt. Der Lambda-Operator `any` wird für einige APIs unterstützt. In der folgenden Tabelle finden Sie einige Verwendungsbeispiele. Weitere Informationen zur `$filter`-Syntax finden Sie im [OData-Protokoll][odata-filter].  

Die folgende Tabelle enthält einige Beispiele zur Verwendung des `$filter`-Abfrageparameters.

> **Hinweis:** Klicken Sie auf die Beispiele, um sie im [Graph-Tester][graph-explorer] auszuprobieren.

| Beschreibung | Beispiel
|:------------|:--------|
| In mehreren Eigenschaften nach Benutzern mit dem Namen „Mary“ suchen | [`https://graph.microsoft.com/v1.0/users?$filter=startswith(displayName,'mary') or startswith(givenName,'mary') or startswith(surname,'mary') or startswith(mail,'mary') or startswith(userPrincipalName,'mary')`](https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(displayName,'mary')+or+startswith(givenName,'mary')+or+startswith(surname,'mary')+or+startswith(mail,'mary')+or+startswith(userPrincipalName,'mary')&method=GET&version=v1.0) 
| Alle Ereignisse des angemeldeten Benutzers abrufen, die nach dem 01.07.2017 beginnen | [`https://graph.microsoft.com/v1.0/me/events?$filter=start/dateTime ge '2017-07-01T08:00'`](https://developer.microsoft.com/graph/graph-explorer?request=me/events?$filter=start/dateTime+ge+'2017-07-01T08:00'&method=GET&version=v1.0) 
| Alle E-Mails von einer bestimmten Adresse abrufen, die der angemeldete Benutzer erhalten hat | [`https://graph.microsoft.com/v1.0/me/messages?$filter=from/emailAddress/address eq 'someuser@example.com'`](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=from/emailAddress/address+eq+'someuser@.com'&method=GET&version=v1.0) 
| Alle E-Mails abrufen, die der angemeldete Benutzer im April 2017 erhalten hat | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=ReceivedDateTime ge 2017-04-01 and receivedDateTime lt 2017-05-01`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=ReceivedDateTime+ge+2017-04-01+and+receivedDateTime+lt+2017-05-01&method=GET&version=v1.0) 
| Alle ungelesenen E-Mails im Postfach des angemeldeten Benutzers abrufen | [`https://graph.microsoft.com/v1.0/me/mailFolders/inbox/messages?$filter=isRead eq false`](https://developer.microsoft.com/graph/graph-explorer?request=me/mailFolders/inbox/messages?$filter=isRead+eq+false&method=GET&version=v1.0) 
| Alle Office 365-Gruppen in einer Organisation auflisten | [`https://graph.microsoft.com/v1.0/groups?$filter=groupTypes/any(c:c+eq+'Unified')`](https://developer.microsoft.com/graph/graph-explorer?request=groups?$filter=groupTypes/any(c:c+eq+'Unified')&method=GET&version=v1.0) 

> **Hinweis:** Die folgenden `$filter`-Operatoren werden für Azure AD-Ressourcen nicht unterstützt: `ne`, `gt`, `ge`, `lt`, `le` und `not`. Der `contains`-Zeichenfolgenoperator wird derzeit nicht für Microsoft Graph-Ressourcen unterstützt.

## <a name="format-parameter"></a>format-Parameter

Verwenden Sie zum Festlegen des Medienformats der von Microsoft Graph zurückgegebenen Elemente den `$format`-Abfrageparameter.

Die folgende Anforderung gibt beispielsweise die Benutzer in der Organisation im JSON-Format zurück:

```http
GET https://graph.microsoft.com/v1.0/users?$format=json
```

[Ausprobieren im Graph-Tester][format-example]

> **Hinweis:** Der `$format`-Abfrageparameter unterstützt eine Reihe von Formaten (z. B. Atom, XML und JSON), die Ergebnisse werden aber möglicherweise nicht in allen Formaten zurückgegeben.

## <a name="orderby-parameter"></a>orderby-Parameter

Verwenden Sie zum Festlegen der Sortierreihenfolge der von Microsoft Graph zurückgegebenen Elemente den `$orderby`-Abfrageparameter.

Die folgende Anforderung gibt beispielsweise die Benutzer in der Organisation sortiert nach ihrem Anzeigenamen zurück:

```http
GET https://graph.microsoft.com/v1.0/users?$orderby=displayName
```
[Ausprobieren im Graph-Tester][orderby-example]

Sie können auch nach komplexen Typentitäten sortieren. In der folgenden Anforderung werden Nachrichten abgerufen und nach dem **Adresse**-Feld der **from**-Eigenschaft sortiert, die vom komplexen Typ **emailAddress** ist:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$orderby=from/emailAddress/address
```
[Im Graph-Tester ausprobieren](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/address&method=GET&version=v1.0)

Wenn Sie die Ergebnisse in aufsteigender oder absteigender Reihenfolge sortieren möchten, fügen Sie entweder `asc` oder `desc` getrennt durch ein Leerzeichen an den Namen des Felds an, z. B. `?$orderby=name%20desc`.

Bei einigen APIs können Sie die Ergebnisse anhand mehrerer Eigenschaften sortieren. Die folgende Anforderung sortiert die Nachrichten im Posteingang des Benutzers beispielsweise zuerst nach dem Namen der Person, die die Nachricht gesendet hat, in absteigender Reihenfolge (von Z nach A) und anschließend nach dem Betreff in aufsteigender Reihenfolge (Standard).

```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/Inbox/messages?$orderby=from/emailAddress/name desc,subject
```

[Im Graph-Tester ausprobieren](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$orderby=from/emailAddress/name%20desc,subject&method=GET&version=v1.0)

Wenn Sie $filter angeben, leitet der Server eine Sortierreihenfolge für die Ergebnisse ab. Wenn Sie sowohl `$orderby` als auch `$filter` verwenden, müssen die Eigenschaften in der `$filter` zuerst in der `$orderby` vor allen anderen Eigenschaften aufgeführt werden, und sie müssen in der Reihenfolge aufgeführt werden, in der sie im Parameter `$filter` angezeigt werden, da der Server immer eine Sortierreihenfolge für die Ergebnisse eines `$filter` ableitet. 

Das folgende Beispiel zeigt eine Abfrage, die nach den Eigenschaften **subject** und **importance** gefiltert ist und dann nach den Eigenschaften **subject**, **importance** und **receivedDateTime** in absteigender Reihenfolge sortiert werden.

```http
GET https://graph.microsoft.com/v1.0/me/messages?$filter=Subject eq 'welcome' and importance eq 'normal'&$orderby=subject,importance,receivedDateTime desc
```

[Ausprobieren im Graph-Tester](https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$filter=subject%20eq%20%27welcome%27%20and%20importance%20eq%20%27normal%27%20&$orderby=subject,importance,receivedDateTime%20desc&method=GET&version=v1.0)

 > **Hinweis:** Bei Azure AD-Ressourcen, die von [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) abgeleitet werden, wie z. B. [Benutzer](/graph/api/resources/user?view=graph-rest-1.0) und [Gruppe](/graph/api/resources/group?view=graph-rest-1.0), kann `$orderby` nicht mit `$filter`-Ausdrücken verwendet werden. 

## <a name="search-parameter"></a>search-Parameter

Um die Ergebnisse einer Anforderung so zu beschränken, dass sie einem Suchkriterium entsprechen, verwenden Sie den `$search`-Abfrageparameter.

> **Hinweis:** Sie können derzeit **nur** [Nachrichten](/graph/api/resources/message?view=graph-rest-1.0)- und [Personen](/graph/api/resources/person?view=graph-rest-1.0)-Sammlungen suchen. Eine `$search`-Anforderung gibt bis zu 250 Ergebnisse zurück. Sie können [`$filter`](#filter-parameter) oder [`$orderby`](#orderby-parameter) nicht in einer Suchabfrage verwenden.

### <a name="using-search-on-message-collections"></a>Verwenden von $search in Nachrichtensammlungen

Sie können nach Nachrichten auf Grundlage eines Werts in einer bestimmten Eigenschaften suchen. Die Suchergebnisse sind nach Datum und Uhrzeit sortiert, zu dem bzw. der die Nachricht gesendet wurde.

Wenn Sie eine Suche nach Nachrichten durchführen und nur einen Wert ohne bestimmte Nachrichteneigenschaften angeben, wird die Suche anhand der Standardsucheigenschaften**from**, **subject** und **body** ausgeführt.

Im folgenden Beispiel werden alle Nachrichten im Posteingang des angemeldeten Benutzers zurückgegeben, die das Wort „Pizza“ in einer der drei Standardsucheigenschaften enthalten:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$search="pizza"
```

[Ausprobieren im Graph-Tester][search-example]

Alternativ können Sie eine Suche nach Nachrichten durchführen, indem Sie die Nachrichteneigenschaftennamen in der folgenden Tabelle angeben, die durch die KQL-Syntax erkannt werden. Diese Eigenschaftennamen entsprechen den in der **message**-Entität von Microsoft Graph definierten Eigenschaften. Outlook und andere Office 365-Anwendungen wie SharePoint unterstützen die KQL-Syntax und bieten den Komfort einer gemeinsamen Discovery-Domäne für ihre Datenspeicher.


| Durchsuchbare E-Mail-Eigenschaft                | Beschreibung | Beispiel 
|:-------------------------|:------------|:---------|
| **Anlage**           | Die Namen der an eine E-Mail angefügten Dateien.|[`me/messages?$search="attachment:api-catalog.md"`][search-att-example]
| **bcc**           | Das **bcc**-Feld einer E-Mail-Nachricht, das als SMTP-Adresse, Anzeigename oder Alias angegeben ist.|[`me/messages?$search="bcc:samanthab@contoso.com"&$select=subject,bccRecipients`][search-bcc-example]
| **Text**           | Text einer E-Mail.|[`me/messages?$search="body:excitement"`][search-body-example]
| **cc**           | Das **cc**-Feld einer E-Mail-Nachricht, das als SMTP-Adresse, Anzeigename oder Alias angegeben ist.|[`me/messages?$search="cc:danas"&$select=subject,ccRecipients`][search-cc-example]
| **Von**           | Der Absender einer E-Mail-Nachricht, der als SMTP-Adresse, Anzeigename oder Alias angegeben ist.|[`me/messages?$search="from:randiw"&$select=subject,from`][search-from-example]
| **hasAttachment** | „True“, wenn eine E-Mail eine Anlage enthält, die keine Inlineanlage ist, andernfalls „false“. |[`me/messages?$search="hasAttachments=true"`][search-from-example]
| **Wichtigkeit**           | Die Wichtigkeit einer E-Mail-Nachricht, die ein Absender festlegen kann, wenn er eine Nachricht sendet. Die möglichen Werte sind `low`, `medium` oder `high`.|[`me/messages?$search="importance:high"&$select=subject,importance`][search-imp-example]
| **Art**           | Der Typ der Nachricht. Die möglichen Werte sind `contacts`, `docs`, `email`, `faxes`, `im`, `journals`, `meetings`, `notes`, `posts`, `rssfeeds`, `tasks` oder `voicemail`.|[`me/messages?$search="kind:voicemail"`][search-kind-example]
| **Teilnehmer**           | Die **von**-, **an**-, **cc**- und **bcc**-Felder einer E-Mail-Nachricht, die als SMTP-Adressen, Anzeigenamen oder Aliase angegeben sind.|[`me/messages?$search="participants:danas"`][search-part-example]
| **Empfangen**           | Das Datum, an dem eine E-Mail-Nachricht von einem Empfänger empfangen wurde.|[`me/messages?$search="received:07/23/2018"&$select=subject,receivedDateTime`][search-rcvd-example]
| **recipients**           | Die **an**-, **cc**- und **bcc**-Felder einer E-Mail-Nachricht, die als SMTP-Adressen, Anzeigenamen oder Aliase angegeben sind.|[`me/messages?$search="recipients:randiq"&$select=subject,toRecipients,ccRecipients,bccRecipients`][search-rcpts-example]
| **Gesendet**           | Das Datum, an dem eine E-Mail vom Absender gesendet wurde.|[`me/messages?$search="sent:07/23/2018"&$select=subject,sentDateTime`][search-sent-example]
| **size**           | Die Größe eines Elements in Byte.|[`me/messages?$search="size:1..500000"`][search-size-example]
| **Betreff**           | Der Text in der Betreffzeile einer E-Mail. .|[`me/messages?$search="subject:has"&$select=subject`][search-sbj-example]
| **An**           | Das **An**-Feld einer E-Mail-Nachricht, das als SMTP-Adresse, Anzeigename oder Alias angegeben ist.|[`me/messages?$search="to:randiw"&$select=subject,toRecipients`][search-to-example]


Weitere Informationen zu durchsuchbaren E-Mail-Eigenschaften, zu KQL-Syntax, unterstützten Operatoren und Tipps für die Suche finden Sie in den folgenden Artikeln:

- [Durchsuchbar Eigenschaften in Exchange](https://docs.microsoft.com/de-DE/Exchange/policy-and-compliance/ediscovery/message-properties-and-search-operators#searchable-properties-in-exchange)

- [Syntaxreferenz für die Keyword Query Language (KQL)](https://docs.microsoft.com/de-DE/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)

- 
  [Nachrichteneigenschaften und Suchoperatoren für In-Situ-eDiscovery in Exchange 2016](https://technet.microsoft.com/en-us/library/dn774955(v=exchg.160).aspx)

### <a name="using-search-on-person-collections"></a>Verwenden von $search in Personensammlungen

Sie können die Personen-API von Microsoft Graph verwenden, um Personen abzurufen, die für einen Benutzer am relevantesten sind. Relevanz wird durch die Kommunikations- und Zusammenarbeitsmuster und Geschäftsbeziehungen des Benutzers bestimmt. Die Personen-API unterstützt den `$search`-Abfrageparameter.

Personensuchen werden sowohl für die Eigenschaft **displayName** als auch für die Eigenschaft **emailAddress** der Ressource vom Typ [person](/graph/api/resources/person?view=graph-rest-1.0) ausgeführt.

Die folgende Anforderung führt eine Suche nach einer Person mit dem Namen „Irene McGowen“ in den Eigenschaften **displayName** und **emailAddress** für jede Person in der Sammlung **people** des angemeldeten Benutzers durch. Da eine Person mit dem Namen „Irene McGowan“ für den angemeldeten Benutzer relevant ist, werden die Informationen für „Irene McGowan“ zurückgegeben.

```http
GET https://graph.microsoft.com/v1.0/me/people/?$search="Irene McGowen"
```

Das folgende Beispiel zeigt die Antwort. 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
       {
           "id": "C0BD1BA1-A84E-4796-9C65-F8A0293741D1",
           "displayName": "Irene McGowan",
           "givenName": "Irene",
           "surname": "McGowan",
           "birthday": "",
           "personNotes": "",
           "isFavorite": false,
           "jobTitle": "Auditor",
           "companyName": null,
           "yomiCompany": "",
           "department": "Finance",
           "officeLocation": "12/1110",
           "profession": "",
           "userPrincipalName": "irenem@contoso.onmicrosoft.com",
           "imAddress": "sip:irenem@contoso.onmicrosoft.com",
           "scoredEmailAddresses": [
               {
                   "address": "irenem@contoso.onmicrosoft.com",
                   "relevanceScore": -16.446060612802224
               }
           ],
           "phones": [
               {
                   "type": "Business",
                   "number": "+1 412 555 0109"
               }
           ],
           "postalAddresses": [],
           "websites": [],
           "personType": {
               "class": "Person",
               "subclass": "OrganizationUser"
           }
       }
   ]
}
```

Weitere Informationen zur Personen-API finden Sie unter [Abrufen von Informationen über die entsprechenden Personen](./people-example.md#search-people).  

## <a name="select-parameter"></a>select-Parameter

Verwenden Sie den `$select`-Abfrageparameter, um eine Reihe von Eigenschaften zurückzugeben, die sich von den Standardeigenschaften für eine einzelne Ressource oder eine Sammlung von Ressourcen unterscheidet. Mit $select können Sie eine Teilmenge oder eine Obermenge der Standardeigenschaften angeben.

Wenn Sie z. B. die Nachrichten des angemeldeten Benutzers abrufen, können Sie angeben, dass nur die Eigenschaften **from** und **subject** zurückgegeben werden:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$select=from,subject
```

[Ausprobieren im Graph-Tester][select-example]

> **Wichtig:** Im Allgemeinen wird empfohlen, dass Sie `$select` verwenden, um die von einer Abfrage zurückgegebenen Eigenschaften auf diejenigen zu beschränken, die von Ihrer App benötigt werden. Dies gilt insbesondere für Abfragen, die möglicherweise ein großes Resultset zurückgeben. Durch Beschränken der in den einzelnen Zeilen zurückgegebenen Eigenschaften werden die Netzwerklast reduziert und die Leistung Ihrer App verbessert.
>
> In `v1.0` geben einige Azure AD-Ressourcen, die von [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0) abgeleitet werden, z.B. [Benutzer](/graph/api/resources/user?view=graph-rest-1.0) und [Gruppe](/graph/api/resources/group?view=graph-rest-1.0) eine begrenzte, standardmäßige Untermenge von Eigenschaften für Lesevorgänge zurück. Für diese Ressourcen müssen Sie `$select` verwenden, um Eigenschaften außerhalb des Standardsatzes zurückzugeben.  

## <a name="skip-parameter"></a>skip-Parameter

Verwenden Sie den `$skip`-Abfrageparameter zum Festlegen der Anzahl der Elemente, die am Anfang einer Sammlung übersprungen werden sollen. Die folgende Anforderung gibt beispielsweise Ereignisse für den Benutzer sortiert nach Erstellungsdatum zurück, beginnend mit dem 21. Ereignis in der Sammlung:

```http
GET  https://graph.microsoft.com/v1.0/me/events?$orderby=createdDateTime&$skip=20
```
[Ausprobieren im Graph-Tester][skip-example]

> **Hinweis:** Einige Microsoft Graph-APIs, z. B. Outlook-Mail und Outlook-Kalender (**Nachricht**, **Ereignis** und **Kalender**), verwenden `$skip` zur Implementierung von Paging. Wenn Ergebnisse einer Abfrage mehrere Seiten umfassen, geben diese APIs eine `@odata:nextLink`-Eigenschaft mit einer URL zurück, die einen `$skip`-Parameter enthält. Sie können diese URL verwenden, um die nächste Seite mit Ergebnissen zurückzugeben. Weitere Informationen finden Sie unter [Paging](./paging.md).

## <a name="skiptoken-parameter"></a>skipToken-Parameter

Einige Abfragen geben mehrere Seiten von Daten zurück, entweder aufgrund von serverseitigem Paging oder aufgrund der Verwendung des [`$top`](#top-parameter)-Parameters, um die Seitengröße der Antwort zu begrenzen. Viele Microsoft Graph-APIs verwenden den `skipToken`-Abfrageparameter, um auf nachfolgende Seiten des Ergebnisses zu verweisen. Der `$skiptoken`-Parameter enthält ein undurchsichtiges Token, das auf die nächste Seite von Ergebnissen verweist und in der URL zurückgegeben wird, die in der `@odata.nextLink`-Eigenschaft in der Antwort bereitgestellt wird. Weitere Informationen finden Sie unter [Paging](./paging.md).


## <a name="top-parameter"></a>top-Parameter

Verwenden Sie den `$top`-Abfrageparameter, um die Seitengröße des Resultsets anzugeben. 

Wenn mehr Elemente im Resultset verbleiben, enthält der Antworttext einen `@odata.nextLink`-Parameter. Dieser Parameter enthält eine URL, die Sie verwenden können, um die nächste Seite mit Ergebnissen abzurufen. Weitere Informationen finden Sie unter [Paging](./paging.md). 

Die folgende Anforderung gibt beispielsweise die ersten fünf Nachrichten im Postfach des Benutzers zurück:

```http
GET https://graph.microsoft.com/v1.0/me/messages?$top=5
```

[Ausprobieren im Graph-Tester][top-example]


## <a name="error-handling-for-query-parameters"></a>Fehlerbehandlung für Abfrageparameter

Einige Anforderungen geben eine Fehlermeldung zurück, wenn ein angegebener Abfrageparameter nicht unterstützt wird. `$expand` kann zum Beispiel nicht in der `user/photo`-Beziehung verwendet werden. 

```http
https://graph.microsoft.com/beta/me?$expand=photo
```

```json
{
    "error":{
        "code":"ExpandNotSupported",
        "message":"Expand is not allowed for property 'Photo' according to the entity schema.",
        "innerError":{
            "request-id":"1653fefd-bc31-484b-bb10-8dc33cb853ec",
            "date":"2017-07-31T20:55:01"
        }
    }
}
```

Beachten Sie jedoch, dass Abfrageparameter, die in einer Anforderung angegeben sind, im Hintergrund einen Fehler verursachen können. Dies gilt für nicht unterstützte Abfrageparameter sowie für nicht unterstützte Kombinationen von Abfrageparametern. In diesen Fällen sollten Sie die von der Anforderung zurückgegebenen Daten überprüfen, um zu ermitteln, ob die angegebenen Abfrageparameter den gewünschten Effekt erzielt haben. 

[graph-explorer]: https://developer.microsoft.com/graph/graph-explorer
[odata-filter]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752358
[odata-query]: https://docs.oasis-open.org/odata/odata/v4.0/errata03/os/complete/part2-url-conventions/odata-v4.0-errata03-os-part2-url-conventions-complete.html#_Toc453752356
[count-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$top=2%26$count=true&method=GET&version=v1.0
[expand-example]: https://developer.microsoft.com/graph/graph-explorer?request=groups?$expand=members&method=GET&version=v1.0
[filter-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$filter=startswith(givenName,'J')&method=GET&version=v1.0
[format-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$format=json&method=GET&version=v1.0
[orderby-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$orderby=displayName%20DESC&method=GET&version=v1.0
[search-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=pizza&method=GET&version=v1.0
[select-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$select=givenName,surname&method=GET&version=v1.0
[skip-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$skip=11&method=GET&version=v1.0
[top-example]: https://developer.microsoft.com/graph/graph-explorer?request=users?$top=2&method=GET&version=v1.0

[search-att-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22attachment%3Aapi-catalog%2Emd%22&method=GET&version=v1.0
[search-bcc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22bcc%3Asamanthab%40contoso%2Ecom%22%26$select=subject,bccRecipients&method=GET&version=v1.0
[search-body-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22body%3Aexcitement%22&method=GET&version=v1.0
[search-cc-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22cc%3Adanas%22%26$select=subject,ccRecipients&method=GET&version=v1.0
[search-from-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22from%3Arandiw%22%26$select=subject,from&method=GET&version=v1.0
[search-hasatt-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22hasAttachments=true%22&method=GET&version=v1.0
[search-imp-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22importance%3Ahigh%22%26$select=subject,importance&method=GET&version=v1.0
[search-kind-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22kind%3Avoicemail%22&method=GET&version=v1.0
[search-part-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22participants%3Adanas%22&method=GET&version=v1.0

[search-rcvd-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22received%3A07/23/2018%22%26$select=subject,receivedDateTime&method=GET&version=v1.0

[search-rcpts-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22recipients%3Arandiw%22%26$select=subject,toRecipients,ccRecipients,bccRecipients&method=GET&version=v1.0
[search-sent-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22sent%3A07/23/2018%22%26$select=subject,sentDateTime&method=GET&version=v1.0
[search-size-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22size%3A1%2E%2E500000%22&method=GET&version=v1.0

[search-sbj-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22subject%3Ahas%22%26$select=subject&method=GET&version=v1.
[search-to-example]: https://developer.microsoft.com/graph/graph-explorer?request=me/messages?$search=%22to%3Arandiw%22%26$select=subject,toRecipients&method=GET&version=v1.0

