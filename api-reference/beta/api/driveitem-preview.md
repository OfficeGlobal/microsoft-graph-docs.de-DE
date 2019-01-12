---
title: 'DriveItem: Vorschau'
description: Diese Aktion können Sie kurzlebige eingebettet werden URLs für ein Element abrufen, um eine temporäre Vorschau zu rendern.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: be96a0cd451bb3f1c75c32f235d7669ce0bd7509
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980874"
---
# <a name="driveitem-preview"></a>DriveItem: Vorschau

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

Diese Aktion können Sie kurzlebige eingebettet werden URLs für ein Element abrufen, um eine temporäre Vorschau zu rendern.

Wenn Sie Links mit langer Lebensdauer eingebettet werden abrufen möchten, verwenden Sie stattdessen die [CreateLink][] API.

> **Hinweis:** Die **Preview** -Aktion ist derzeit nur auf SharePoint und OneDrive für Unternehmen verfügbar.

[createLink]: driveitem-createlink.md

## <a name="permissions"></a>Berechtigungen

Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).

| Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)
|:---------------------------------------|:-------------------------------------------
| Delegiert (Geschäfts-, Schul- oder Unikonto)     | Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All
| Delegiert (persönliches Microsoft-Konto) | Files.Read, Files.ReadWrite, Files.ReadWrite.All
| Anwendung                            | Nicht unterstützt

## <a name="http-request"></a>HTTP-Anforderung

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a>Anforderungstext

Der Text der Anforderung definiert Eigenschaften der embeddable URL Ihrer Anwendung anfordert.
Bei der Anforderung sollte es sich um ein JSON-Objekt mit folgenden Eigenschaften handeln:

|   Name      |  Typ         | Beschreibung
|:------------|:--------------|:-----------------------------------------------
| Viewer      | string        | Optional. Preview-app verwendet. `onedrive` oder `office`. Wenn der Wert null ist, wird ein passender Viewer automatisch ausgewählt.
| Chromeless  | Boolean       | Optional. Wenn `true` (Standard), die eingebettete Ansicht wird nicht schließen Sie alle Steuerelemente.
| allowEdit   | Boolean       | Optional. Wenn `true`, die Datei aus der eingebetteten Benutzeroberfläche bearbeitet werden kann.
| page        | Zeichenfolge/eine einzelne Nummer | Optional. Seitenzahl des Dokuments an, falls zutreffend zu starten. Als Zeichenfolge für die zukünftige Verwendung Fällen um Dateitypen wie ZIP angegeben.
| Zoom        | number        | Optional. Zoom-Wert auf, falls zutreffend.

## <a name="response"></a>Antwort

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

Die Antwort wird ein JSON-Objekt mit den folgenden Eigenschaften werden:

| Name           | Typ   | Beschreibung
|:---------------|:-------|:---------------------------------------------------
| getUrl         | string | URL für das Einbetten von mit HTTP-GET (Iframes usw.) geeignet
| postUrl        | string | URL für das Einbetten von mithilfe von HTTP POST geeignet (bilden, JS, usw..)
| postParameters | string | POST-Parameter einschließen, wenn PostUrl verwenden

GetUrl, PostUrl oder beide möglicherweise abhängig vom aktuellen Status des Embed-Unterstützung für den angegebenen Optionen zurückgegeben.

PostParameters ist eine Zeichenfolge, die als formatiert `application/x-www-form-urlencoded`, und wenn Ausführen von POST an den PostUrl Content-Type entsprechend festgelegt werden sollen. Beispiel:
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a>Leser von Berichten

Die folgenden Werte sind für den **Viewer** -Parameter zulässig.

| Typwert | Beschreibung
|:-----------|:----------------------------------------------------------------
| (null)     | Wählt eine entsprechende app für das Rendern der Datei. Hiermit wird in den meisten Fällen verwendet die `onedrive` Vorschau, aber nach dem Dateityp variieren.
| `onedrive` | Verwenden Sie die previewer OneDrive-app, um die Datei zu rendern.
| `office`   | Verwenden Sie die WAC (online für Office), um die Datei zu rendern. Nur gültig für Office-Dokumenten.

### <a name="chrome-vs-chromeless"></a>Chrome Vs chromeless

Wenn `chromeless` true ist, wird die Vorschau einer bare Rendering der Datei werden.
Anderenfalls möglicherweise zusätzliche Symbolleisten/Schaltflächen für die Interaktion mit der Dokument-Ansicht angezeigt.

### <a name="viewedit"></a>Anzeigen/Bearbeiten

Wenn `allowEdit` true ist, das Dokument durch Benutzerinteraktion mit eingebettete Vorschau geändert werden kann.
Diese Funktion möglicherweise nicht für alle apps Preview oder Dateitypen zur Verfügung.

### <a name="pagezoom"></a>Seite/zoom

Die `page` und `zoom` Optionen möglicherweise nicht für alle Preview apps verfügbar, jedoch wird angewendet werden soll, wenn die app Preview unterstützt.
