---
title: Ressourcentyp accessReview
description: 'In Azure AD Access Feature, überprüft die `accessReview` eine Überprüfung Access darstellt.  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e9099b1ec55a8ed017f77757d527abbd7e45bdf6
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016737"
---
# <a name="accessreview-resource-type"></a>Ressourcentyp accessReview

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

In Azure AD [Access überprüft](accessreviews-root.md) Feature der `accessReview` eine Access-Überprüfung darstellt.  


## <a name="methods"></a>Methoden

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Abrufen von accessReview](../api/accessreview-get.md) |   [accessReview](accessreview.md) |   Rufen Sie eine Access-Überprüfung mit einer bestimmten Id ab. |
|[Erstellen von accessReview](../api/accessreview-create.md) | [accessReview](accessreview.md) |   Erstellen Sie eine neue AccessReview. |
|[AccessReview löschen](../api/accessreview-delete.md) | Keine.   | Löschen einer AccessReview. |
|[AccessReview aktualisieren](../api/accessreview-update.md) | [accessReview](accessreview.md) | Aktualisieren einer AccessReview. |
|[Liste AccessReview Bearbeiter](../api/accessreview-listreviewers.md) |      [Benutzeridentität](useridentity.md) -Auflistung| Rufen Sie die Bearbeiter ein AccessReview. |
|[AccessReview Bearbeiter hinzufügen](../api/accessreview-addreviewer.md) |      Keine.   |   Fügen Sie einem Bearbeiter ein AccessReview hinzu. |
|[AccessReview Reviewer entfernen](../api/accessreview-removereviewer.md) | Keine.  |   Entfernen Sie einen Prüfer aus einer AccessReview. |
|[Liste AccessReview Entscheidungen](../api/accessreview-listdecisions.md) |      [AccessReviewDecision](accessreviewdecision.md) -Auflistung| Rufen Sie die Entscheidungen des ein AccessReview.|
|[Meine AccessReview Entscheidungen auflisten](../api/accessreview-listmydecisions.md) |     [AccessReviewDecision](accessreviewdecision.md) -Auflistung| Rufen Sie als "Leser" Mein Entscheidungen von einer AccessReview.|
|[AccessReview Erinnerung senden](../api/accessreview-sendreminder.md) |        Keine.   |   Senden Sie eine Erinnerung an die Bearbeiter ein AccessReview. |
|[AccessReview beenden](../api/accessreview-stop.md) |     Keine.   |   Beenden einer AccessReview. |
|[AccessReview Entscheidungen zurücksetzen](../api/accessreview-reset.md) |     Keine.   |   Setzen Sie die Entscheidungen in einer laufenden AccessReview zurück.|
|[Anwenden von AccessReview Entscheidungen](../api/accessreview-apply.md) |     Keine.   |   Gelten Sie die Entscheidungen aus einer abgeschlossenen AccessReview.|

## <a name="permissions"></a>Berechtigungen

|Berechtigungstyp                        | Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegiert (Geschäfts-, Schul- oder Unikonto)     | AccessReview.Read.All AccessReview.ReadWrite.All |
|Delegiert (persönliches Microsoft-Konto) | Nicht unterstützt |
|Anwendung                            | Nicht unterstützt |


## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| `id`                      |`String`                                                        | Das Feature zugewiesen Eindeutiger Bezeichner der einer Access-Überprüfung. |
| `displayName`             |`String`                                                        | Der Name des Access überprüfen. Erforderliche auf erstellen. |
| `startDateTime`           |`DateTimeOffset`                                                | Den DateTime-Wert, wenn die Überprüfung geplant ist, gestartet werden.  Dabei kann es sich um ein Datum in der Zukunft handeln.  Erforderliche auf erstellen. |
| `endDateTime`             |`DateTimeOffset`                                                | Den DateTime-Wert, wenn die Überprüfung geplant ist, um zu beenden. Dies muss mindestens einen Tag später als das Startdatum sein.  Erforderliche auf erstellen. |
| `status`                  |`String`                                                        | Dieses schreibgeschützte Feld gibt den Status eines AccessReview an. Die normale Statusarten `Initializing`, `NotStarted`, `Starting`,`InProgress`, `Completing`, `Completed`, `AutoReviewing`, und `AutoReviewed`. |
| `description`             |`String`                                                        | Die Beschreibung, die vom Ersteller überprüfen Access so, dass der Bearbeiter bereitgestellt. |
| `businessFlowTemplateId`  |`String`                                                        | Der Bezeichner der Business-Fluss-Vorlage. Erforderliche auf erstellen. |
| `reviewerType`            |`String`                                                        | Die Beziehungstyp des Reviewer auf das Zielobjekt, eine der `self`, `delegated` oder `entityOwners`. Erforderliche auf erstellen. | 
| `createdBy`               |[Benutzeridentität](useridentity.md)                                 | Der Benutzer, die diese Überprüfung erstellt hat. |
| `reviewedEntity`          |`microsoft.graph.identity`                                      | Das Objekt für das das Access überprüft überprüft die zugewiesenen Zugriffsrechte. Dies kann die Gruppe für die Überprüfung von Mitgliedschaften von Benutzern in einer Gruppe oder der app für eine Überprüfung der Zuordnungen von Benutzern zu einer Anwendung sein. Erforderliche auf erstellen. | 
| `settings`                |`microsoft.graph.accessReviewSettings`             | Die Einstellungen für ein AccessReview finden Sie unter Typdefinition unten. |



## <a name="relationships"></a>Beziehungen




| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
| `reviewers`               |[Benutzeridentität](useridentity.md) -Auflistung                     | Die Auflistung der Bearbeiter für eine Access-Überprüfung, Access überprüfen ReviewerType ist vom Typ `delegate`. |
| `decisions`               |[AccessReviewDecision](accessreviewdecision.md) -Auflistung | Die Auflistung von Entscheidungen für diese Überprüfung Zugriff. |
| `myDecisions`             |[AccessReviewDecision](accessreviewdecision.md) -Auflistung | Die Auflistung von Entscheidungen für den Anrufer, wenn der Aufrufer Bearbeiter ist. |
| `instances`               |[AccessReview](accessreview.md) -Auflistung         | Die Auflistung von Bewertungen für Access-Instanzen Vergangenheit, Gegenwart und Zukunft, wenn dieses Objekt eine periodische Access Überprüfung ist. |

Ob diese Beziehungen auf ein Objekt vorhanden sind, hängt davon ab, gibt an, ob das Objekt eine Überprüfung einmaligen Zugriff auf einer Reihe von sich wiederholenden Access Wiederholung oder eine Instanz einer wiederkehrenden Access Überprüfung ist.

| Szenario | Hat Bearbeiter? | Hat Entscheidungen und MyDecisions? | Hat Instanzen? |
|:---------|:---------------|:---------------|:---------------|
|Einmalige Access überprüfen|Ja | Ja, gestartet | Nein |
| Überprüfen von sich wiederholenden Zugriff | Ja | Nein | Ja |
| Instanz von sich wiederholenden Access Wiederholung | Ja | Ja, gestartet | Nein |

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReview"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "description": "string",
 "businessFlowTemplateId": "string (identifier)",
 "reviewerType": "string",
 "createdBy": "microsoft.graph.userIdentity",
 "reviewedEntity": "microsoft.graph.identity",
 "settings": "microsoft.graph.accessReviewSettings",
 "reviewers": "Collection(microsoft.graph.userIdentity)"
}

