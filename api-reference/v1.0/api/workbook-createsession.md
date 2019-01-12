---
title: Sitzung erstellen
description: 'Verwenden Sie diese API zum Erstellen einer neuen Arbeitsmappensitzung. '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 9a377c4bb86f468e9e6107e451b40494665f5b16
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972817"
---
# <a name="create-session"></a><span data-ttu-id="4ef1a-103">Sitzung erstellen</span><span class="sxs-lookup"><span data-stu-id="4ef1a-103">Create Session</span></span>

<span data-ttu-id="4ef1a-104">Verwenden Sie diese API zum Erstellen einer neuen Arbeitsmappensitzung.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-104">Use this API to create a new workbook session.</span></span> 

<span data-ttu-id="4ef1a-105">Excel-APIs können in einem der beiden folgenden Modi aufgerufen werden:</span><span class="sxs-lookup"><span data-stu-id="4ef1a-105">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="4ef1a-p101">Beständige Sitzung: Alle an der Arbeitsmappe vorgenommenen Änderungen werden gespeichert. Dies ist die übliche Vorgehensweise.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="4ef1a-p102">Nicht beständige Sitzung: Die von der API vorgenommenen Änderungen werden nicht am Quellspeicherort gespeichert. Stattdessen behält der Excel-Back-End-Server eine temporäre Kopie der Datei  bei, welche die während dieser API-Sitzung vorgenommenen Änderungen enthält. Wenn die Excel-Sitzung abläuft, gehen die Änderungen verloren. Dieser Modus eignet sich für Apps, die Analysen durchführen oder die Ergebnisse einer Berechnung oder eines Diagrammbilds abrufen, aber nicht den Dokumentstatus betreffen.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="4ef1a-112">Um die Sitzung in der API darzustellen, verwenden Sie den `workbook-session-id: {session-id}`-Header.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-112">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="4ef1a-p103">**Hinweis:** Der Sitzungsheader ist für das Funktionieren einer Excel-API nicht erforderlich. Die Verwendung des Sitzungsheaders wird jedoch empfohlen, um die Leistung zu verbessern. Wenn Sie keinen Sitzungsheader verwenden, _werden_ die während des API-Aufrufs vorgenommenen Änderungen in der Datei gespeichert.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="error-handling"></a><span data-ttu-id="4ef1a-116">Fehlerbehandlung</span><span class="sxs-lookup"><span data-stu-id="4ef1a-116">Error Handling</span></span>

<span data-ttu-id="4ef1a-117">Bei dieser Anforderung tritt gelegentlich der 504 HTTP-Fehler auf.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-117">This request might occasionally receive a 504 HTTP error.</span></span> <span data-ttu-id="4ef1a-118">Sollte dieser Fehler auftreten,  wiederholen Sie die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-118">The appropriate response to this error is to repeat the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="4ef1a-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4ef1a-119">Permissions</span></span>
<span data-ttu-id="4ef1a-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4ef1a-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ef1a-122">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="4ef1a-122">Permission type</span></span>      | <span data-ttu-id="4ef1a-123">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="4ef1a-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4ef1a-124">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="4ef1a-124">Delegated (work or school account)</span></span> | <span data-ttu-id="4ef1a-125">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="4ef1a-125">Files.ReadWrite</span></span>    |
|<span data-ttu-id="4ef1a-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="4ef1a-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4ef1a-127">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ef1a-127">Not supported.</span></span>    |
|<span data-ttu-id="4ef1a-128">Anwendung</span><span class="sxs-lookup"><span data-stu-id="4ef1a-128">Application</span></span> | <span data-ttu-id="4ef1a-129">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="4ef1a-129">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4ef1a-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ef1a-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession

```
## <a name="request-headers"></a><span data-ttu-id="4ef1a-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="4ef1a-131">Request headers</span></span>
| <span data-ttu-id="4ef1a-132">Name</span><span class="sxs-lookup"><span data-stu-id="4ef1a-132">Name</span></span>       | <span data-ttu-id="4ef1a-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="4ef1a-133">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4ef1a-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ef1a-134">Authorization</span></span>  | <span data-ttu-id="4ef1a-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4ef1a-137">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="4ef1a-137">Request body</span></span>
<span data-ttu-id="4ef1a-138">Geben Sie im Anforderungstext eine JSON-Darstellung des [WorkbookSessionInfo](../resources/workbooksessioninfo.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-138">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4ef1a-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ef1a-139">Response</span></span>

<span data-ttu-id="4ef1a-140">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und ein [WorkbookSessionInfo](../resources/workbooksessioninfo.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-140">If successful, this method returns `201 Created` response code and [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ef1a-141">Beispiel</span><span class="sxs-lookup"><span data-stu-id="4ef1a-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4ef1a-142">Anforderung</span><span class="sxs-lookup"><span data-stu-id="4ef1a-142">Request</span></span>
<span data-ttu-id="4ef1a-143">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistChanges": true
}
```
<span data-ttu-id="4ef1a-144">Geben Sie im Anforderungstext eine JSON-Darstellung des [WorkbookSessionInfo](../resources/workbooksessioninfo.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-144">In the request body, supply a JSON representation of [WorkbookSessionInfo](../resources/workbooksessioninfo.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="4ef1a-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="4ef1a-145">Response</span></span>
<span data-ttu-id="4ef1a-p107">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="4ef1a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistChanges": true
}
```

