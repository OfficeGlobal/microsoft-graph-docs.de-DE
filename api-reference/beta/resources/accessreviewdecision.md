---
title: Ressourcentyp accessReviewDecision
description: In Azure AD Access Feature, überprüft die `accessReviewDecision` eine Azure AD Access Treffen einer Entscheidung anhand des Zugriffs für eine bestimmte Entität darstellt.  In einer Access-Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung, ist eine `accessReviewDecision` pro überprüfter Benutzer.  Beispielsweise eine Gruppe besitzt zwei Gäste und einen anderen Typ als Mitglieder und einer Access-Überprüfung von Gästen für diese Gruppe erfolgt dann zwei Access überprüfen Entscheidung-Objekte werden.  Wenn ein Bearbeiter ihre Entscheidung ändert oder einen anderen Prüfer diese überschreibt, und klicken Sie dann die `accessReviewDecision` wird aktualisiert.
localization_priority: Normal
ms.openlocfilehash: 208337f3427fad65499b400dee769d379c38dcb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870049"
---
# <a name="accessreviewdecision-resource-type"></a>Ressourcentyp accessReviewDecision

> **Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen. Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.

In der Azure AD [Access überprüft](accessreviews-root.md) -Funktion die `accessReviewDecision` eine Azure AD Access Treffen einer Entscheidung anhand des Zugriffs für eine bestimmte Entität darstellt.  In einer Access-Überprüfung oder eine Instanz einer wiederkehrenden Access Überprüfung, ist eine `accessReviewDecision` pro überprüfter Benutzer.  Beispielsweise eine Gruppe besitzt zwei Gäste und einen anderen Typ als Mitglieder und einer Access-Überprüfung von Gästen für diese Gruppe erfolgt dann zwei Access überprüfen Entscheidung-Objekte werden.  Wenn ein Bearbeiter ihre Entscheidung ändert oder einen anderen Prüfer diese überschreibt, und klicken Sie dann die `accessReviewDecision` wird aktualisiert.


## <a name="methods"></a>Methoden

Keine.  Objekte dieses Typs werden automatisch vom Feature erstellt, wenn eine Access initialisiert überprüfen, und kann nicht gelöscht werden.  Sie können von einer Access-Überprüfung mit den Beziehungen [Entscheidungen](../api/accessreview-listdecisions.md) und [Mydecisions](../api/accessreview-listmydecisions.md) abgerufen werden.

## <a name="properties"></a>Eigenschaften

Die folgende Tabelle zeigt die Basiseigenschaften Objekte dieses Typs. 

| Eigenschaft                        | Typ                         | Beschreibung                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `id`                            |`String`                      | Die Id der Entscheidung in die Access-Überprüfung.                                                                                     |
| `accessReviewId`                |`String`                      | Die Funktion generierte Id der Überprüfung Zugriff.                                                                                       |
| `reviewedBy`                    |[Benutzeridentität](useridentity.md)| Die Identität des Bearbeiters.                                                                                       |
| `reviewedDate`                  |`DateTimeOffset`              | Datum und Uhrzeit die letzte Überprüfung für dieses Zugriffsrecht angegeben wurde.                                                                         |
| `reviewResult`                  |`String`                      | Das Ergebnis der Überprüfung.                                                                                    |
| `justification`                 |`String`                      | Der Prüfer-unternehmensvorgabe, wenn angegeben.                                                                         |
| `appliedBy`                     |[Benutzeridentität](useridentity.md)| Wenn die Überprüfung abgeschlossen ist, wenn die Ergebnisse manuell angewendet wurden, die Benutzeridentität des Benutzers, der die Entscheidung angewendet.                                                           |
| `appliedDateTime`               |`DateTimeOffset`              | Datum und Uhrzeit, wann die Überprüfung Entscheidung angewendet wurde.                                                          |
| `applyResult`                   |`String`                      | Das Ergebnis der Anwendung der Entscheidung, eine der `NotApplied`, `Success`, `Failed`, `NotFound` oder `NotSupported`.                      |
| `accessRecommendation`          |`String`                      | Die Feature-generiert Empfehlung dargestellt, um der Prüfer, eine der `Approve`, `Deny` oder `NotAvailable`. |


Darüber hinaus können zusätzliche Eigenschaften vorhanden sein, je nach Typ des des-Objekts mit dem Zugriff, der beschlossen wurde.  Ist die Entscheidung Access überprüfen Gruppenmitgliedschaft eines bestimmten Benutzers oder Anwendungszugriff, wird der Benutzer potenziell ihre entfernt werden, werden über diese Eigenschaften identifiziert:

| Eigenschaft                        | Typ                         | Beschreibung                                                                                            |
| :------------------------------ | :-----------------------     | :----------------------------------------------------------------------------------------------------- |
| `userId`                            |`String`                      | Die Id des Benutzers, dessen Zugriff überprüft wurde.                                                                                    |
| `userDisplayName`                            |`String`                      | Der Anzeigename des Benutzers, dessen Zugriff überprüft wurde.                                                                                     |
| `userPrincipalName`                            |`String`                      | Der Benutzerprinzipalname des Benutzers, dessen Zugriff überprüft wurde.                                                                                     |



## <a name="relationships"></a>Beziehungen

Keine.  Objekte dieses Typs können aus einer Access-Überprüfung mit den Beziehungen [Entscheidungen](../api/accessreview-listdecisions.md) und [Mydecisions](../api/accessreview-listmydecisions.md) des [AccessReview](accessreview.md) -Objekts abgerufen werden.

## <a name="see-also"></a>Siehe auch

| Methode           | Rückgabetyp    |Beschreibung|
|:---------------|:--------|:----------|
|[Liste AccessReview Entscheidungen](../api/accessreview-listdecisions.md) |      [AccessReviewDecision](accessreviewdecision.md) -Auflistung| Rufen Sie die Entscheidungen des ein AccessReview.|
|[Meine AccessReview Entscheidungen auflisten](../api/accessreview-listmydecisions.md) |     [AccessReviewDecision](accessreviewdecision.md) -Auflistung| Rufen Sie als "Leser" Mein Entscheidungen von einer AccessReview.|

## <a name="json-representation"></a>JSON-Darstellung

Es folgt eine JSON-Darstellung der Ressource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessReviewDecision"
}-->

```json
{
"id": "string (identifier)",
"accessReviewId": "string (identifier)",
"reviewedBy": "microsoft.graph.userIdentity",
"reviewedDate": "string (timestamp)",
"reviewResult": "string",
"justification": "string",
"appliedBy": "microsoft.graph.userIdentity",
"appliedDateTime": "string (timestamp)",
"applyResult": "string",
"accessRecommendation": "string",
"userId": "string",
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- {
  "type": "#page.annotation",
  "description": "accessReviewDecision resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
