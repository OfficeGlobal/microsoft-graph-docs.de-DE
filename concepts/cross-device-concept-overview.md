---
title: Geräteübergreifende Oberflächen in Microsoft Graph
description: 'Die Gerätevielfalt ist heute nahezu unüberschaubar. Heimanwender nutzen Geräte in den verschiedensten Formfaktoren und mit den unterschiedlichsten Plattformen: Morgens lesen sie die neuesten Nachrichten auf ihrem Tablet, auf dem Weg zur Arbeit checken sie ihre E-Mails auf dem Smartphone und im Büro erledigen sie ihre Aufgaben am Desktop-PC. Abends schauen sie sich vielleicht einen Film auf ihrer Heimkonsole an und hören über intelligente Lautsprecher die Nachrichten des Tages. Der durchschnittliche Kunde nutzt im Laufe des Tages mehrere verschiedene Geräte und Plattformen. '
localization_priority: Priority
ms.prod: project-rome
ms.openlocfilehash: 85d48d07f06d189f30c8eba9f7f0876353b3ff25
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920682"
---
# <a name="cross-device-experiences-in-microsoft-graph"></a>Geräteübergreifende Oberflächen in Microsoft Graph

Die Gerätevielfalt ist heute nahezu unüberschaubar. Heimanwender nutzen Geräte in den verschiedensten Formfaktoren und mit den unterschiedlichsten Plattformen: Morgens lesen sie die neuesten Nachrichten auf ihrem Tablet, auf dem Weg zur Arbeit checken sie ihre E-Mails auf dem Smartphone und im Büro erledigen sie ihre Aufgaben am Desktop-PC. Abends schauen sie sich vielleicht einen Film auf ihrer Heimkonsole an und hören über intelligente Lautsprecher die Nachrichten des Tages. Der durchschnittliche Kunde nutzt im Laufe des Tages mehrere verschiedene Geräte und Plattformen. 

In der Vergangenheit war das Nutzungsverhalten zwischen den einzelnen Formfaktoren klar abgegrenzt, und es wurden auf jedem Formfaktor spezifische Aufgaben erledigt. Heute jedoch nutzen Heimanwender verschiedenste Geräte und möchten auf jedem einzelnen von ihnen auch jede Aktivität durchführen können. Die während eines typischen Tages anfallenden Aufgaben (ob zu Hause im Familienkreis oder im Büro unter Kollegen) sind nicht mehr geräteorientiert, sondern **anwenderorientiert**. Heimanwender möchten jederzeit genau den Bildschirm verwenden können, den sie gerade zur Hand haben, unabhängig von der Eingabequelle. In der Realität stellt sich dabei oft heraus, dass jedes Gerät Einschränkungen mit sich bringt. Geräteübergreifendes Arbeiten erfordert unnatürliche Aktionen: Der Anwender muss sich selbst eine E-Mail schicken oder muss USB-Sticks verwenden. Der Kunde erlebt beim Wechsel zwischen seinen Geräten einen Bruch, und manchmal wird aufgrund eben dieses Kontextwechsels Wichtiges nicht erledigt. Auch für Entwickler ergeben sich dadurch Herausforderungen. Wenn Kunden bei der Nutzung einer App Brüche erleben, sinkt ihre Akzeptanz der App.

Microsoft arbeitet derzeit an einer Plattform zur Erstellung von Oberflächen, die die Beschränkungen einzelner Geräte aufheben und eine geräteübergreifende Harmonisierung möglich machen. Mit ihr können Sie **anwenderorientierte** Szenarien erstellen, die den Benutzer begleiten und Einschränkungen zwischen Geräten aufheben, unabhängig von Formfaktor oder Plattform. Microsoft Graph ist ein zentraler, vereinheitlichter Endpunkt für den Zugriff auf Daten aus Azure Active Directory und Office 365. Ab sofort können Sie über Microsoft Graph zusätzlich auf die Aktivitäten und Geräte Ihrer Kunden zugreifen und funktionsreiche, anwenderorientierte Oberflächen entwerfen, die auf allen Geräten und Plattformen zur Verfügung stehen. 

