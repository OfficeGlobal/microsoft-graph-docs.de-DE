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
# <a name="microsoft-graph-security-api-data-flow"></a><span data-ttu-id="f8a7e-105">Datenfluss in der Microsoft Graph Security-API</span><span class="sxs-lookup"><span data-stu-id="f8a7e-105">Microsoft Graph Security API data flow</span></span>

<span data-ttu-id="f8a7e-106">Die Microsoft Graph Security-API leitet Anforderungen im Verbund an alle Anbieter im Microsoft Graph Security-Ökosystem weiter.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-106">The Microsoft Graph Security API federates requests to all providers in the Microsoft Graph Security ecosystem.</span></span> <span data-ttu-id="f8a7e-107">Dies basiert auf der Zustimmung des von der Anwendung bereitgestellten Sicherheitsanbieters, wie im folgenden Diagramm dargestellt.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-107">This is based on the security provider consent provided by the application, as shown in the following diagram.</span></span> <span data-ttu-id="f8a7e-108">Der Ablauf der Zustimmung betrifft nur nicht von Microsoft stammende Anbieter.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-108">The consent workflow only applies to non-Microsoft providers.</span></span>

![security_dataflow_1.png](./images/security-dataflow-1.png)

<span data-ttu-id="f8a7e-110">Im Folgenden finden Sie eine Beschreibung des Ablaufs:</span><span class="sxs-lookup"><span data-stu-id="f8a7e-110">The following is a description of the flow:</span></span>

1. <span data-ttu-id="f8a7e-111">Der Anwendungsbenutzer meldet sich bei der Anbieteranwendung an, um das Zustimmungsformular vom Anbieter anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-111">The application user signs in to the provider application to view the consent form from the provider.</span></span> <span data-ttu-id="f8a7e-112">Die Benutzeroberfläche dieses Zustimmungsformulars ist im Besitz des Anbieters und betrifft nur nicht von Microsoft stammende Anbieter, um die ausdrückliche Zustimmung ihrer Kunden zum Senden von Anforderungen an die Microsoft Graph Security-API einzuholen.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-112">This consent form experience or UI is owned by the provider and applies to non-Microsoft providers only to get explicit consent from their customers to send requests to Microsoft Graph Security API.</span></span>
2. <span data-ttu-id="f8a7e-113">Die Zustimmung des Kunden wird auf der Anbieterseite gespeichert.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-113">The client consent is stored on the provider side.</span></span>
3. <span data-ttu-id="f8a7e-114">Der Zustimmungsdienst des Anbieters ruft die Microsoft Graph Security-API auf, um über die erteilte Zustimmung für den betreffenden Kunden zu informieren.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-114">The provider consent service calls the Microsoft Graph Security API to inform consent approval for the respective customer.</span></span>
4. <span data-ttu-id="f8a7e-115">Die Anwendung sendet eine Anforderung an die Microsoft Graph Security-API.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-115">The application sends a request to the Microsoft Graph Security API.</span></span>
5. <span data-ttu-id="f8a7e-116">Die Microsoft Graph Security-API prüft die den verschiedenen Anbietern zugeordneten Zustimmungsinformationen für diesen Kunden nach.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-116">The Microsoft Graph Security API checks for the consent information for this customer mapped to various providers.</span></span>
6. <span data-ttu-id="f8a7e-117">Die Microsoft Graph Security-API ruft alle Anbieter auf, denen der Kunde mithilfe der Zustimmungsfunktionalität des Anbieters eine explizite Zustimmung erteilt hat.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-117">The Microsoft Graph Security API calls all those providers the customer has given explicit consent to via the provider consent experience.</span></span>
7. <span data-ttu-id="f8a7e-118">Die Antwort wird von allen Anbietern zurückgegeben, die eine Zustimmung für diesen Kunden erhalten haben.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-118">The response is returned from all the consented providers for that client.</span></span>
8. <span data-ttu-id="f8a7e-119">Die Antwort wird in Form eines Resultsets an die Anwendung zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-119">The result set response is returned to the application.</span></span>
9. <span data-ttu-id="f8a7e-120">Wenn der Kunde keinem Anbieter zugestimmt hat, sind in der Antwort keine Ergebnisse dieser Anbieter enthalten.</span><span class="sxs-lookup"><span data-stu-id="f8a7e-120">If the customer has not consented to any provider, no results from those providers are included in the response.</span></span>
