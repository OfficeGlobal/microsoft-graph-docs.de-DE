---
title: Einladungs-Manager
description: 'Verwenden Sie den Einladungs-Manager, um eine Einladung zum Hinzufügen eines externen Benutzers zu der Organisation zu erstellen. '
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0a0ee3ba23cb0c323a660b9afd26fa044a50897c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976737"
---
# <a name="invitation-manager"></a>Einladungs-Manager

Verwenden Sie den Einladungs-Manager, um eine Einladung zum Hinzufügen eines externen Benutzers zu der Organisation zu erstellen. 

Der Einladungsprozess verwendet den folgenden Ablauf:

* Eine Einladung wird erstellt.
* Eine Einladung (mit einem Einladungs-Link) wird an den eingeladenen Benutzer gesendet.
* Der eingeladene Benutzer klickt auf den Einladungs-Link, meldet sich an und löst die Einladung und die Erstellung der Benutzerentität ein, die den eingeladenen Benutzer darstellt.
* Der Benutzer wird nach Abschluss der Einlösung zu einer bestimmten Seite umgeleitet.

Durch Erstellen einer Einladung wird eine URL für die Einlösung in der Antwort zurückgegeben (*InviteRedeemUrl*). Die API zum Erstellen der Einladung kann automatisch eine E-Mail mit der Einlösungs-URL an den eingeladenen Benutzer senden, indem *sendInvitationMessage* auf „true“ festgelegt wird. Sie können die Nachricht, die an den eingeladenen Benutzer gesendet wird, auch anpassen. Wenn Sie die Einlösungs-URL anderweitig versenden möchten, können Sie die *sendInvitationMessage* auf „false“ festlegen und die Einlösungs-URL aus der Antwort verwenden, um Ihre eigene Mitteilung zu erstellen. Derzeit gibt es keine API, die den Einlösungsprozess durchführt. Der eingeladene Benutzer muss auf den Link *inviteRedeemUrl* klicken, der in der Mitteilung im Schritt oben versendet wurde, und den interaktiven Einlösungsprozess in einem Browser durchführen. Nach Abschluss wird der eingeladene Benutzer ein externer Benutzer in der Organisation.


## <a name="methods"></a>Methoden
| Methode       | Rückgabetyp  |Beschreibung|
|:---------------|:--------|:----------|
|[Einladung erstellen](../api/invitation-post.md) | invitation | Dient zum Schreiben der Eigenschaften und der Beziehungen des Einladungsobjekts.|

## <a name="properties"></a>Eigenschaften
| Eigenschaft     | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|invitedUserDisplayName|Zeichenfolge|Der Anzeigename des eingeladenen Benutzers.|
|invitedUserEmailAddress|Zeichenfolge|Die E-Mail-Adresse des eingeladenen Benutzers. Erforderlich. |
|invitedUserMessageInfo|[invitedUserMessageInfo](invitedusermessageinfo.md)|Zusätzliche Konfiguration für die an den eingeladenen Benutzer gesendete Nachricht, einschließlich des Anpassens des Nachrichtentexts, der Sprache und der Empfängerliste in CC.|
|sendInvitationMessage|Boolescher Wert|Gibt an, ob eine E-Mail-Nachricht an den eingeladenen Benutzer gesendet werden soll oder nicht. Der Standardwert ist „false“.|
|inviteRedirectUrl|Zeichenfolge|Die URL, an die der eingeladene Benutzer umgeleitet werden sollte, nachdem die Einladung eingelöst wurde. Erforderlich. |
|inviteRedeemUrl|Zeichenfolge|Die URL, die der Benutzer zum Einlösen seiner Einladung verwenden kann. Schreibgeschützt|
|invitedUserType|Zeichenfolge|Der userType des eingeladenen Benutzers. Standardmäßig ist dieser Wert auf „Gast“ festgelegt. Wenn Sie der Unternehmensadministrator sind, können Sie ihn als „Mitglied“ einladen. |
|status|Zeichenfolge|Der Status der Einladung. Mögliche Werte: PendingAcceptance, Completed, InProgress und Error|

## <a name="relationships"></a>Beziehungen
| Beziehung | Typ   |Beschreibung|
|:---------------|:--------|:----------|
|invitedUser|[Benutzer](user.md)|Der Benutzer, der im Rahmen der Einladungserstellung erstellt wurde. Schreibgeschützt|

## <a name="json-representation"></a>JSON-Darstellung
Es folgt eine JSON-Darstellung der Ressource.

<!-- { "blockType": "resource", "baseType": "microsoft.graph.entity", "@odata.type": "microsoft.graph.invitation" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",
  "invitedUser": {"@odata.type": "microsoft.graph.user"},
  "invitedUserType": "string"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
