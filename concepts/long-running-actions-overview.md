---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
ms.topic: conceptual
ms.openlocfilehash: 687ed04d3ddcede391e9f16a2046cb186a093323
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092204"
---
# <a name="working-with-long-running-actions-beta"></a><span data-ttu-id="7d241-101">Arbeiten mit langen Aktionen (Beta)</span><span class="sxs-lookup"><span data-stu-id="7d241-101">Working with long running actions (beta)</span></span>

> <span data-ttu-id="7d241-102">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="7d241-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d241-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7d241-103">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d241-104">Die Abfrage einiger API-Antworten kann unbestimmte Zeit dauern.</span><span class="sxs-lookup"><span data-stu-id="7d241-104">Some API responses require indeterminate time to complete.</span></span>
<span data-ttu-id="7d241-105">Anstatt zu warten, bis der Vorgang abgeschlossen ist und Sie eine Antwort erhalten, können Sie das lange ausgeführte Aktionsmuster von Microsoft Graph verwenden.</span><span class="sxs-lookup"><span data-stu-id="7d241-105">Instead of waiting until the action is complete before returning a response, Microsoft Graph may use a long running actions pattern.</span></span>
<span data-ttu-id="7d241-106">Bei der Verwendung dieses Musters verfügt die App über eine Wartezeit für die Abfrage von Statusupdates für lange ausgeführte Aktionen, wobei Anforderungen nicht auf den Abschluss der Aktion warten müssen.</span><span class="sxs-lookup"><span data-stu-id="7d241-106">This pattern provides your app a wait to poll for status updates on a long running action, without any request waiting for the action to complete.</span></span>

<span data-ttu-id="7d241-107">Das allgemeine Muster umfasst die folgenden Schritte:</span><span class="sxs-lookup"><span data-stu-id="7d241-107">The general pattern follows these steps:</span></span>

1. <span data-ttu-id="7d241-108">Die App fordert eine lange ausgeführte Aktion über die API an.</span><span class="sxs-lookup"><span data-stu-id="7d241-108">Your app requests a long running action via the API.</span></span> <span data-ttu-id="7d241-109">Die API akzeptiert die Aktion und gibt eine `202 Accepted`-Antwort zusammen mit einem Speicherortheader für die API-URL zum Abrufen von Statusberichten zur Aktion zurück.</span><span class="sxs-lookup"><span data-stu-id="7d241-109">The API accepts the action and returns a `202 Accepted` response along with a Location header for the API URL to retrieve action status reports.</span></span>
2. <span data-ttu-id="7d241-110">Die App fordert die Statusberichts-URL zur Aktion an und empfängt eine [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta)-Antwort mit dem Fortschritt der lange ausgeführten Aktion.</span><span class="sxs-lookup"><span data-stu-id="7d241-110">Your app requests the action status report URL and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response with the progress of the long running action.</span></span>
3. <span data-ttu-id="7d241-111">Die lange ausgeführte Aktion wird abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="7d241-111">The long running action completes.</span></span> 
4. <span data-ttu-id="7d241-112">Ihre App fordert erneut die Statusberichts-URL zur Aktion an und empfängt eine [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta)-Antwort über den Abschluss der lange ausgeführten Aktion.</span><span class="sxs-lookup"><span data-stu-id="7d241-112">Your app requests the action status report URL again and receives an [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) response showing the completion of the action.</span></span>

## <a name="initial-action-request"></a><span data-ttu-id="7d241-113">Anfängliche Aktionsanforderung</span><span class="sxs-lookup"><span data-stu-id="7d241-113">Initial action request</span></span>

<span data-ttu-id="7d241-114">Lassen Sie uns die einzelnen Schritte für ein Beispiel eines [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta)-Szenarios durchgehen.</span><span class="sxs-lookup"><span data-stu-id="7d241-114">Let's walk through the steps for an example [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta) scenario.</span></span>
<span data-ttu-id="7d241-115">In diesem Szenario fordert eine App das Kopieren eines Ordners mit einer großen Menge enthaltener Daten an.</span><span class="sxs-lookup"><span data-stu-id="7d241-115">In this scenario, your app requests to copy a folder that contains a large amount of data.</span></span>
<span data-ttu-id="7d241-116">Das Abschließen dieser Anforderung wird wahrscheinlich einige Sekunden dauern, da die Datenmenge groß ist.</span><span class="sxs-lookup"><span data-stu-id="7d241-116">This request will likely take several seconds to complete since the amount of data is large.</span></span>

