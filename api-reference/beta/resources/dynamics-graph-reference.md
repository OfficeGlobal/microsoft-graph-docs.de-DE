---
title: Arbeiten mit der Dynamics 365 Business Central-API in Microsoft Graph
description: API-Dokumentation für die Integration in Microsoft Graph
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: ee67d28a90732bdc1d804da41994de32bf0a7f4f
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366592"
---
# <a name="working-with-the-dynamics-365-business-central-api-in-microsoft-graph"></a>Arbeiten mit der Dynamics 365 Business Central-API in Microsoft Graph
Sie können Microsoft Graph verwenden, um Ihren Webdienst oder Ihre SaaS-Lösung mit Microsoft Dynamics 365 Business Central zu verbinden und zu integrieren. Mit Microsoft Graph können Sie Apps erstellen, die einen autorisierten Zugriff auf und nahtlose Integration in Microsoft Dynamics 365 Business Central-Daten erhalten.

## <a name="authorization"></a>Authorization
Verwenden Sie den Azure AD v 2.0-Endpunkt, um Dynamics 365 Business Central-APIs zu authentifizieren. Alle APIs erfordern den `Authorization: Bearer {access-token}` Anforderungsheader. Weitere Informationen zur Autorisierung finden Sie unter [Abrufen von Zugriffstoken zum Aufrufen von Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).

## <a name="common-dynamics-365-business-central-scenarios"></a>Allgemeine Dynamics 365 Geschäftszentrale Szenarien
Die Dynamics 365 Business Central-API ermöglicht das Lesen und Ändern von Geschäftsdaten über apps, die über einen einzigen Endpunkt verbunden und integriert sind. Verwenden Sie die API, um beispielsweise Zugriff auf [Kunden](../resources/dynamics-customer.md) -und [Lieferanten](../resources/dynamics-vendor.md) Informationen zu erhalten oder über [fällige Zahlungen anzuzeigen](../resources/dynamics-agedaccountspayable.md).

## <a name="next-steps"></a>Nächste Schritte
Die Dynamics 365 Business Central-API kann Ihnen neue Möglichkeiten für die Interaktion mit Benutzern eröffnen. Weitere Informationen finden Sie in den folgenden Themen:

+ [Dynamics 365 Business Central (Übersicht)](/graph/dynamics-business-central-concept-overview)
+ Testen Sie [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).

<!--
|For Resource Type |See                                                 |
|:-----------------|:---------------------------------------------------|
|account resource type|[account](../resources/dynamics-account.md)|
|aged accounts receivable resource type|[agedAccountsReceivable](../resources/dynamics-agedaccountsreceivable.md)|
|aged accounts payable resource type|[agedAccountsPayable](../resources/dynamics-agedaccountspayable.md)|
|balance sheet resource type|[balanceSheet](../resources/dynamics-balancesheet.md)|
|companies resource type|[companies](../resources/dynamics-companies.md)|
|companyInformation resource type|[companyInformation](../resources/dynamics-companyinformation.md)|
|countriesRegions resource type|[countriesRegions](../resources/dynamics-countriesregions.md)|
|currencies resource type|[currencies](../resources/dynamics-currencies.md)|
|customer resource type|[customer](../resources/dynamics-customer.md)|
|customerPaymentJournal resource type|[customerPaymentsJournal](../resources/dynamics-customerpaymentsjournal.md)|
|customerPayment resource type|[customerPayment](../resources/dynamics-customerpayment.md)|
|dimension resource type|[dimension](../resources/dynamics-dimension.md)|
|dimensionValue resource type|[dimensionValue](../resources/dynamics-dimensionvalue.md)
|employee resource type|[employee](../resources/dynamics-employee.md)|
|generalLedgerEntries resource type|[generalLedgerEntries](../resources/dynamics-generalledgerentries.md)|
|item resource type|[item](../resources/dynamics-item.md)|
|itemCategories resource type|[itemCategories](../resources/dynamics-itemcategories.md)|
|income statement resource type|[incomeStatement](../resources/dynamics-incomestatement.md)|
|IRS1099 resource type|[irs1099](../resources/dynamics-irs1099.md)|
|journal resource type|[journal](../resources/dynamics-journal.md)|
|journalLine resource type|[journalLine](../resources/dynamics-journalline.md)|
|paymentMethods resource type|[paymentMethods](../resources/dynamics-paymentmethods.md)|
|paymentTerms resource type|[paymentTerms](../resources/dynamics-paymentterms.md)|
|retained earnings statement resource type|[retainedEarningsStatement](../resources/dynamics-retainedearningsstatement.md)|
|shipmentMethods resource type|[shipmentMethods](../resources/dynamics-shipmentmethods.md)|
|taxGroups resource type|[taxGroups](../resources/dynamics-taxgroups.md)|
|taxArea resource type|[taxAreas](..resources/dynamics-taxarea.md)|
|trial balance resource type|[trialBalance](../resources/dynamics-trialbalance.md)|
|unitsOfMeasure resource type|[unitsOfMeasure](../resources/dynamics-unitsofmeasure.md)|
|vendor resource type|[vendor](../resources/dynamics-vendor.md)|
-->