```

## <a name="the-accessreviewsettings-type"></a>Geben Sie die accessReviewSettings

Die `accessReviewSettings` bietet zusätzliche Einstellungen beim Erstellen einer Access-Überprüfung, um das Feature Verhalten zu steuern, wenn eine Access-Überprüfung starten.  Dieser Typ hat die folgenden Eigenschaften: 

| Eigenschaft                     | Typ                      | Beschreibung |
| :--------------------------- | :------------------------ | :---------- |
| `mailNotificationsEnabled`|`Boolean`                | Flag, das angibt, ob das Senden von e-Mails an Prüfer und den Ersteller überprüfen aktiviert ist.                |
| `remindersEnabled`|`Boolean`       | Flag, das angibt, ob die sendende Reminder-e-Mails an Bearbeiter aktiviert sind.       |
| `justificationRequiredOnApproval`|`Boolean` | Flag, das angibt, ob Bearbeiter eine Begründung bereitstellen, beim Überprüfen von Access erforderlich sind.|
| `activityDurationInDays`|`Int64` | Die Anzahl der Tage, die die Benutzeraktivitäten für Bearbeiter angezeigt. |
| `autoReviewEnabled`|`Boolean` | Kennzeichnung, die angibt, ob das Feature für eine Entscheidung festgelegt werden soll, wenn der Prüfer eine für die Verwendung mit Auto-apply, nicht angegeben haben, ist aktiviert. |
| `autoReviewSettings`|`microsoft.graph.autoReviewSettings` | Detaillierte Einstellungen für das Feature für die Überprüfung Entscheidung, für die Verwendung mit Auto-apply, die weiter unten beschriebenen festzulegen, wie sollten. |
| `recurrenceSettings`|`microsoft.graph.accessReviewRecurrenceSettings` | Detaillierte Einstellungen für die Serie, die weiter unten beschriebenen. |
| `autoApplyReviewResultsEnabled`|`Boolean` | Kennzeichnung, die angibt, ob gelten Auto-Funktion, so ändern Sie die Zielressource-Objekt zugreifen, automatisch aktiviert ist.  Nicht aktiviert ist, muss, ein Benutzer nach Abschluss die Überprüfung die Überprüfung Access anwenden. |
| `accessRecommendationsEnabled`|`Boolean` | Flag, das angibt, ob Recommendations an Bearbeiter anzeigen aktiviert ist. |



## <a name="the-autoreviewsettings-type"></a>Geben Sie die autoReviewSettings

Die `autoReviewSettings` überprüfen Sie die Einstellungen der Access eingebettet ist, und gibt das Verhalten für das Feature, wenn eine Access-Überprüfung abgeschlossen hat.  Der Typ verfügt über eine Eigenschaft, `notReviewedResult`.

| Eigenschaft                     | Typ     | Beschreibung                          |
| :--------------------------- | :------  | :----------                          |
| `notReviewedResult`          |`String`  | Muss `Approve`, `Deny` oder `Recommendation` sein. |


## <a name="the-accessreviewrecurrencesettings-type"></a>Geben Sie die accessReviewRecurrenceSettings

Die `accessReviewRecurrenceSettings` überprüfen Sie die Einstellungen der Access eingebettet ist, und gibt an, dass die Überprüfung Access in regelmäßigen Abständen auftritt.  Dieser Typ hat die folgenden Eigenschaften:

| Eigenschaft                     | Typ                                                                                                          | Beschreibung |
| :--------------------------- | :------------------------------------------------------------------------------------------------------------ | :---------- |
| `recurrenceType`|`String`    | Das Serienintervall, die eine sein muss der `onetime`, `weekly`, `monthly`, `quarterly`, oder `annual`.                                                                   |
| `recurrenceEndType`|`String` | Das Serienmuster wie endet. Wenn es ist `Never`, und es keine explizite Ende der Serie ist. Wenn es ist `endBy`, klicken Sie dann das Serienmuster zu einem bestimmten Zeitpunkt endet. Wenn es ist `occurrences`, klicken Sie dann die Datenreihe endet nach `recurrentCount` Instanzen der Überprüfung abgeschlossen haben. |
| `durationInDays`|`Int32`     | Die Dauer in Tagen für die Serie.                                                                              |
| `recurrenceCount`|`Int32`    | Die Anzahl der Wiederholungen, wenn der Wert der `recurrenceEndType` ist `occurrences`, oder andernfalls 0.                                                        |



<!-- {
  "type": "#page.annotation",
  "description": "accessReview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