<!-- { "blockType": "request", "name": "lro-copy-item-example", "scopes": "files.readwrite" } -->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{folder-item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "Copy of LargeFolder1"
}
```

<span data-ttu-id="7d241-117">Die API antwortet, dass die Aktion akzeptiert wurde, und gibt die URL zum Abrufen des Status der lange ausgeführten Aktion zurück.</span><span class="sxs-lookup"><span data-stu-id="7d241-117">The API responds that the action was accepted and the URL for retrieving the status of the long running action.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="7d241-118">**Hinweis:** Die zurückgegebene URL des Speicherorts befindet sich möglicherweise nicht auf dem Microsoft Graph-API-Endpunkt.</span><span class="sxs-lookup"><span data-stu-id="7d241-118">**Note:** The location URL returned may not be on the Microsoft Graph API endpoint.</span></span>

<span data-ttu-id="7d241-119">In vielen Fällen ist dies das Ende der Anforderung, da der Kopiervorgang abgeschlossen wird, ohne dass die App weitere Aufgaben ausführt.</span><span class="sxs-lookup"><span data-stu-id="7d241-119">In many cases this may be the end of the request, since the copy action will complete without the app doing any additional work.</span></span>
<span data-ttu-id="7d241-120">Wenn die App jedoch den Status des Kopiervorgangs anzeigen oder sicherstellen muss, dass dieser ohne Fehler abgeschlossen wird, kann sie dazu die Überwachungs-URL verwenden.</span><span class="sxs-lookup"><span data-stu-id="7d241-120">However, if your app needs to show the status of the copy action or ensure that it completes without error, it can do so using the monitor URL.</span></span>

## <a name="retrieve-a-status-report-from-the-monitor-url"></a><span data-ttu-id="7d241-121">Abrufen eines Statusberichts von der Überwachungs-URL</span><span class="sxs-lookup"><span data-stu-id="7d241-121">Retrieve a status report from the monitor URL</span></span>

<span data-ttu-id="7d241-122">Um den Status des Kopiervorgang zu überprüfen, stellt die App eine Anforderung an die URL, die in der vorherigen Antwort bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="7d241-122">To check on the status of the copy action, the app makes a request to the URL provided in the previous response.</span></span>
<span data-ttu-id="7d241-123">*Hinweis:* Diese Anforderung erfordert keine Authentifizierung, da die URL kurzlebig und einzigartig für den ursprünglichen Aufrufer ist.</span><span class="sxs-lookup"><span data-stu-id="7d241-123">*Note:* This request does not require authentication, since the URL is short-lived and unique to the original caller.</span></span> 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="7d241-124">Der Dienst gibt eine Antwort mit der Information zurück, dass die lang ausgeführte Aktion noch nicht abgeschlossen ist:</span><span class="sxs-lookup"><span data-stu-id="7d241-124">The service responses with information that the long running action is still in progress:</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
  "operation": "ItemCopy",
  "percentageComplete": 27.8,
  "status": "inProgress"
}
```

<span data-ttu-id="7d241-125">Diese Information kann verwendet werden, um den Benutzer über den Fortschritt des Kopiervorgangs zu informieren.</span><span class="sxs-lookup"><span data-stu-id="7d241-125">This information can be used to provide an update to the user about the progress of the copy action.</span></span>
<span data-ttu-id="7d241-126">Die App kann die Überwachungs-URL weiterhin abfragen, um Statusupdates anzufordern und den Fortschritt der Aktion nachzuverfolgen.</span><span class="sxs-lookup"><span data-stu-id="7d241-126">The app can continue to poll the monitor URL to request status updates and keep track of the progress of the action.</span></span>

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a><span data-ttu-id="7d241-127">Abrufen eines Statusberichts zum Abschluss von der Überwachungs-URL</span><span class="sxs-lookup"><span data-stu-id="7d241-127">Retrieve a completed status report from the monitor URL</span></span>

