---
title: Microsoft Graph Data Connect (Vorschau)
description: 'Microsoft Graph Data Connect gibt Ihnen Office 365-Daten und Microsoft Azure-Ressourcen mithilfe einer Kerndatenpipeline an die Hand. Mit Microsoft Graph Data Connect können Sie intelligente Anwendungen erstellen, die unter Nutzung der besten Entwicklungstools von Microsoft auf wertvolle Daten zugreifen, und all das in der sicheren Microsoft-Cloud. Alle Unternehmen sind daran interessiert, ihre Produktivität zu steigern. Daher bietet die Entwicklung von Produkten, die Wissensarbeiter produktiver machen, enorme Möglichkeiten. '
author: ajacks-msft
ms.openlocfilehash: 283ad9044eb5ae5bc53bb4b72e4d6d1f2434cfee
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315267"
---
# <a name="microsoft-graph-data-connect-preview"></a>Microsoft Graph Data Connect (Vorschau)

Microsoft Graph Data Connect gibt Ihnen Office 365-Daten und Microsoft Azure-Ressourcen mithilfe einer Kerndatenpipeline an die Hand. Mit Microsoft Graph Data Connect können Sie intelligente Anwendungen erstellen, die unter Nutzung der besten Entwicklungstools von Microsoft auf wertvolle Daten zugreifen, und all das in der sicheren Microsoft-Cloud. Alle Unternehmen sind daran interessiert, ihre Produktivität zu steigern. Daher bietet die Entwicklung von Produkten, die Wissensarbeiter produktiver machen, enorme Möglichkeiten. 

Sie können Microsoft Graph Data Connect nutzen, wenn Sie zu einer dieser Personengruppen gehören:

- Unabhängiger Softwareanbieter, der intelligente Anwendungen für Office 365-Kunden erstellt.
- Entwickler in einem Unternehmen, der intelligente Anwendungen für alle Benutzer innerhalb seiner Organisation entwickelt, die auf Office 365-Daten zugreifen.

## <a name="develop-a-pipeline-with-office-365-data"></a>Entwickeln einer Pipeline mit Office 365-Daten
Sie können Microsoft Graph Data Connect verwenden, um neue Typen von Anwendungen zu erstellen, die Office 365-Daten nutzen, und dabei die Vorzüge der besten Tools in Microsoft Azure genießen. Mithilfe von Azure Data Factory können Sie Office 365-Daten in beliebte Azure-Datenspeicher verschieben: Azure Data Lake Gen 1 oder Gen 2 (Vorschau) oder Azure Blob Storage. Anschließend können Sie die Daten verarbeiten (beispielsweise mit Azure Data Lake Analytics) oder sie in einen zusätzlichen Speicher verschieben, z. B. Azure SQL-Datenbank. Dann können Sie die Daten dafür verwenden, das Endbenutzerszenario Ihrer Anwendung zu unterstützen.

Bevor die Azure Data Factory-Pipeline Daten aus Office 365 verschieben kann, wird eine Einwilligung zur Datenanforderung an die vom Office 365-Administrator ernannten Genehmigungsinstanzen für Daten gesendet. Das Verschieben von Daten beginnt erst nach der Genehmigung durch die Genehmigungsinstanzen.

## <a name="publish-your-app-as-an-azure-managed-application"></a>Veröffentlichen der App als von Azure verwaltete Anwendung
Nach dem Entwickeln einer Anwendung mithilfe von Microsoft Graph Data Connect können Sie Ihre Anwendung anderen zur Verfügung stellen (entweder in ihrem Unternehmen oder mit breiterer Verfügbarkeit). Microsoft Graph Data Connect verwendet [Azure Managed Applications](https://docs.microsoft.com/de-DE/azure/managed-applications/overview), um diese Anwendungen anderen Personen über den Microsoft Azure Marketplace zur Verfügung zu stellen. Mithilfe von Azure Managed Applications können unabhängige Softwareanbieter ihren Kunden schlüsselfertige Lösungen bieten. Kunden setzen diese verwalteten Anwendungen in ihren Abonnements ein, während die Anbieter (unabhängige Softwareanbieter und Entwickler in Unternehmen) Verwaltung und Support übernehmen. Anbieter von Anwendungen können darüber hinaus [Richtlinien](https://docs.microsoft.com/de-DE/azure/managed-applications/overview#azure-policy) auf ihre Anwendungen anwenden, beispielsweise zur Verschlüsselung ruhender Daten, um ihren Kunden die Gewissheit zu geben, dass die Verarbeitung ihrer Daten sicherer erfolgt. Anwendungen können entweder im [Azure Marketplace](https://docs.microsoft.com/de-DE/azure/managed-applications/publish-marketplace-app) oder im [Azure-Dienstkatalog](https://docs.microsoft.com/de-DE/azure/managed-applications/publish-service-catalog-app) veröffentlicht werden.

Kunden, die die Anwendung installieren, werden die Nutzungsbedingungen, die erforderlichen Daten, der Preis für jede Anwendungs-SKU und die ungefähren Kosten für die Ressourcennutzung angezeigt. Wenn die Eigenschaften vom Käufer angegeben werden, werden die Ressourcen bereitgestellt. Dies schließt die Data Factory-Pipeline ein, die mit dem Extrahieren von Daten beginnt. Sie stellen eine Infodatei für Ihre Anwendung zur Verfügung, die erläutert, wann die Installation normalerweise abgeschlossen ist, wie die Anwendung verwendet wird und wo Support angefordert werden kann.

## <a name="next-steps"></a>Nächste Schritte 
Anweisungen zum Einstieg in die Entwicklung von Microsoft Graph Data Connect-Anwendungen finden Sie unter [Microsoft Graph Data Connect – Übersicht](data-connect-concept-overview.md).
