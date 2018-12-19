---
title: Konfigurieren der integrierten Registerkartentypen in Microsoft Teams
description: So erstellen oder konfigurieren Sie eine Microsoft Teams-Registerkarte mithilfe von Microsoft Graph-APIs
author: nkramer
ms.openlocfilehash: 05a7f719cdedad8ea9040721d9411e45529d3c09
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316387"
---
# <a name="configuring-the-built-in-tab-types-in-microsoft-teams"></a>Konfigurieren der integrierten Registerkartentypen in Microsoft Teams

Um eine Microsoft Teams-Registerkarte mithilfe von Microsoft Graph-APIs zu [erstellen](/graph/api/teamstab-add?view=graph-rest-beta) oder zu [konfigurieren](/graph/api/teamstab-update?view=graph-rest-beta), müssen Sie die `teamsAppId` der App sowie die `entityId`, `contentUrl`, `removeUrl` und `websiteUrl` kennen, die für die Art der betreffenden App angegeben werden müssen.
In diesem Artikel wird erläutert, wie Sie diese Werte für die integrierten Registerkartentypen abrufen.

## <a name="custom-tabs"></a>Benutzerdefinierte Registerkarten

Um Microsoft Graph zum Konfigurieren einer Registerkarte zu verwenden, die einem von Ihnen geschriebenen [Registerkartenanbieter](https://docs.microsoft.com/de-DE/microsoftteams/platform/concepts/tabs/tabs-overview)zugeordnet ist, identifizieren Sie die `entityId`, `contentUrl`, `removeUrl` und `websiteUrl`, die die [Konfigurations-Benutzeroberfläche für Microsoft Teams bereitstellt](https://docs.microsoft.com/en-us/javascript/api/@microsoft/teams-js/microsoftteams.settings.settings?view=msteams-client-js-latest), und übergeben Sie eben diese Werte für `entityId`, `contentUrl`, `removeUrl` und `websiteUrl` an Microsoft Graph.

Die `teamsAppId` ist die gleiche wie die `id` im [App-Manifestschema für Microsoft Teams](https://docs.microsoft.com/de-DE/microsoftteams/platform/resources/schema/manifest-schema).

## <a name="website-tabs"></a>Website-Registerkarten

Für Website-Registerkarten lautet die `teamsAppId` `com.microsoft.teamspace.tab.web`. Die folgende Tabelle zeigt die Konfiguration.

| Eigenschaft   | Typ        | Beschreibung                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Null                                                     |
| contentUrl | string      | URL der Website                                       |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      | URL der Website                                       |

## <a name="planner-tabs"></a>Planner-Registerkarten

Die teamsAppId für Planner-Registerkarten lautet `com.microsoft.teamspace.tab.planner`. Die folgende Tabelle zeigt die Konfiguration.

| Eigenschaft   | Typ        | Beschreibung                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Die Plan-ID (die ID, die für "GET /planner/plans/{id}" verwendet wird).                                              |
| contentUrl | string      | `https://tasks.office.com/{tenantName}/Home/PlannerFrame?page=7&planId={planId}`, wobei {tenantName} der Name des Mandanten (wie etwa "example.onmicrosoft.com") und {planId} gleich der Entitäts-ID ist.  |
| removeUrl  | string      | Gleicher Wert wie contentUrl.    |
| websiteUrl | string      | Gleicher Wert wie contentUrl.   |

Informationen zum Erstellen eines neuen Plans zum Anzeigen auf Ihrer Planner-Registerkarte finden Sie unter [plannerPlan erstellen](/graph/api/planner-post-plans?view=graph-rest-beta).

## <a name="microsoft-stream-tabs"></a>Microsoft Stream-Registerkarten

Für Microsoft Stream-Registerkarten ist die `teamsAppId` `com.microsoftstream.embed.skypeteamstab`. Die folgende Tabelle zeigt die Konfiguration.

| Eigenschaft   | Typ        | Beschreibung                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Null                                                     |
| contentUrl | string      | `https://web.microsoftstream.com/embed/video/{id}?autoplay=false&showinfo=true&app=microsoftteams&l={locale}`, wobei {Id} die ID des Videostreams ist. Um die {id} eines Streams zu ermitteln, öffnen Sie den Stream in einem Browser, und sehen Sie die URL an – sie weist die Form `https://{domain}.microsoftstream.com/video/{id}` auf.  |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      | `https://web.microsoftstream.com/video/{id}`, wobei {id} die ID des Videostreams ist.    |

## <a name="microsoft-forms-tabs"></a>Microsoft Forms-Registerkarten

Für Microsoft Forms-Registerkarten ist die `teamsAppId` `81fef3a6-72aa-4648-a763-de824aeafb7d`.
Konfiguration:

| Eigenschaft   | Typ        | Beschreibung                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | Die ID des Formulars.  Definieren Sie diesen Wert, navigieren Sie zum Formular auf der Forms-Website, und suchen Sie die URL des Formulars `https://forms.office.com/Pages/DesignPage.aspx#FormId={formId}`.      |
| contentUrl | string      | `https://forms.office.com/Pages/TeamsDesignPage.aspx?Host=Teams&lang={locale}&groupId={groupId}&tid={tid}&teamsTheme={theme}&upn={upn}&fragment=FormId%3D{formId}`, wobei {formId} gleich der Entitäts-ID ist und {locale}, {groupId}, {tid} und {upn} Literale darstellen.   |
| removeUrl  | string      | Null                                                     |
| websiteUrl | string      |  `https://forms.office.com`    |

## <a name="word-excel-powerpoint-and-pdf-tabs"></a>Word-, Excel-, PowerPoint- und PDF-Registerkarten

In der folgenden Tabelle ist die `teamsAppId` für die einzelnen Apps aufgelistet.

| App   | teamsAppId | Typ (Erweiterung)                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| Word | `com.microsoft.teamspace.tab.file.staticviewer.word` | `docx` |
| Excel | `com.microsoft.teamspace.tab.file.staticviewer.excel` | `xlsx` |
| PowerPoint  | `com.microsoft.teamspace.tab.file.staticviewer.powerpoint` | `pptx` |
| PDF | `com.microsoft.teamspace.tab.file.staticviewer.pdf` | `pdf` |

Konfiguration wird nicht unterstützt.

## <a name="wiki-tabs"></a>Wiki-Registerkarten

Für Wiki-Registerkarten ist die `teamsAppId` `com.microsoft.teamspace.tab.wiki`.
Wiki-Registerkarten unterstützen die Konfiguration mithilfe von Graph nicht.
Beachten Sie aber, dass es auch nicht viel zu konfigurieren gibt – auf einer nicht konfigurierten Wiki-Registerkarte muss der erste Benutzer lediglich auf **Registerkarte einrichten** klicken, um sie zu konfigurieren.

## <a name="document-library-tabs"></a>Registerkarten der Dokumentbibliothek

Für Registerkarten der Dokumentbibliothek ist die `teamsAppId` `com.microsoft.teamspace.tab.files.sharepoint`. Konfiguration wird nicht unterstützt.

## <a name="onenote-tabs"></a>OneNote-Registerkarten

Für OneNote-Registerkarten ist die `teamsAppId` `0d820ecd-def2-4297-adad-78056cde7c78`. Die folgende Tabelle zeigt die Konfiguration.

| Eigenschaft   | Typ        | Beschreibung                                              |
| ---------- | ----------- | -------------------------------------------------------- |
| entityId   | string      | `{randomGuid}_{notebookId}`, wobei {randomGuid} eine von Ihnen generierte GUID ist.                                      |
| contentUrl | string      | Eine URL der Form `https://www.onenote.com/teams/TabContent?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`, wobei `{sectionsUrl}`, `{notebookId}` und `{oneNoteWebUrl}` in [GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta) zu finden sind. Schrägstrichen müssen Escapezeichen vorangestellt werden. {locale} und {tid} sind Literale. |
| removeUrl  | string      | Eine URL der Form `https://www.onenote.com/teams/TabRemove?entityid=%7BentityId%7D&subentityid=%7BsubEntityId%7D&auth_upn=%7Bupn%7D&notebookSource=New&notebookSelfUrl=https%3A%2F%2Fwww.onenote.com%2Fapi%2Fv1.0%2FmyOrganization%2Fgroups%2F{sectionsUrl}%2Fnotes%2Fnotebooks%2F{notebookId}&oneNoteWebUrl={oneNoteWebUrl}&notebookName=note&ui={locale}&tenantId={tid}`, wobei `{sectionsUrl}`, `{notebookId}` und `{oneNoteWebUrl}` in [GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta) zu finden sind. Schrägstrichen müssen Escapezeichen vorangestellt werden. {locale} und {tid} sind Literale. |
| websiteUrl | string      | Eine URL der Form `https://www.onenote.com/teams/TabRedirect?redirectUrl={oneNoteWebUrl}`, wobei `oneNoteWebUrl` in [GET /groups/{id}/onenote/notebooks](/graph/api/onenote-list-notebooks?view=graph-rest-beta) zu finden ist. |

## <a name="power-bi-tabs"></a>Power BI-Registerkarten

Für Power BI-Registerkarten ist `teamsAppId` `com.microsoft.teamspace.tab.powerbi`.
Konfiguration wird nicht unterstützt.

## <a name="sharepoint-page-and-list-tabs"></a>Registerkarten von SharePoint-Seiten und -Listen

Für Registerkarten von SharePoint-Seiten und -Listen ist die `teamsAppId` `2a527703-1f6f-4559-a332-d8a7d288cd88`.
Konfiguration wird nicht unterstützt.
Wenn Konfiguration gewünscht wird, erwägen Sie die Verwendung einer Website-Registerkarte.
