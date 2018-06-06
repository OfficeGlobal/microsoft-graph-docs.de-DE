---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
ms.topic: conceptual
ms.openlocfilehash: 30f98afa7b75784b0ee2b9ec446c6389cc876949
ms.sourcegitcommit: af8fdd5ea762fb54b7fbebb9a70bd942a56c6b7a
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/25/2018
ms.locfileid: "19473153"
---
# <a name="working-with-long-running-actions-beta"></a><span data-ttu-id="b9d1d-101">Arbeiten mit langen Aktionen (Beta)</span><span class="sxs-lookup"><span data-stu-id="b9d1d-101">Working with long running actions (beta)</span></span>

> <span data-ttu-id="b9d1d-102">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-102">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b9d1d-103">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-103">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b9d1d-104">Die Abfrage einiger API-Antworten kann unbestimmte Zeit dauern.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-104">Some API responses require indeterminate time to complete.</span></span>
<span data-ttu-id="b9d1d-105">Anstatt zu warten, bis der Vorgang abgeschlossen ist und Sie eine Antwort erhalten, können Sie das lange ausgeführte Aktionsmuster von Microsoft Graph verwenden.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-105">Instead of waiting until the action is complete before returning a response, Microsoft Graph may use a long running actions pattern.</span></span>
<span data-ttu-id="b9d1d-106">Bei der Verwendung dieses Musters verfügt die App über eine Wartezeit für die Abfrage von Statusupdates für lange ausgeführte Aktionen, wobei Anforderungen nicht auf den Abschluss der Aktion warten müssen.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-106">This pattern provides your app a wait to poll for status updates on a long running action, without any request waiting for the action to complete.</span></span>

<span data-ttu-id="b9d1d-107">Das allgemeine Muster umfasst die folgenden Schritte:</span><span class="sxs-lookup"><span data-stu-id="b9d1d-107">The general pattern follows these steps:</span></span>

1. <span data-ttu-id="b9d1d-108">Die App fordert eine lange ausgeführte Aktion über die API an.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-108">Your app requests a long running action via the API.</span></span> <span data-ttu-id="b9d1d-109">Die API akzeptiert die Aktion und gibt eine `202 Accepted`-Antwort zusammen mit einem Speicherortheader für die API-URL zum Abrufen von Statusberichten zur Aktion zurück.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-109">The API accepts the action and returns a `202 Accepted` response along with a Location header for the API URL to retrieve action status reports.</span></span>
2. <span data-ttu-id="b9d1d-110">Die App fordert die Statusberichts-URL zur Aktion an und empfängt eine [AsyncJobStatus](../api-reference/beta/resources/asyncjobstatus.md)-Antwort mit dem Fortschritt der lange ausgeführten Aktion.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-110">Your app requests the action status report URL and receives an [AsyncJobStatus](../api-reference/beta/resources/asyncjobstatus.md) response with the progress of the long running action.</span></span>
3. <span data-ttu-id="b9d1d-111">Die lange ausgeführte Aktion wird abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-111">The long running action completes.</span></span> 
4. <span data-ttu-id="b9d1d-112">Ihre App fordert erneut die Statusberichts-URL zur Aktion an und empfängt eine [AsyncJobStatus](../api-reference/beta/resources/asyncjobstatus.md)-Antwort über den Abschluss der lange ausgeführten Aktion.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-112">Your app requests the action status report URL again and receives an [AsyncJobStatus](../api-reference/beta/resources/asyncjobstatus.md) response showing the completion of the action.</span></span>

## <a name="initial-action-request"></a><span data-ttu-id="b9d1d-113">Anfängliche Aktionsanforderung</span><span class="sxs-lookup"><span data-stu-id="b9d1d-113">Initial action request</span></span>

<span data-ttu-id="b9d1d-114">Lassen Sie uns die einzelnen Schritte für ein Beispiel eines [DriveItem Copy](../api-reference/beta/api/driveitem_copy.md)-Szenarios durchgehen.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-114">Let's walk through the steps for an example [DriveItem Copy](../api-reference/beta/api/driveitem_copy.md) scenario.</span></span>
<span data-ttu-id="b9d1d-115">In diesem Szenario fordert eine App das Kopieren eines Ordners mit einer großen Menge enthaltener Daten an.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-115">In this scenario, your app requests to copy a folder that contains a large amount of data.</span></span>
<span data-ttu-id="b9d1d-116">Das Abschließen dieser Anforderung wird wahrscheinlich einige Sekunden dauern, da die Datenmenge groß ist.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-116">This request will likely take several seconds to complete since the amount of data is large.</span></span>

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

<span data-ttu-id="b9d1d-117">Die API antwortet, dass die Aktion akzeptiert wurde, und gibt die URL zum Abrufen des Status der lange ausgeführten Aktion zurück.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-117">The API responds that the action was accepted and the URL for retrieving the status of the long running action.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="b9d1d-118">**Hinweis:** Die zurückgegebene URL des Speicherorts befindet sich möglicherweise nicht auf dem Microsoft Graph-API-Endpunkt.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-118">**Note:** The location URL returned may not be on the Microsoft Graph API endpoint.</span></span>

<span data-ttu-id="b9d1d-119">In vielen Fällen ist dies das Ende der Anforderung, da der Kopiervorgang abgeschlossen wird, ohne dass die App weitere Aufgaben ausführt.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-119">In many cases this many be the end of the request, since the copy action will complete without the app doing any additional work.</span></span>
<span data-ttu-id="b9d1d-120">Wenn die App jedoch den Status des Kopiervorgangs anzeigen oder sicherstellen muss, dass dieser ohne Fehler abgeschlossen wird, kann sie dazu die Überwachungs-URL verwenden.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-120">However, if your app needs to show the status of the copy action or ensure that it completes without error, it can do so using the monitor URL.</span></span>