## <a name="why-invest-in-cross-device-experiences"></a>Gründe für eine Investition in geräteübergreifende Oberflächen

### <a name="let-customers-pick-up-where-they-leave-off-with-the-activity-feed-api"></a>Nahtlose Fortsetzung von begonnenen Aktivitäten mit der Aktivitätsfeed-API 
Mithilfe von Aktivitäten können Sie die einzelnen Aufgaben der Benutzer Ihrer App erfassen und nahtlos auf allen Plattformen und Geräten bereitstellen. Die Benutzer können im Handumdrehen mit ihrer Arbeit fortfahren, und das auf ihrem bevorzugten Bildschirm. Der Aktivitätsfeed ermöglicht es Ihnen, anwenderorientierte Ansichten der wichtigsten Aufgaben eines Benutzers zu erstellen. Das reduziert den Bruch beim Wechsel zwischen Internet, Mobilgerät und PC. 

### <a name="build-rich-cross-device-experiences-by-using-the-device-relay-api"></a>Erstellen funktionsreicher geräteübergreifender Oberflächen mithilfe der Geräterelay-API 
Die Geräterelay-API macht neben Microsoft-Geräten (PCs, Windows Phones, Xbox, IoT, HoloLens etc.) auch Android- und iOS-Geräte verfügbar. So lassen sich die Barrieren zwischen den Geräten Ihrer Benutzer effektiv aufbrechen. Sie können Apps erstellen, die auf die Benutzerumgebung zurückgreifen, und funktionsreiche Oberflächen entwerfen, die nicht auf ein einzelnes Gerät beschränkt sind, sondern sich in Echtzeit überall nutzen lassen. 

### <a name="engage-users-with-human-centric-cross-device-notifications-preview"></a>Ansprechen von Benutzern mit geräteübergreifenden, an den Benutzer gerichteten Benachrichtigungen (Vorschau)

Benachrichtigungen sind eine der wirksamsten und direkten Methoden, um mit Benutzern zu kommunizieren und zu interagieren. 

Mit der Benachrichtigungs-API in Microsoft Graph können Sie Benachrichtigungen an Personen und nicht an Geräte richten. Sie können auf einen Benutzer abzielen, der Benachrichtigungen erhalten soll, und das Benachrichtigungsframework von Microsoft Graph verwenden, um die Benachrichtigungen an die einzelnen Endpunkte zu übermitteln, an denen der Benutzer angemeldet ist. Die geräteübergreifende Verwaltung von Benachrichtigungen wird auch durch die Benachrichtigungs-API von Microsoft Graph erleichtert: Sie können Benachrichtigungen über Benutzergeräte hinweg synchronisieren und die Redundanz und Unterbrechung für Ihre Benutzer reduzieren. 

## <a name="api-reference"></a>API-Referenz
Suchen Sie die API-Referenz für diesen Dienst?

- [API für geräteübergreifende Oberflächen in Microsoft Graph v1.0](/graph/api/resources/project-rome-overview?view=graph-rest-1.0)
- [API für geräteübergreifende Oberflächen in Microsoft Graph, Betaversion](/graph/api/resources/project-rome-overview?view=graph-rest-beta)


## <a name="next-steps"></a>Nächste Schritte

- [Use the Microsoft Graph API to enable cross-device experiences](/graph/api/resources/cross-device-reference-overview?view=graph-rest-1.0)
- [Weitere Informationen zur Aktivitätsfeed-API in Microsoft Graph](activity-feed-concept-overview.md)
- [Weitere Informationen zur Geräterelay-API in Microsoft Graph](device-relay-concept-overview.md)
- [Weitere Informationen zur Benachrichtigungs-API in Microsoft Graph](notifications-concept-overview.md)