<span data-ttu-id="7d241-128">Nach einigen Sekunden ist der Kopiervorgang abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="7d241-128">After a few seconds the copy operation has completed.</span></span>
<span data-ttu-id="7d241-129">Wenn die App nun die Überwachungs-URL abfragt, ist die Antwort eine Weiterleitung zum Endergebnis der Aktion.</span><span class="sxs-lookup"><span data-stu-id="7d241-129">This time when the app makes a request to the monitor URL the response is a redirection to the finished result of the action.</span></span>

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="7d241-130">Wenn die Aktion ausgeführt wurde, gibt die Antwort des Überwachungsdienstes die resourceId für die Ergebnisse zurück.</span><span class="sxs-lookup"><span data-stu-id="7d241-130">When the action has completed, the response from the monitor service will return the resourceId for the results.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "percentageComplete": 100.0,
    "resourceId": "01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM",
    "status": "completed"
}
```

## <a name="retrieve-the-results-of-the-completed-operation"></a><span data-ttu-id="7d241-131">Abrufen der Ergebnisse des abgeschlossenen Vorgangs</span><span class="sxs-lookup"><span data-stu-id="7d241-131">Retrieve the results of the completed operation</span></span>

<span data-ttu-id="7d241-132">Nachdem der Auftrag abgeschlossen wurde, gibt die Überwachungs-URL die Ressourcen-ID des Ergebnisses zurück, in diesem Fall die neue Kopie des ursprünglichen Elements.</span><span class="sxs-lookup"><span data-stu-id="7d241-132">Once the job has completed, the monitor URL returns the resourceId of the result, in this case the new copy of the original item.</span></span>
<span data-ttu-id="7d241-133">Sie können dieses neue Element mithilfe der Ressourcen-ID ansprechen. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="7d241-133">You can address this new item using the resourceId, for example:</span></span>

<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "",
    "name": "Copy of LargeFolder1",
    "folder": { },
    "size": 12019
}
```

## <a name="supported-resources"></a><span data-ttu-id="7d241-134">Unterstützte Ressourcen</span><span class="sxs-lookup"><span data-stu-id="7d241-134">Supported resources</span></span>

<span data-ttu-id="7d241-135">Lange ausgeführte Aktionen werden für die folgenden API-Methoden API unterstützt:</span><span class="sxs-lookup"><span data-stu-id="7d241-135">Long running actions are supported on the following API methods</span></span>

| <span data-ttu-id="7d241-136">**Ressource**</span><span class="sxs-lookup"><span data-stu-id="7d241-136">**Resource**</span></span> | <span data-ttu-id="7d241-137">**API**</span><span class="sxs-lookup"><span data-stu-id="7d241-137">**API**</span></span> |
|:------ | :------ |
| <span data-ttu-id="7d241-138">DriveItem</span><span class="sxs-lookup"><span data-stu-id="7d241-138">DriveItem</span></span> | [<span data-ttu-id="7d241-139">Copy</span><span class="sxs-lookup"><span data-stu-id="7d241-139">Copy</span></span>](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a><span data-ttu-id="7d241-140">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="7d241-140">Prerequisites</span></span>

<span data-ttu-id="7d241-141">Die gleichen [Berechtigungen](./permissions-reference.md), die für die Ausführung einer lange ausgeführten Aktion erforderlich sind, sind ebenfalls erforderlich, um den Status einer lange ausgeführten Aktion abzufragen.</span><span class="sxs-lookup"><span data-stu-id="7d241-141">The same [permissions](./permissions-reference.md) that are required to perform a long running action are also required to query the status of a long running action.</span></span>




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "suppressions": [
    "Error: lro-check-status:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus",
    "Error: lro-check-status-complete:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus"
  ],
  "tocPath": "Concepts/Long running actions"
} -->
