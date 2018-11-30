---
title: Posteingang mit Relevanz verwalten
description: 'Fokussierte Posteingang können Sie wichtige Nachrichten in Anzeigen der `Focused` auf der Registerkarte Posteingang und dem Rest der Posteingangsnachrichten in der `Other` Registerkarte. Das System Klassifikation '
ms.openlocfilehash: 1e1a4fa091c618c4f51a5621b8800d35c8c4cf5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020013"
---
# <a name="manage-focused-inbox"></a>Posteingang mit Relevanz verwalten

Mit dem Posteingang mit Relevanz können Sie wichtige Nachrichten auf der Registerkarte `Focused` des Posteingangs und die restlichen Posteingangsnachrichten auf der Registerkarte `Other` verwalten. Das Klassifizierungssystem organisiert anfänglich Nachrichten im Posteingang mit einer Standardmethode. Sie können das System mit der Zeit über die Benutzeroberfläche oder programmgesteuert korrigieren und trainieren. Je häufiger Sie das System verwenden, desto besser kann es schließen, welche eingehenden Nachrichten wichtig sind.

Auf programmgesteuerter Ebene arbeitet die REST-API des Posteingangs mit Relevanz mit den Nachrichten des angegebenen Benutzers und unterstützt für jede Nachricht eine **inferenceClassification**-Eigenschaft. Die möglichen Werte sind `Focused` und `Other`, die angeben, ob der Benutzer diese Nachricht für mehr bzw. weniger wichtig hält. Um zu korrigieren, wie das System eine Nachricht klassifiziert, [aktualisieren Sie die inferenceClassification-Eigenschaft dieser Nachricht](../api/message-update.md). Im Laufe der Zeit wird durch diese Korrekturen auch das Nachrichtenklassifizierungssystem geschult.

Mit der REST-API des Posteingangs mit Relevanz können Sie auch Außerkraftsetzungen erstellen. Jede Außerkraftsetzung, die durch eine Instanz von [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) dargestellt wird, ist eine Anweisung an das Klassifizierungssystem, Nachrichten von einem bestimmten Absender immer einheitlich zu bezeichnen (also immer als relevante oder als sonstige Nachrichten), unabhängig von allen zuvor trainierten Vorgehensweisen. Sie können Außerkraftsetzungen für den angegebenen Benutzer [erstellen](../api/inferenceclassification-post-overrides.md), [auflisten](../api/inferenceclassification-list-overrides.md), [aktualisieren](../api/inferenceclassificationoverride-update.md) und [löschen](../api/inferenceclassificationoverride-delete.md). Falls Außerkraftsetzungen für diesen Benutzer vorhanden sind, kann darauf in einer **inferenceClassification**-Navigationseigenschaft zugegriffen werden. Dabei handelt es sich um eine Sammlung von **inferenceClassificationOverride**-Instanzen. Anhand von Außerkraftsetzungen erhält der Benutzer mehr Kontrolle über die Klassifizierung von eingehenden Nachrichten, und das Klassifizierungssystem wird zuverlässiger.

Beachten Sie, dass das Klassifizierungssystem nur für eingehende Nachrichten im Posteingang trainiert wird und Klassifizierungen anwendet. Nachrichten in anderen Ordnern sind standardmäßig als relevant eingestuft. Wenn eine Außerkraftsetzung eingerichtet wird, wirkt sie sich auf zukünftig im Posteingang eingehende Nachrichten aus; die **inferenceClassification**-Eigenschaft für vorhandene Nachrichten in beliebigen Ordnern, einschließlich des Posteingangs, wird nicht geändert.

## <a name="focused-inbox-api"></a>API des Posteingangs mit Relevanz

**Trainieren des Nachrichtenklassifizierungssystems**

[Aktualisieren der inferenceClassification-Eigenschaft einer Nachricht](../api/message-update.md)


**Verwenden von Außerkraftsetzungen, um einheitlich nach Absender zu klassifizieren**

[Erstellen einer Außerkraftsetzung für einen Absender](../api/inferenceclassification-post-overrides.md) | [Auflisten aller Außerkraftsetzungen für Benutzer](../api/inferenceclassification-list-overrides.md) |

[Aktualisieren einer Außerkraftsetzung für einen Absender](../api/inferenceclassificationoverride-update.md) | [Löschen einer Außerkraftsetzung für einen Absender](../api/inferenceclassificationoverride-delete.md) 