## <a name="retrieve-a-status-report-from-the-monitor-url"></a><span data-ttu-id="b9d1d-121">Abrufen eines Statusberichts von der Überwachungs-URL</span><span class="sxs-lookup"><span data-stu-id="b9d1d-121">Retrieve a status report from the monitor URL</span></span>

<span data-ttu-id="b9d1d-122">Um den Status des Kopiervorgang zu überprüfen, stellt die App eine Anforderung an die URL, die in der vorherigen Antwort bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-122">To check on the status of the copy action, the app makes a request to the URL provided in the previous response.</span></span>
<span data-ttu-id="b9d1d-123">*Hinweis:* Diese Anforderung erfordert keine Authentifizierung, da die URL kurzlebig und einzigartig für den ursprünglichen Aufrufer ist.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-123">*Note:* This request does not require authentication, since the URL is short-lived and unique to the original caller.</span></span> 

<!-- { "blockType": "request", "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="b9d1d-124">Der Dienst gibt eine Antwort mit der Information zurück, dass die lang ausgeführte Aktion noch nicht abgeschlossen ist:</span><span class="sxs-lookup"><span data-stu-id="b9d1d-124">The service responses with information that the long running action is still in progress:</span></span>

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

<span data-ttu-id="b9d1d-125">Diese Information kann verwendet werden, um den Benutzer über den Fortschritt des Kopiervorgangs zu informieren.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-125">This information can be used to provide an update to the user about the progress of the copy action.</span></span>
<span data-ttu-id="b9d1d-126">Die App kann die Überwachungs-URL weiterhin abfragen, um Statusupdates anzufordern und den Fortschritt der Aktion nachzuverfolgen.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-126">The app can continue to poll the monitor URL to request status updates and keep track of the progress of the action.</span></span>

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a><span data-ttu-id="b9d1d-127">Abrufen eines Statusberichts zum Abschluss von der Überwachungs-URL</span><span class="sxs-lookup"><span data-stu-id="b9d1d-127">Retrieve a completed status report from the monitor URL</span></span>

<span data-ttu-id="b9d1d-128">Nach einigen Sekunden ist der Kopiervorgang abgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-128">After a few seconds the copy operation has completed.</span></span>
<span data-ttu-id="b9d1d-129">Wenn die App nun die Überwachungs-URL abfragt, ist die Antwort eine Weiterleitung zum Endergebnis der Aktion.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-129">This time when the app makes a request to the monitor URL the response is a redirection to the finished result of the action.</span></span>

<!-- { "blockType": "request", "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

<span data-ttu-id="b9d1d-130">Wenn die Aktion ausgeführt wurde, gibt die Antwort des Überwachungsdienstes die resourceId für die Ergebnisse zurück.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-130">When the action has completed, the response from the monitor service will return the resourceId for the results.</span></span>

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

## <a name="retrieve-the-results-of-the-completed-operation"></a><span data-ttu-id="b9d1d-131">Abrufen der Ergebnisse des abgeschlossenen Vorgangs</span><span class="sxs-lookup"><span data-stu-id="b9d1d-131">Retrieve the results of the completed operation</span></span>

<span data-ttu-id="b9d1d-132">Nachdem der Auftrag abgeschlossen wurde, gibt die Überwachungs-URL die Ressourcen-ID des Ergebnisses zurück, in diesem Fall die neue Kopie des ursprünglichen Elements.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-132">Once the job has completed, the monitor URL returns the resourceId of the result, in this case the new copy of the original item.</span></span>
<span data-ttu-id="b9d1d-133">Sie können dieses neue Element mithilfe der Ressourcen-ID ansprechen. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="b9d1d-133">You can address this new item using the resourceId, for example:</span></span>

<!-- { "blockType": "request", "name": "lro-copy-item-example-complete", "scopes": "files.readwrite" } -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem" } -->

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

## <a name="supported-resources"></a><span data-ttu-id="b9d1d-134">Unterstützte Ressourcen</span><span class="sxs-lookup"><span data-stu-id="b9d1d-134">Supported resources</span></span>

<span data-ttu-id="b9d1d-135">Lange ausgeführte Aktionen werden für die folgenden API-Methoden API unterstützt:</span><span class="sxs-lookup"><span data-stu-id="b9d1d-135">Long running actions are supported on the following API methods</span></span>

| <span data-ttu-id="b9d1d-136">**Ressource**</span><span class="sxs-lookup"><span data-stu-id="b9d1d-136">**Resource**</span></span> | <span data-ttu-id="b9d1d-137">**API**</span><span class="sxs-lookup"><span data-stu-id="b9d1d-137">**API**</span></span> |
|:------ | :------ |
| <span data-ttu-id="b9d1d-138">DriveItem</span><span class="sxs-lookup"><span data-stu-id="b9d1d-138">DriveItem</span></span> | [<span data-ttu-id="b9d1d-139">Copy</span><span class="sxs-lookup"><span data-stu-id="b9d1d-139">Copy</span></span>](../api-reference/beta/api/driveitem_copy.md) |

## <a name="prerequisites"></a><span data-ttu-id="b9d1d-140">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="b9d1d-140">Prerequisites</span></span>

<span data-ttu-id="b9d1d-141">Die gleichen [Berechtigungen](./permissions_reference.md), die für die Ausführung einer lange ausgeführten Aktion erforderlich sind, sind ebenfalls erforderlich, um den Status einer lange ausgeführten Aktion abzufragen.</span><span class="sxs-lookup"><span data-stu-id="b9d1d-141">The same [permissions](./permissions_reference.md) that are required to perform a long running action are also required to query the status of a long running action.</span></span>




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "tocPath": "Concepts/Long running actions"
} -->
