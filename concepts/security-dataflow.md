---
title: Datenfluss in der Microsoft Graph Security-API
description: Die Microsoft Graph Security-API leitet Anforderungen im Verbund an alle Anbieter im Microsoft Graph Security-Ökosystem weiter. Dies basiert auf der Zustimmung des von der Anwendung bereitgestellten Sicherheitsanbieters, wie im folgenden Diagramm dargestellt. Der Ablauf der Zustimmung betrifft nur nicht von Microsoft stammende Anbieter.
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 47731520b9ae959212750aea4f9668d58ac85a08
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987811"
---
# <a name="microsoft-graph-security-api-data-flow"></a>Datenfluss in der Microsoft Graph Security-API

Die Microsoft Graph Security-API leitet Anforderungen im Verbund an alle Anbieter im Microsoft Graph Security-Ökosystem weiter. Dies basiert auf der Zustimmung des von der Anwendung bereitgestellten Sicherheitsanbieters, wie im folgenden Diagramm dargestellt. Der Ablauf der Zustimmung betrifft nur nicht von Microsoft stammende Anbieter.

![security_dataflow_1.png](./images/security-dataflow-1.png)

Im Folgenden finden Sie eine Beschreibung des Ablaufs:

1. Der Anwendungsbenutzer meldet sich bei der Anbieteranwendung an, um das Zustimmungsformular vom Anbieter anzuzeigen. Die Benutzeroberfläche dieses Zustimmungsformulars ist im Besitz des Anbieters und betrifft nur nicht von Microsoft stammende Anbieter, um die ausdrückliche Zustimmung ihrer Kunden zum Senden von Anforderungen an die Microsoft Graph Security-API einzuholen.
2. Die Zustimmung des Kunden wird auf der Anbieterseite gespeichert.
3. Der Zustimmungsdienst des Anbieters ruft die Microsoft Graph Security-API auf, um über die erteilte Zustimmung für den betreffenden Kunden zu informieren.
4. Die Anwendung sendet eine Anforderung an die Microsoft Graph Security-API.
5. Die Microsoft Graph Security-API prüft die den verschiedenen Anbietern zugeordneten Zustimmungsinformationen für diesen Kunden nach.
6. Die Microsoft Graph Security-API ruft alle Anbieter auf, denen der Kunde mithilfe der Zustimmungsfunktionalität des Anbieters eine explizite Zustimmung erteilt hat.
7. Die Antwort wird von allen Anbietern zurückgegeben, die eine Zustimmung für diesen Kunden erhalten haben.
8. Die Antwort wird in Form eines Resultsets an die Anwendung zurückgegeben.
9. Wenn der Kunde keinem Anbieter zugestimmt hat, sind in der Antwort keine Ergebnisse dieser Anbieter enthalten.
