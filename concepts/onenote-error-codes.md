---
title: Fehlercodes für OneNote-APIs in Microsoft Graph
description: Dieser Artikel beschreibt Fehlercodes, die von der OneNote-API zurückgegeben werden, wenn eine von der API gesendete Anfrage fehlschlägt.
ms.openlocfilehash: 265929be081ee61a88b8baf4f600e2c154797ec7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092265"
---
# <a name="error-codes-for-onenote-apis-in-microsoft-graph"></a><span data-ttu-id="270f9-103">Fehlercodes für OneNote-APIs in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="270f9-103">Error codes for OneNote APIs in Microsoft Graph</span></span>

<span data-ttu-id="270f9-104">Dieser Artikel beschreibt Fehlercodes, die von der OneNote-API zurückgegeben werden, wenn eine von der API gesendete Anfrage fehlschlägt.</span><span class="sxs-lookup"><span data-stu-id="270f9-104">This article describes error codes that are returned by the OneNote APIs in Microsoft Graph whenever a request sent through the API fails.</span></span>

## <a name="error-response-example"></a><span data-ttu-id="270f9-105">Fehlerantwort-Beispiel</span><span class="sxs-lookup"><span data-stu-id="270f9-105">Error response example</span></span>

<span data-ttu-id="270f9-106">Wenn Ihre Anforderung einen Fehler generiert, hält die OneNote-API die Ausführung der Anforderung an und gibt eine Fehlerantwort als JSON-Objekt zurück.</span><span class="sxs-lookup"><span data-stu-id="270f9-106">When your request generates an error, the OneNote API stops performing the request and returns an error response as a JSON object.</span></span> <span data-ttu-id="270f9-107">Eine Fehlerantwort enthält den zugehörigen Fehlercode, eine Nachricht und einen Link zum entsprechenden Abschnitt dieses Artikels.</span><span class="sxs-lookup"><span data-stu-id="270f9-107">An error response contains the associated error code, a message, and a link to the appropriate section of this article.</span></span> <span data-ttu-id="270f9-108">Im folgenden Beispiel wird eine Fehlerantwort veranschaulicht.</span><span class="sxs-lookup"><span data-stu-id="270f9-108">The following example shows how an error response looks.</span></span>

```json
{
   "error":{
      "code":"10002",
      "message":"The service is currently unavailable. Please try again later.",
      "innerError": {
        "requestId": "request-id",
        "date": "date-time"
      }
   }
}
```

<span data-ttu-id="270f9-109">Weitere Informationen zu Microsoft Graph-Fehlern finden Sie unter [Microsoft Graph-Fehlerantworten und Ressourcentypen](errors.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-109">For more information about Microsoft Graph errors, see [Microsoft Graph error responses and resource types](errors.md).</span></span>

## <a name="codes-from-10001-to-19999"></a><span data-ttu-id="270f9-110">Codes von 10001-19999</span><span class="sxs-lookup"><span data-stu-id="270f9-110">Codes from 10001 to 19999</span></span>

<span data-ttu-id="270f9-111">Der Dienst hat Probleme oder sendet Informationen zur Anwendung.</span><span class="sxs-lookup"><span data-stu-id="270f9-111">The service is having problems or is sending information to the application.</span></span>

### <a name="10001"></a><span data-ttu-id="270f9-112">10001</span><span class="sxs-lookup"><span data-stu-id="270f9-112">10001</span></span>
<span data-ttu-id="270f9-113">Ein unerwarteter Fehler ist aufgetreten, und die Anforderung ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="270f9-113">An unexpected error occurred and the request failed.</span></span>

### <a name="10002"></a><span data-ttu-id="270f9-114">10002</span><span class="sxs-lookup"><span data-stu-id="270f9-114">10002</span></span>
<span data-ttu-id="270f9-115">Der Dienst ist derzeit nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="270f9-115">The service is not currently available.</span></span>

### <a name="10003"></a><span data-ttu-id="270f9-116">10003</span><span class="sxs-lookup"><span data-stu-id="270f9-116">10003</span></span>
<span data-ttu-id="270f9-117">Das Konto des aktuellen Benutzers hat die Maximalanzahl an aktiven Anforderungen überschritten.</span><span class="sxs-lookup"><span data-stu-id="270f9-117">The current user's account has exceeded the maximum number of active requests.</span></span> <span data-ttu-id="270f9-118">Ihre App muss die Anforderung wiederholen.</span><span class="sxs-lookup"><span data-stu-id="270f9-118">Your app will have to repeat the request.</span></span>

### <a name="10004"></a><span data-ttu-id="270f9-119">10004</span><span class="sxs-lookup"><span data-stu-id="270f9-119">10004</span></span>
<span data-ttu-id="270f9-120">Der Dienst kann keine Seite im angeforderten Abschnitt erstellen, da der Abschnitt kennwortgeschützt ist.</span><span class="sxs-lookup"><span data-stu-id="270f9-120">The service can't create a page in the requested section because that section is protected by a password.</span></span>

### <a name="10005"></a><span data-ttu-id="270f9-121">10005</span><span class="sxs-lookup"><span data-stu-id="270f9-121">10005</span></span>
<span data-ttu-id="270f9-122">Die Anforderung enthält mehr als die Maximalanzahl an Bildtags, wobei das **data-render-src**-Attribut eine PDF enthält.</span><span class="sxs-lookup"><span data-stu-id="270f9-122">The request contains more than the maximum number of image tags in which the **data-render-src** attribute contains a PDF.</span></span> <span data-ttu-id="270f9-123">Siehe [Hinzufügen von Bildern und Dateien](onenote-images-files.md)</span><span class="sxs-lookup"><span data-stu-id="270f9-123">See [Add images and files](onenote-images-files.md).</span></span>

### <a name="10006"></a><span data-ttu-id="270f9-124">10006</span><span class="sxs-lookup"><span data-stu-id="270f9-124">10006</span></span>
<span data-ttu-id="270f9-125">Die OneNote-API konnte keine Seite im angegebenen Abschnitt erstellen, da dieser Abschnitt beschädigt ist.</span><span class="sxs-lookup"><span data-stu-id="270f9-125">The OneNote API was unable to create a page in the specified section because that section is corrupt.</span></span>

### <a name="10007"></a><span data-ttu-id="270f9-126">10007</span><span class="sxs-lookup"><span data-stu-id="270f9-126">10007</span></span>
<span data-ttu-id="270f9-p104">Der Server ist zu ausgelastet, um die eingehende Anforderung zu bearbeiten. Bitte versuchen Sie es später erneut.</span><span class="sxs-lookup"><span data-stu-id="270f9-p104">The server is too busy to handle the incoming request at this moment. Please try again later.</span></span>

### <a name="10008"></a><span data-ttu-id="270f9-129">10008</span><span class="sxs-lookup"><span data-stu-id="270f9-129">10008</span></span>
<span data-ttu-id="270f9-130">Eine oder mehrere der Dokumentbibliotheken des OneDrive-Benutzers oder der -Gruppe enthalten mehr als 5.000 OneDrive-Elemente (Notizbücher, Abschnitte, Abschnittsgruppen) und können nicht mithilfe der API abgefragt werden.</span><span class="sxs-lookup"><span data-stu-id="270f9-130">One or more of the document libraries on the user or group's OneDrive contains more than 5000 OneNote items (notebooks, sections, section groups), and cannot be queried using the API.</span></span> <span data-ttu-id="270f9-131">Stellen Sie sicher, dass keine der Benutzer- oder Gruppen-Dokumentbibliotheken mehr als 5.000 OneNote-Elemente enthält.</span><span class="sxs-lookup"><span data-stu-id="270f9-131">Please make sure that none of the user or group's document libraries contains more than 5000 OneNote items.</span></span> <span data-ttu-id="270f9-132">Im [OneNote-Entwicklerblog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) finden Sie Informationen zur Reduzierung der Elemente.</span><span class="sxs-lookup"><span data-stu-id="270f9-132">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10012"></a><span data-ttu-id="270f9-133">10012</span><span class="sxs-lookup"><span data-stu-id="270f9-133">10012</span></span>
<span data-ttu-id="270f9-134">Die Entität kann nicht erstellt oder aktualisiert werden, da aus der Bibliothek, die das Notizbuch enthält, Elemente ausgecheckt werden müssen, bevor diese bearbeitet werden können.</span><span class="sxs-lookup"><span data-stu-id="270f9-134">Unable to create or update the entity because the library that contains the notebook requires items to be checked out before they can be edited.</span></span> <span data-ttu-id="270f9-135">Weitere Informationen finden Sie unter [Einrichten einer Bibliothek, um das Auschecken von Dateien erforderlich zu machen](https://support.office.com/de-DE/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7).</span><span class="sxs-lookup"><span data-stu-id="270f9-135">For more information, see [Set up a library to require check-out of files](https://support.office.com/de-DE/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7).</span></span>

<span data-ttu-id="270f9-136">Entfernen Sie entweder die Anforderung zum Auschecken aus der Bibliothek oder verschieben Sie das Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="270f9-136">Either remove the check-out requirement from the library, or move the notebook.</span></span>

### <a name="10013"></a><span data-ttu-id="270f9-137">10013</span><span class="sxs-lookup"><span data-stu-id="270f9-137">10013</span></span>
<span data-ttu-id="270f9-p107">Eine oder mehrere Dokumentbibliotheken in OneDrive des Benutzers oder der Gruppe enthalten mehr als 20.000 Elemente und können nicht für das Abfragen mithilfe der API indiziert werden. Stellen Sie sicher, dass keine der Dokumentbibliotheken des Benutzers oder der Gruppe mehr als 20.000 Elemente enthält. Schritte zur Lösung des Problems finden Sie im [OneNote Developer-Blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/).</span><span class="sxs-lookup"><span data-stu-id="270f9-p107">One or more of the document libraries on the user or group's OneDrive contains more than 5000 OneNote items (notebooks, sections, section groups), and cannot be queried using the API. Please make sure that none of the user or group's document libraries contains more than 5000 OneNote items. See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10014"></a><span data-ttu-id="270f9-141">10014</span><span class="sxs-lookup"><span data-stu-id="270f9-141">10014</span></span>
<span data-ttu-id="270f9-142">Azure Key Vault ist zu ausgelastet, um die eingehende Anforderung zu bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="270f9-142">Azure Key Vault is too busy to handle the incoming request at this moment.</span></span> <span data-ttu-id="270f9-143">Versuchen Sie es später erneut.</span><span class="sxs-lookup"><span data-stu-id="270f9-143">Please try again later.</span></span>

### <a name="10015"></a><span data-ttu-id="270f9-144">10015</span><span class="sxs-lookup"><span data-stu-id="270f9-144">10015</span></span>
<span data-ttu-id="270f9-145">SharePoint ist derzeit nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="270f9-145">SharePoint is currently unavailable.</span></span> <span data-ttu-id="270f9-146">Versuchen Sie es später erneut.</span><span class="sxs-lookup"><span data-stu-id="270f9-146">Please try again later.</span></span>

### <a name="10016"></a><span data-ttu-id="270f9-147">10016</span><span class="sxs-lookup"><span data-stu-id="270f9-147">10016</span></span>
<span data-ttu-id="270f9-148">Die Dokumentbibliothek des OneDrive-Benutzers oder der -Gruppe hat den Sicherheitsschwellwert überschritten.</span><span class="sxs-lookup"><span data-stu-id="270f9-148">Document library on the user or group’s OneDrive exceeded unique security scopes threshold limit.</span></span> <span data-ttu-id="270f9-149">Der Sicherheitsschwellwert von 50.000 für die Bibliothek darf nicht überschritten werden.</span><span class="sxs-lookup"><span data-stu-id="270f9-149">The maximum number of unique security scopes set for a library cannot exceed 50,000.</span></span>

### <a name="10017"></a><span data-ttu-id="270f9-150">10017</span><span class="sxs-lookup"><span data-stu-id="270f9-150">10017</span></span>
<span data-ttu-id="270f9-151">Ungültige Anforderung.</span><span class="sxs-lookup"><span data-stu-id="270f9-151">Bad Request.</span></span>

### <a name="19999"></a><span data-ttu-id="270f9-152">19999</span><span class="sxs-lookup"><span data-stu-id="270f9-152">19999</span></span>
<span data-ttu-id="270f9-153">Die Anforderung ist fehlgeschlagen, da ein unbekannter Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="270f9-153">The request failed because an undetermined error occurred.</span></span>

## <a name="codes-from-20001-to-29999"></a><span data-ttu-id="270f9-154">Codes von 20001 bis 29999</span><span class="sxs-lookup"><span data-stu-id="270f9-154">Codes from 20001 to 29999</span></span>

<span data-ttu-id="270f9-155">Der Anwendungscode hat einen Fehler gemacht.</span><span class="sxs-lookup"><span data-stu-id="270f9-155">The application code has done something wrong.</span></span>

### <a name="20001"></a><span data-ttu-id="270f9-156">20001</span><span class="sxs-lookup"><span data-stu-id="270f9-156">20001</span></span>

<span data-ttu-id="270f9-157">In der Anforderung fehlt der erforderliche "Präsentation"-Teil.</span><span class="sxs-lookup"><span data-stu-id="270f9-157">The request is missing the required "Presentation" part.</span></span> <span data-ttu-id="270f9-158">Es ist einer erforderlich.</span><span class="sxs-lookup"><span data-stu-id="270f9-158">Exactly one is required.</span></span> 

### <a name="20002"></a><span data-ttu-id="270f9-159">20002</span><span class="sxs-lookup"><span data-stu-id="270f9-159">20002</span></span>
<span data-ttu-id="270f9-160">Die Anforderung enthält zwei oder mehr "Präsentation"-Teile.</span><span class="sxs-lookup"><span data-stu-id="270f9-160">The request contains two or more "Presentation" parts.</span></span> <span data-ttu-id="270f9-161">Es ist einer erforderlich.</span><span class="sxs-lookup"><span data-stu-id="270f9-161">Exactly one is required.</span></span>

### <a name="20003"></a><span data-ttu-id="270f9-162">20003</span><span class="sxs-lookup"><span data-stu-id="270f9-162">20003</span></span>
<span data-ttu-id="270f9-163">Der Inhaltstyp des "Präsentation"-Teils kann nur Text/HTML oder Anwendung/XHTML + XML sein.</span><span class="sxs-lookup"><span data-stu-id="270f9-163">The content type of the "Presentation" part can be only text/HTML or application/XHTML+XML.</span></span> 

### <a name="20004"></a><span data-ttu-id="270f9-164">20004</span><span class="sxs-lookup"><span data-stu-id="270f9-164">20004</span></span>
<span data-ttu-id="270f9-p113">Der HTML-Code des "Presentation"-Teils enthält ein Bildtag, bei dem sowohl die Eigenschaft **src** als auch die Eigenschaft **data-render-src** festgelegt ist. Die API ignoriert die Eigenschaft **src** und verwendet die Eigenschaft **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="270f9-p113">The "Presentation" part HTML contains an image tag with both the **src** and the **data-render-src** properties set. The API will ignore the **src** property and use the **data-render-src** property. See OneNote API reference.</span></span> 

### <a name="20005"></a><span data-ttu-id="270f9-167">20005</span><span class="sxs-lookup"><span data-stu-id="270f9-167">20005</span></span>
<span data-ttu-id="270f9-168">Die Anforderungs-URI ist zu lang.</span><span class="sxs-lookup"><span data-stu-id="270f9-168">The request URI is too long.</span></span> <span data-ttu-id="270f9-169">Der maximale Länge der Anforderungs-URI (einschließlich aller Parameter und Daten) beträgt 16 KB oder 16.384 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="270f9-169">The maximum size of the URI (including all parameters and data) is 16 KB or 16,384 characters.</span></span>

### <a name="20006"></a><span data-ttu-id="270f9-170">20006</span><span class="sxs-lookup"><span data-stu-id="270f9-170">20006</span></span>
<span data-ttu-id="270f9-171">Die „Presentation”-Teil-HTML enthält ein Bild-Tag, für das weder eine src- noch eine **data-render-src**-Eigenschaft festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="270f9-171">The "Presentation" part HTML contains an image tag with neither the src nor the **data-render-src** properties set.</span></span> <span data-ttu-id="270f9-172">Die API ignoriert das **image**-Tag.</span><span class="sxs-lookup"><span data-stu-id="270f9-172">The API will ignore the **image** tag.</span></span> 

### <a name="20007"></a><span data-ttu-id="270f9-173">20007</span><span class="sxs-lookup"><span data-stu-id="270f9-173">20007</span></span>
<span data-ttu-id="270f9-174">Die „Presentation”-Teil-HTML enthält eine Zeichenfolge mit Erstellungsdatum/-Uhrzeit, die keinem zulässigen Format entspricht.</span><span class="sxs-lookup"><span data-stu-id="270f9-174">The "Presentation" part HTML contains a created date/time string that does not match any of the allowed formats.</span></span> 

### <a name="20008"></a><span data-ttu-id="270f9-175">20008</span><span class="sxs-lookup"><span data-stu-id="270f9-175">20008</span></span>
<span data-ttu-id="270f9-176">Die Anforderung ist zu groß.</span><span class="sxs-lookup"><span data-stu-id="270f9-176">The size of the request is too large.</span></span> 

### <a name="20009"></a><span data-ttu-id="270f9-177">20009</span><span class="sxs-lookup"><span data-stu-id="270f9-177">20009</span></span>
<span data-ttu-id="270f9-178">Die Anforderung enthält Teile mit identischen Namen.</span><span class="sxs-lookup"><span data-stu-id="270f9-178">The request contains parts with duplicate names.</span></span> <span data-ttu-id="270f9-179">Teilnamen müssen eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="270f9-179">Part names must be unique.</span></span> 

### <a name="20010"></a><span data-ttu-id="270f9-180">20010</span><span class="sxs-lookup"><span data-stu-id="270f9-180">20010</span></span>
<span data-ttu-id="270f9-181">Die Kopfzeile „Content-Disposition“ wurde nicht für den angegebenen Inhaltstyp festgelegt.</span><span class="sxs-lookup"><span data-stu-id="270f9-181">The Content-Disposition header was not supplied for the specified content type.</span></span> 

### <a name="20011"></a><span data-ttu-id="270f9-182">20011</span><span class="sxs-lookup"><span data-stu-id="270f9-182">20011</span></span>
<span data-ttu-id="270f9-183">Die Anforderung enthält eine ungültige mehrteilige Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="270f9-183">The request contains a malformed multipart payload.</span></span> <span data-ttu-id="270f9-184">Das Problem kann durch fehlende Leerzeilen, eine fehlende letzten Zeile, falsch formatierte Teil-Trennzeichen usw. ausgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="270f9-184">Problems could include missing blank lines, a missing last line, incorrectly formatted part separators, and so on.</span></span> <span data-ttu-id="270f9-185">Wenn Sie die mehrteilige Nachricht manuell erstellen, überprüfen Sie sorgfältig die Logik oder ziehen Sie eine Drittanbieter-Bibliothek hinzu.</span><span class="sxs-lookup"><span data-stu-id="270f9-185">If you're building the multipart message by hand, carefully check the logic, or consider using a third-party library.</span></span> 

### <a name="20012"></a><span data-ttu-id="270f9-186">20012</span><span class="sxs-lookup"><span data-stu-id="270f9-186">20012</span></span>
<span data-ttu-id="270f9-187">Die Anforderung stellt keinen Inhaltstyp für das angegebene Teil zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="270f9-187">The request doesn't supply a content type for the specified part.</span></span> 

### <a name="20013"></a><span data-ttu-id="270f9-188">20013</span><span class="sxs-lookup"><span data-stu-id="270f9-188">20013</span></span>
<span data-ttu-id="270f9-189">Die Anforderung stellt keinen Inhaltstyp und keine Kopfzeile für die Content-Disposition für das angegebene Teil zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="270f9-189">The request doesn't supply Content-Type and Content-Disposition headers for the specified part.</span></span> 

### <a name="20014"></a><span data-ttu-id="270f9-190">20014</span><span class="sxs-lookup"><span data-stu-id="270f9-190">20014</span></span>
<span data-ttu-id="270f9-191">Die Länge eines Teils in der mehrteiligen Nachricht überschreitet die maximale Größe von 25 MB.</span><span class="sxs-lookup"><span data-stu-id="270f9-191">The length of a part in the multipart message exceeds the maximum size of 25 MB.</span></span> 

### <a name="20015"></a><span data-ttu-id="270f9-192">20015</span><span class="sxs-lookup"><span data-stu-id="270f9-192">20015</span></span>
<span data-ttu-id="270f9-193">Die Anzahl der Teile in der mehrteiligen Nachricht überschreitet die Begrenzung von 500.</span><span class="sxs-lookup"><span data-stu-id="270f9-193">The count of parts in the multipart message exceeds the limit of 500.</span></span> 

### <a name="20016"></a><span data-ttu-id="270f9-194">20016</span><span class="sxs-lookup"><span data-stu-id="270f9-194">20016</span></span>
<span data-ttu-id="270f9-195">Die Länge der mehrteiligen Nachricht überschreitet die maximale Größe von 75 MB.</span><span class="sxs-lookup"><span data-stu-id="270f9-195">The length of the multipart message exceeds the limit of 75 MB.</span></span> 

### <a name="20017"></a><span data-ttu-id="270f9-196">20017</span><span class="sxs-lookup"><span data-stu-id="270f9-196">20017</span></span>
<span data-ttu-id="270f9-197">Die E-Mail-MIME ist fehlerhaft.</span><span class="sxs-lookup"><span data-stu-id="270f9-197">The email MIME was malformed.</span></span> 

### <a name="20018"></a><span data-ttu-id="270f9-198">20018</span><span class="sxs-lookup"><span data-stu-id="270f9-198">20018</span></span>
<span data-ttu-id="270f9-199">Die Besprechungs-MIME oder -ICal ist fehlerhaft.</span><span class="sxs-lookup"><span data-stu-id="270f9-199">The meeting MIME or ICal was malformed.</span></span> 

### <a name="20019"></a><span data-ttu-id="270f9-200">20019</span><span class="sxs-lookup"><span data-stu-id="270f9-200">20019</span></span>
<span data-ttu-id="270f9-201">Es wurde kein ICal gefunden.</span><span class="sxs-lookup"><span data-stu-id="270f9-201">No ICal was found.</span></span> 

### <a name="20020"></a><span data-ttu-id="270f9-202">20020</span><span class="sxs-lookup"><span data-stu-id="270f9-202">20020</span></span>
<span data-ttu-id="270f9-203">Es wurde ein fehlerhafter Json-Anforderungstext gefunden.</span><span class="sxs-lookup"><span data-stu-id="270f9-203">Encountered malformed Json in request body.</span></span> 

### <a name="20100"></a><span data-ttu-id="270f9-204">20100</span><span class="sxs-lookup"><span data-stu-id="270f9-204">20100</span></span>
<span data-ttu-id="270f9-205">Etwas stimmt mit der Syntax der Anforderung nicht.</span><span class="sxs-lookup"><span data-stu-id="270f9-205">Something is wrong with the syntax of your request.</span></span> 

### <a name="20101"></a><span data-ttu-id="270f9-206">20101</span><span class="sxs-lookup"><span data-stu-id="270f9-206">20101</span></span>
<span data-ttu-id="270f9-207">Die angeforderte Eigenschaft ist nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="270f9-207">The property that you requested doesn't exist.</span></span>

### <a name="20102"></a><span data-ttu-id="270f9-208">20102</span><span class="sxs-lookup"><span data-stu-id="270f9-208">20102</span></span>
<span data-ttu-id="270f9-209">Sie haben eine Ressource angefordert, die nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="270f9-209">You requested a resource that doesn't exist.</span></span>

### <a name="20103"></a><span data-ttu-id="270f9-210">20103</span><span class="sxs-lookup"><span data-stu-id="270f9-210">20103</span></span>
<span data-ttu-id="270f9-211">Die **expand**-Abfrage wird für diese Anforderung nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="270f9-211">The **expand** query is not supported for this request.</span></span> <span data-ttu-id="270f9-212">Siehe [Unterstützte Zeichenfolge-Optionen für OData-Anfragen](onenote-get-content.md#supported-odata-query-string-options).</span><span class="sxs-lookup"><span data-stu-id="270f9-212">See [Supported OData query string options](onenote-get-content.md#supported-odata-query-string-options).</span></span>

### <a name="20104"></a><span data-ttu-id="270f9-213">20104</span><span class="sxs-lookup"><span data-stu-id="270f9-213">20104 (SectionNameInvalidChar)</span></span>
<span data-ttu-id="270f9-p119">Die **pagelevel**-Abfrageoption wird nur unterstützt, wenn Sie eine Abfrage für die Seitensammlung in einem Abschnitt oder für eine bestimmte Seite ausführen. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="270f9-p119">The **pagelevel** query option is supported only when querying for the pages collection in a section or for a specific page. For example:</span></span>  

```http
GET ../sections/{id}/pages?pagelevel=true
GET ../pages/{id}?pagelevel=true
```

### <a name="20106"></a><span data-ttu-id="270f9-216">20106</span><span class="sxs-lookup"><span data-stu-id="270f9-216">20106</span></span>
<span data-ttu-id="270f9-217">Ihre Anforderung enthält einen Abfrageoperator, der nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="270f9-217">Your request contains a query operator that is not supported.</span></span> 

### <a name="20108"></a><span data-ttu-id="270f9-218">20108</span><span class="sxs-lookup"><span data-stu-id="270f9-218">20108</span></span>
<span data-ttu-id="270f9-219">Die Anforderung enthält nicht unterstützte OData-Abfrageparameter.</span><span class="sxs-lookup"><span data-stu-id="270f9-219">Your request contains unsupported OData query parameters.</span></span>

### <a name="20109"></a><span data-ttu-id="270f9-220">20109</span><span class="sxs-lookup"><span data-stu-id="270f9-220">20109</span></span>
<span data-ttu-id="270f9-221">Die Nutzlast in der PATCH-Anforderung wurde nicht ordnungsgemäß erstellt.</span><span class="sxs-lookup"><span data-stu-id="270f9-221">The payload in the PATCH request is not constructed correctly.</span></span>

### <a name="20110"></a><span data-ttu-id="270f9-222">20110</span><span class="sxs-lookup"><span data-stu-id="270f9-222">20110</span></span>
<span data-ttu-id="270f9-223">Bei Anfragen für die Erstellung von Seiten mit Datenteilen muss der Inhalt mehrteilig sein und einen „Präsentation“-Teil enthalten.</span><span class="sxs-lookup"><span data-stu-id="270f9-223">Page create requests with data parts require the content to be multipart, with a "Presentation" part.</span></span> 

### <a name="20111"></a><span data-ttu-id="270f9-224">20111</span><span class="sxs-lookup"><span data-stu-id="270f9-224">20111</span></span>
<span data-ttu-id="270f9-225">Ihre Anforderung verwendet ein OData-Feature, das nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="270f9-225">Your request uses an OData feature that isn't supported.</span></span>

### <a name="20112"></a><span data-ttu-id="270f9-226">20112</span><span class="sxs-lookup"><span data-stu-id="270f9-226">20112</span></span>
<span data-ttu-id="270f9-227">Ihre Anfrage enthält eine ungültige ID für das Ziel-Notebook, die Abschnittsgruppe, den Abschnitt oder die Seitenentität.</span><span class="sxs-lookup"><span data-stu-id="270f9-227">Your request contains an invalid ID for the target notebook, section group, section, or page entity.</span></span>

### <a name="20113"></a><span data-ttu-id="270f9-228">20113</span><span class="sxs-lookup"><span data-stu-id="270f9-228">20113</span></span>
<span data-ttu-id="270f9-229">Die in der Anforderung angegebene Ressource wurde gelöscht.</span><span class="sxs-lookup"><span data-stu-id="270f9-229">The resource specified in the request has been deleted.</span></span>

### <a name="20115"></a><span data-ttu-id="270f9-230">20115</span><span class="sxs-lookup"><span data-stu-id="270f9-230">20115</span></span>
<span data-ttu-id="270f9-231">Der Name enthält ungültige Zeichen.</span><span class="sxs-lookup"><span data-stu-id="270f9-231">The name contains invalid characters.</span></span> <span data-ttu-id="270f9-232">Der Name des Notizbuchs darf die folgenden Zeichen nicht enthalten: `? * \ / : < > | ' "`</span><span class="sxs-lookup"><span data-stu-id="270f9-232">A notebook name cannot contain any of the following characters: `? * \ / : < > | ' "`</span></span>

### <a name="20117"></a><span data-ttu-id="270f9-233">20117</span><span class="sxs-lookup"><span data-stu-id="270f9-233">20117</span></span>
<span data-ttu-id="270f9-234">Ein Element mit dem angegebenen Namen ist bereits im angegebenen Ort vorhanden.</span><span class="sxs-lookup"><span data-stu-id="270f9-234">An item with the name you specified already exists in the location that you specified.</span></span>

### <a name="20119"></a><span data-ttu-id="270f9-235">20119</span><span class="sxs-lookup"><span data-stu-id="270f9-235">20119</span></span>
<span data-ttu-id="270f9-236">Die HTML im „Presentation“-Teil enthält ein **data-attachment**-Attribut, das kein gültiges Format hat oder einen oder mehrere dieser ungültigen Zeichen für einen Dateinamen enthält: `\ / : * ? < > | "`.</span><span class="sxs-lookup"><span data-stu-id="270f9-236">The HTML in the "Presentation" part contains a **data-attachment** attribute that either doesn't have a valid format or includes one or more of these invalid characters for a file name: `\ / : * ? < > | "`.</span></span> <span data-ttu-id="270f9-237">Die Anforderung hat den Wert in der Fehlermeldung ersetzt.</span><span class="sxs-lookup"><span data-stu-id="270f9-237">The request substituted the value indicated in the error message.</span></span>

### <a name="20120"></a><span data-ttu-id="270f9-238">20120</span><span class="sxs-lookup"><span data-stu-id="270f9-238">20120</span></span>
<span data-ttu-id="270f9-239">Die Anforderung gibt ein PATCH-Ziel an, das nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="270f9-239">Your request specifies a PATCH target that can't be located.</span></span>

### <a name="20121"></a><span data-ttu-id="270f9-240">20121</span><span class="sxs-lookup"><span data-stu-id="270f9-240">20121</span></span>
<span data-ttu-id="270f9-p122">Die Anforderung enthält ein ungültiges PATCH-Argument. Weitere Informationen finden Sie unter [Aktualisieren von Seiteninhalt](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-p122">Your request contains an invalid PATCH argument. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20122"></a><span data-ttu-id="270f9-243">20122</span><span class="sxs-lookup"><span data-stu-id="270f9-243">20122</span></span>
<span data-ttu-id="270f9-p123">Ihre Anforderung gibt eine nicht unterstützte PATCH-Aktion an. Weitere Informationen finden Sie unter [Aktualisieren von Seiteninhalt](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-p123">Your request specifies an unsupported PATCH action. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20123"></a><span data-ttu-id="270f9-246">20123</span><span class="sxs-lookup"><span data-stu-id="270f9-246">20123</span></span>
<span data-ttu-id="270f9-247">Die PATCH-Anforderung kann die angegebene Seite nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="270f9-247">The PATCH request is unable to alter the specified page.</span></span>

### <a name="20124"></a><span data-ttu-id="270f9-248">20124</span><span class="sxs-lookup"><span data-stu-id="270f9-248">20124</span></span>
<span data-ttu-id="270f9-249">Die mehrteilige PATCH-Anforderung beinhaltet keinen „Befehle“-Teil mit der PATCH-Aktion-JSON-Struktur.</span><span class="sxs-lookup"><span data-stu-id="270f9-249">Your multipart PATCH request doesn't include a "commands" part with the PATCH action JSON structure.</span></span> <span data-ttu-id="270f9-250">Siehe [Aktualisieren von Seiteninhalt](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-250">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20125"></a><span data-ttu-id="270f9-251">20125</span><span class="sxs-lookup"><span data-stu-id="270f9-251">20125</span></span>
<span data-ttu-id="270f9-p125">Die PATCH-Anforderung enthält keine Aktionen. Weitere Informationen finden Sie unter [Aktualisieren von Seiteninhalt](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-p125">Your PATCH request contains no actions. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20126"></a><span data-ttu-id="270f9-254">20126</span><span class="sxs-lookup"><span data-stu-id="270f9-254">20126</span></span>
<span data-ttu-id="270f9-255">Der Nachrichtentext enthält entweder falsch formatierten JSON-Code oder Felder, die für diesen Vorgang nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="270f9-255">The message body contains either incorrectly formatted JSON or fields that are not supported for this operation.</span></span>

### <a name="20127"></a><span data-ttu-id="270f9-256">20127</span><span class="sxs-lookup"><span data-stu-id="270f9-256">20127</span></span>
<span data-ttu-id="270f9-257">Die Anfrage gibt den Namen einer unbekannten Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="270f9-257">Your request specifies the name of an unknown property.</span></span>

### <a name="20128"></a><span data-ttu-id="270f9-258">20128</span><span class="sxs-lookup"><span data-stu-id="270f9-258">20128</span></span>
<span data-ttu-id="270f9-259">Die Anforderung enthält einen OData-Syntaxfehler an der in der Nachricht angegebenen Position.</span><span class="sxs-lookup"><span data-stu-id="270f9-259">Your request contains an OData syntax error at the position indicated in the message.</span></span>

### <a name="20129"></a><span data-ttu-id="270f9-260">20129</span><span class="sxs-lookup"><span data-stu-id="270f9-260">20129</span></span>
<span data-ttu-id="270f9-261">Die Anforderung enthält eine **top**-Abfrage-Zeichenfolgeoption, deren Wert zu hoch ist.</span><span class="sxs-lookup"><span data-stu-id="270f9-261">Your request contains a **top** query string option whose value is too high.</span></span> <span data-ttu-id="270f9-262">Der Maximalwert für Seitenabfragen beträgt 100, und der Standardwert ist 20.</span><span class="sxs-lookup"><span data-stu-id="270f9-262">For page queries, the maximum value is 100, and the default value is 20.</span></span>

### <a name="20130"></a><span data-ttu-id="270f9-263">20130</span><span class="sxs-lookup"><span data-stu-id="270f9-263">20130</span></span>
<span data-ttu-id="270f9-264">Die Anforderung enthält einen URI, der zu einer HTTP-Ressource zeigt, die nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="270f9-264">Your request contains a URI that points to an HTTP resource that can't be found.</span></span>

### <a name="20131"></a><span data-ttu-id="270f9-265">20131</span><span class="sxs-lookup"><span data-stu-id="270f9-265">20131</span></span>
<span data-ttu-id="270f9-266">Die Anforderung enthält einen ungültigen Wert für den Inhaltstyp.</span><span class="sxs-lookup"><span data-stu-id="270f9-266">Your request contains an invalid value for Content-Type.</span></span> <span data-ttu-id="270f9-267">Verwenden Sie den in der Nachricht angegeben Wert.</span><span class="sxs-lookup"><span data-stu-id="270f9-267">Use the value indicated in the message.</span></span> 

### <a name="20132"></a><span data-ttu-id="270f9-268">20132</span><span class="sxs-lookup"><span data-stu-id="270f9-268">20132</span></span>
<span data-ttu-id="270f9-269">Die Anforderung enthält ungültige Inhalte.</span><span class="sxs-lookup"><span data-stu-id="270f9-269">Your request contains invalid content.</span></span> <span data-ttu-id="270f9-270">Häufige Ursachen hierfür sind eine fehlende Kopfzeile für die Inhaltstyp-Anfrage und/oder keine Inhalte im Textkörper der Anfrage.</span><span class="sxs-lookup"><span data-stu-id="270f9-270">Common causes for this are a missing Content-Type request header and/or no content in the body of the request.</span></span> 

### <a name="20133"></a><span data-ttu-id="270f9-271">20133</span><span class="sxs-lookup"><span data-stu-id="270f9-271">20133</span></span>
<span data-ttu-id="270f9-272">Die Anforderung gibt ein PATCH-Ziel an, das nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="270f9-272">Your request specifies a PATCH target that is not supported.</span></span> <span data-ttu-id="270f9-273">Siehe [Aktualisieren von Seiteninhalt](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-273">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20134"></a><span data-ttu-id="270f9-274">20134</span><span class="sxs-lookup"><span data-stu-id="270f9-274">20134</span></span>
<span data-ttu-id="270f9-p130">Die Anforderung gibt ein ungültiges Element als Ziel der PATCH-Aktion an. Wenn das Ziel den **data-id**-Bezeichner verwendet, stellen Sie sicher, dass ein #-Symbol diesem vorangestellt ist. Weitere Informationen finden Sie unter [Aktualisieren von Seiteninhalt](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-p130">Your request specifies an invalid element as the target of the PATCH action. If the target uses the **data-id** identifier, make sure it's prefixed with a # symbol. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20135"></a><span data-ttu-id="270f9-278">20135</span><span class="sxs-lookup"><span data-stu-id="270f9-278">20135</span></span>
<span data-ttu-id="270f9-279">Die Anforderung gibt einen Entitätstyp an, der für den PATCH-Vorgang nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="270f9-279">Your request specifies an entity type that is not supported for the PATCH operation.</span></span> <span data-ttu-id="270f9-280">Siehe [Aktualisieren von Seiteninhalt](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-280">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20136"></a><span data-ttu-id="270f9-281">20136</span><span class="sxs-lookup"><span data-stu-id="270f9-281">20136</span></span>
<span data-ttu-id="270f9-282">Ihre Anforderung enthält ein ungültiges oder fehlendes **data-render-src**- oder **data-render-method**-Attribut.</span><span class="sxs-lookup"><span data-stu-id="270f9-282">Your request contains an invalid or missing **data-render-src** or **data-render-method** attribute.</span></span> <span data-ttu-id="270f9-283">Siehe [Extrahieren von Daten aus Bildschirmausschnitten](onenote-extract-data.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-283">See [Extract data from captures](onenote-extract-data.md).</span></span>

### <a name="20137"></a><span data-ttu-id="270f9-284">20137</span><span class="sxs-lookup"><span data-stu-id="270f9-284">20137</span></span>
<span data-ttu-id="270f9-285">Die Zielseite unterstützt keine PATCH-Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="270f9-285">The target page does not support PATCH requests.</span></span>

### <a name="20138"></a><span data-ttu-id="270f9-286">20138</span><span class="sxs-lookup"><span data-stu-id="270f9-286">20138</span></span>
<span data-ttu-id="270f9-p133">Das Ziel in der PATCH-Anforderung unterstützt die angegebene **append**Aktion nicht. Weitere Informationen finden Sie unter [Aktualisieren von Seiteninhalt](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-p133">The target element type in your PATCH request doesn't support the **append** action. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20139"></a><span data-ttu-id="270f9-289">20139</span><span class="sxs-lookup"><span data-stu-id="270f9-289">20139</span></span>
<span data-ttu-id="270f9-p134">Die Anforderung enthält einen ungültigen **data-tag**-Attributwert. Weitere Informationen finden Sie unter [Verwenden von Notiztags](onenote-note-tags.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-p134">Your request contains an invalid **data-tag** attribute value. See [Use note tags](onenote-note-tags.md).</span></span>

### <a name="20140"></a><span data-ttu-id="270f9-292">20140</span><span class="sxs-lookup"><span data-stu-id="270f9-292">20140</span></span>
<span data-ttu-id="270f9-293">Die Anforderung enthält einen ungültigen **data-tag**-Statuswert.</span><span class="sxs-lookup"><span data-stu-id="270f9-293">Your request contains an invalid **data-tag** status value.</span></span> <span data-ttu-id="270f9-294">Kontrollkästchen-Notiztags können den Status **completed** besitzen.</span><span class="sxs-lookup"><span data-stu-id="270f9-294">Check box note tags can have a **completed** status.</span></span> 

<span data-ttu-id="270f9-295">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="270f9-295">Example:</span></span>

```html
    <p data-tag="to-do:completed">To-do note tag in completed state (checked box in the UI)</p>
```
<span data-ttu-id="270f9-296">Siehe [Verwenden von Notiztags](onenote-note-tags.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-296">See [Use note tags](onenote-note-tags.md).</span></span>

### <a name="20141"></a><span data-ttu-id="270f9-297">20141</span><span class="sxs-lookup"><span data-stu-id="270f9-297">20141</span></span>
<span data-ttu-id="270f9-298">Der Zielelementtyp in der PATCH-Anforderung unterstützt die angegebene Aktion nicht.</span><span class="sxs-lookup"><span data-stu-id="270f9-298">The target in your PATCH request doesn't support the specified action.</span></span> <span data-ttu-id="270f9-299">Siehe [Aktualisieren von Seiteninhalt](onenote-update-page.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-299">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20142"></a><span data-ttu-id="270f9-300">20142</span><span class="sxs-lookup"><span data-stu-id="270f9-300">20142</span></span>
<span data-ttu-id="270f9-301">Ihre Anforderung enthält einen **expand**-Ausdruck für ein übergeordnetes Element untergeordneter Entitäten oder ein untergeordnetes Element übergeordneter Entitäten, der nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="270f9-301">Your request contains an **expand** expression for a parent of child entities or a child of parent entities, which is not supported.</span></span> <span data-ttu-id="270f9-302">Siehe [Unterstützte Zeichenfolge-Optionen für OData-Anfragen](onenote-get-content.md#supported-odata-query-string-options).</span><span class="sxs-lookup"><span data-stu-id="270f9-302">See [Supported OData query string options](onenote-get-content.md#supported-odata-query-string-options).</span></span>

### <a name="20143"></a><span data-ttu-id="270f9-303">20143</span><span class="sxs-lookup"><span data-stu-id="270f9-303">20143</span></span>
<span data-ttu-id="270f9-304">Die OData-Abfrage ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="270f9-304">The OData query is invalid.</span></span>

### <a name="20144"></a><span data-ttu-id="270f9-305">20144</span><span class="sxs-lookup"><span data-stu-id="270f9-305">20144</span></span>
<span data-ttu-id="270f9-306">Die Anforderung enthält einen **expand**-Ausdruck für eine Nicht-Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="270f9-306">Your request contains an **expand** expression for a non-navigation property.</span></span> <span data-ttu-id="270f9-307">Nur Navigationseigenschaften können erweitert werden.</span><span class="sxs-lookup"><span data-stu-id="270f9-307">Only navigation properties can be expanded.</span></span>

### <a name="20145"></a><span data-ttu-id="270f9-308">20145</span><span class="sxs-lookup"><span data-stu-id="270f9-308">20145</span></span>
<span data-ttu-id="270f9-309">Der **select**- oder **expand**-Ausdruck in der Anforderung enthält einen ungültigen Term.</span><span class="sxs-lookup"><span data-stu-id="270f9-309">The **select** or **expand** expression in your request contains an invalid term.</span></span>

### <a name="20146"></a><span data-ttu-id="270f9-310">20146</span><span class="sxs-lookup"><span data-stu-id="270f9-310">20146</span></span>
<span data-ttu-id="270f9-311">Das `style="position:absolute"`-Attribut wurde für ein Element angegeben, aber das **body**-Element gibt `data-absolute-enabled="true"` nicht an, das jedoch für die Unterstützung der Positionierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="270f9-311">The `style="position:absolute"` attribute is specified on an element, but the **body** element does not specify `data-absolute-enabled="true"`, which is required to support positioning.</span></span> <span data-ttu-id="270f9-312">Alle Positionseinstellungen werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="270f9-312">All position settings will be ignored.</span></span> <span data-ttu-id="270f9-313">Siehe [Erstellen von absolut positionierten Elementen](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-313">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20147"></a><span data-ttu-id="270f9-314">20147</span><span class="sxs-lookup"><span data-stu-id="270f9-314">20147</span></span>
<span data-ttu-id="270f9-315">Das `style="position:absolute"`-Attribut ist für ein Element angegeben, das kein direkt untergeordnetes Element des **body**-Elemente ist, welches nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="270f9-315">The `style="position:absolute"` attribute is specified on an element that is not a direct child of the **body** element, which is not supported.</span></span> <span data-ttu-id="270f9-316">Wenn das Element **div**, **img** oder **object** ist, muss es als untergeordnetes Element des Textkörpers angegeben werden; andernfalls werden die Positionseinstellungen ignoriert und die dazugehörigen Inhalte werden als absolut positioniertes div dargestellt.</span><span class="sxs-lookup"><span data-stu-id="270f9-316">If the element is a **div**, **img**, or **object**, make it a direct child of the body; otherwise the position settings will be ignored and its content will render inside an absolute positioned div.</span></span> <span data-ttu-id="270f9-317">Siehe [Erstellen von absolut positionierten Elementen](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-317">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20148"></a><span data-ttu-id="270f9-318">20148</span><span class="sxs-lookup"><span data-stu-id="270f9-318">20148</span></span>
<span data-ttu-id="270f9-319">Das `style="position:absolute"`-Attribut ist für einen nicht unterstützten Elementyp angegeben.</span><span class="sxs-lookup"><span data-stu-id="270f9-319">The `style="position:absolute"` attribute is specified on an element type that does not support it.</span></span> <span data-ttu-id="270f9-320">Nur **div**-, **img**- und **object**-Elemente, die direkt untergeordnete Elemente des Seitentextes sind, unterstützten die Positionierung.</span><span class="sxs-lookup"><span data-stu-id="270f9-320">Only **div**, **img**, and **object** elements that are direct children of the page body support positioning.</span></span> <span data-ttu-id="270f9-321">Siehe [Erstellen von absolut positionierten Elementen](onenote-abs-pos.md).</span><span class="sxs-lookup"><span data-stu-id="270f9-321">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20149"></a><span data-ttu-id="270f9-322">20149</span><span class="sxs-lookup"><span data-stu-id="270f9-322">20149</span></span>
<span data-ttu-id="270f9-323">Die Anforderung gibt ein Zielelement an, das nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="270f9-323">Your request specifies a target element that cannot be found.</span></span>

### <a name="20150"></a><span data-ttu-id="270f9-324">20150</span><span class="sxs-lookup"><span data-stu-id="270f9-324">20150</span></span>
<span data-ttu-id="270f9-325">Die Anforderung ist für diesen Authentifizierungstyp nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="270f9-325">The request is not valid for this authentication type.</span></span> <span data-ttu-id="270f9-326"> Verwenden Sie stattdessen den `../me/onenote/\`-Pfad.</span><span class="sxs-lookup"><span data-stu-id="270f9-326">Use the `../me/onenote/` path instead.</span></span>

### <a name="20151"></a><span data-ttu-id="270f9-327">20151</span><span class="sxs-lookup"><span data-stu-id="270f9-327">20151</span></span>
<span data-ttu-id="270f9-328">Die Anforderung ist für diesen Authentifizierungstyp nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="270f9-328">The request is not valid for this authentication type.</span></span> <span data-ttu-id="270f9-329">Verwenden Sie den `../me/onenote/section/{id}/pages`-Endpunkt, um eine Seite in einem bestimmten Abschnitt zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="270f9-329">Use the `../me/onenote/section/{id}/pages` endpoint to create a page in a specific section.</span></span>

### <a name="20152"></a><span data-ttu-id="270f9-330">20152</span><span class="sxs-lookup"><span data-stu-id="270f9-330">20152 (EntityNameEmpty)</span></span>
<span data-ttu-id="270f9-p144">Für die Entität ist kein name-Wert angegeben. Der Name muss definiert werden, und er darf nicht nur aus Leerzeichen bestehen.</span><span class="sxs-lookup"><span data-stu-id="270f9-p144">There is no name value specified for the entity. The name must be defined, and it cannot contain whitespaces only.</span></span>

### <a name="20153"></a><span data-ttu-id="270f9-333">20153</span><span class="sxs-lookup"><span data-stu-id="270f9-333">20153 (EntityNameInvalidChar)</span></span>
<span data-ttu-id="270f9-334">Der Entitätsname enthält ungültige Zeichen.</span><span class="sxs-lookup"><span data-stu-id="270f9-334">The entity name contains invalid characters.</span></span> <span data-ttu-id="270f9-335">Der Name darf die folgenden Zeichen nicht enthalten: `? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="270f9-335">The name cannot contain the following characters: `? * \ / : < > | & # " % ~`</span></span>

### <a name="20154"></a><span data-ttu-id="270f9-336">20154</span><span class="sxs-lookup"><span data-stu-id="270f9-336">20154 (EntityNameInvalidStart)</span></span>
<span data-ttu-id="270f9-337">Der Entitätsname darf nicht mit einem Leerzeichen beginnen.</span><span class="sxs-lookup"><span data-stu-id="270f9-337">The entity name cannot start with a space.</span></span>

### <a name="20155"></a><span data-ttu-id="270f9-338">20155</span><span class="sxs-lookup"><span data-stu-id="270f9-338">20155 (EntityNameTooLong)</span></span>
<span data-ttu-id="270f9-339">Der Entitätsname ist zu lang.</span><span class="sxs-lookup"><span data-stu-id="270f9-339">The entity name is too long.</span></span> <span data-ttu-id="270f9-340">Namen für Notizbücher dürfen maximal 128 Zeichen lang sein.</span><span class="sxs-lookup"><span data-stu-id="270f9-340">Notebook names have a 128-character limit.</span></span> <span data-ttu-id="270f9-341">Andere Entitätsnamen dürfen maximal 50 Zeichen lang sein.</span><span class="sxs-lookup"><span data-stu-id="270f9-341">Other entity names have a 50-character limit.</span></span>

### <a name="20156"></a><span data-ttu-id="270f9-342">20156</span><span class="sxs-lookup"><span data-stu-id="270f9-342">20156</span></span>
<span data-ttu-id="270f9-343">Die angegebene ID für die Zielressource ist nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="270f9-343">The specified ID for the destination resource does not exist.</span></span>

### <a name="20157"></a><span data-ttu-id="270f9-344">20157</span><span class="sxs-lookup"><span data-stu-id="270f9-344">20157</span></span>
<span data-ttu-id="270f9-345">Die angegebene ID für die Zielentität ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="270f9-345">The specified ID for the destination entity is invalid.</span></span>

### <a name="20158"></a><span data-ttu-id="270f9-346">20158</span><span class="sxs-lookup"><span data-stu-id="270f9-346">20158</span></span>
<span data-ttu-id="270f9-347">Die Metadaten für die Website-URL in der angegebenen Anfrage können nicht abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="270f9-347">Unable to get metadata for the site URL specified in the request.</span></span> <span data-ttu-id="270f9-348">Überprüfen Sie das Format der angegebenen URL.</span><span class="sxs-lookup"><span data-stu-id="270f9-348">Check the format of the supplied URL.</span></span> <span data-ttu-id="270f9-349">Zu den unterstützten Formate gehören `https://domain.sharepoint.com/site-a` und `https://domain.com/sites/site-a`.</span><span class="sxs-lookup"><span data-stu-id="270f9-349">Supported formats include `https://domain.sharepoint.com/site-a` and `https://domain.com/sites/site-a`.</span></span>

### <a name="20160"></a><span data-ttu-id="270f9-350">20160</span><span class="sxs-lookup"><span data-stu-id="270f9-350">20160</span></span>
<span data-ttu-id="270f9-351">Es kann keine einheitliche Office 365-Gruppe mit der angegebenen ID gefunden werden.</span><span class="sxs-lookup"><span data-stu-id="270f9-351">Unable to find an Office 365 unified group that has the specified ID.</span></span>

### <a name="20161"></a><span data-ttu-id="270f9-352">20161</span><span class="sxs-lookup"><span data-stu-id="270f9-352">20161</span></span>
<span data-ttu-id="270f9-353">Der Kontext gibt keine gültige Benutzer-ID an.</span><span class="sxs-lookup"><span data-stu-id="270f9-353">The context does not specify a valid user ID.</span></span> <span data-ttu-id="270f9-354">Ein häufiger Fehler ist, dass die PUID/CID in Langform statt als Hexadezimalwert übergeben wurde.</span><span class="sxs-lookup"><span data-stu-id="270f9-354">One common error is that PUID/CID was passed in as a long instead of a hex.</span></span>

### <a name="20166"></a><span data-ttu-id="270f9-355">20166</span><span class="sxs-lookup"><span data-stu-id="270f9-355">20166</span></span>
<span data-ttu-id="270f9-356">Die Anwendung hat zu viele Anfragen im Auftrag eines Benutzers innerhalb eines kurzen Zeitraums ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="270f9-356">The application has issued too many requests on behalf of a user in a short period of time.</span></span> <span data-ttu-id="270f9-357">Um sicherzustellen, dass die OneNote-API stabil und reaktionsschnell bleibt, gibt die API den Statuscode 429 und diesen Fehler aus, wenn sie erkennt, dass eine Anwendung zu viele Ressourcen verwendet.</span><span class="sxs-lookup"><span data-stu-id="270f9-357">To help ensure that the OneNote API remains stable and responsive, the API returns a 429 status code and this error when it detects that an application is using too many resources.</span></span> 

<span data-ttu-id="270f9-358">Weitere Informationen finden Sie unter [Drosselung von OneNote-API und wie Sie dies vermeiden](https://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span><span class="sxs-lookup"><span data-stu-id="270f9-358">For more information, see [OneNote API throttling and how to avoid it](https://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span></span>

### <a name="20168"></a><span data-ttu-id="270f9-359">20168</span><span class="sxs-lookup"><span data-stu-id="270f9-359">20168</span></span>
<span data-ttu-id="270f9-360">Die in der Anfrage angegebene Video-Quelle wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="270f9-360">The video source specified in the request is not supported.</span></span> <span data-ttu-id="270f9-361">Eine aktuelle Liste finden Sie unter [Unterstützte Video-Websites](onenote-images-files.md#adding-videos).</span><span class="sxs-lookup"><span data-stu-id="270f9-361">See [Supported video sites](onenote-images-files.md#adding-videos) for the current list.</span></span>


## <a name="codes-from-30001-to-39999"></a><span data-ttu-id="270f9-362">Codes von 30001 bis 39999</span><span class="sxs-lookup"><span data-stu-id="270f9-362">Codes from 30001 to 39999</span></span>
<span data-ttu-id="270f9-363">Etwas stimmt nicht mit dem Benutzerkonto.</span><span class="sxs-lookup"><span data-stu-id="270f9-363">Something is wrong with the user's account.</span></span>

### <a name="30101"></a><span data-ttu-id="270f9-364">30101</span><span class="sxs-lookup"><span data-stu-id="270f9-364">30101</span></span>
<span data-ttu-id="270f9-365">Das Benutzerkonto hat das OneDrive-Kontingent überschritten.</span><span class="sxs-lookup"><span data-stu-id="270f9-365">The user account has exceeded its OneDrive quota.</span></span> <span data-ttu-id="270f9-366">Siehe [OneDrive](https://onedrive.live.com/about/de-DE/).</span><span class="sxs-lookup"><span data-stu-id="270f9-366">See [OneDrive](https://onedrive.live.com/about/de-DE/).</span></span>

### <a name="30102"></a><span data-ttu-id="270f9-367">30102</span><span class="sxs-lookup"><span data-stu-id="270f9-367">30102</span></span>
<span data-ttu-id="270f9-368">Es kann nichts mehr zum angeforderten Abschnitt hinzugefügt werden, da dieser seine maximale Größe ereicht hat.</span><span class="sxs-lookup"><span data-stu-id="270f9-368">Nothing more can be added to the requested section because it has reached its maximum size.</span></span>

### <a name="30103"></a><span data-ttu-id="270f9-369">30103</span><span class="sxs-lookup"><span data-stu-id="270f9-369">30103</span></span>
<span data-ttu-id="270f9-370">Der Ressourceverbrauch ist zu hoch für die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="270f9-370">Resource consumption is too high for the request.</span></span> <span data-ttu-id="270f9-371">Entweder weist das Benutzerkonto ein zu großes Datenset auf, oder der Dienst erhält eine große Anzahl konkurrierender Anforderungen für dieselbe Website (z. B. die persönliche Website des Benutzers oder eine Teamwebsite).</span><span class="sxs-lookup"><span data-stu-id="270f9-371">Either the target user account has a large dataset, or the service is receiving a high number of concurrent requests to the same site (for example, the user's personal site or a team site).</span></span>

### <a name="30104"></a><span data-ttu-id="270f9-372">30104</span><span class="sxs-lookup"><span data-stu-id="270f9-372">30104</span></span>
<span data-ttu-id="270f9-373">Das Benutzerkonto wurde angehalten.</span><span class="sxs-lookup"><span data-stu-id="270f9-373">The user account has been suspended.</span></span>

### <a name="30105"></a><span data-ttu-id="270f9-374">30105</span><span class="sxs-lookup"><span data-stu-id="270f9-374">30105</span></span>
<span data-ttu-id="270f9-375">Die persönliche OneDrive for Business-Website des Benutzers, die für den Zugriff auf Notizbücher erforderlich ist,  wird nicht bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="270f9-375">The user's personal OneDrive for Business site is not provisioned, which is required to access notebooks.</span></span> <span data-ttu-id="270f9-376">Der OneNote-Dienst stellt die Seite jetzt bereit.</span><span class="sxs-lookup"><span data-stu-id="270f9-376">The OneNote service will provision the site now.</span></span> <span data-ttu-id="270f9-377">Dieser Vorgang kann mehrere Minuten dauern.</span><span class="sxs-lookup"><span data-stu-id="270f9-377">This process may take several minutes.</span></span>

### <a name="30106"></a><span data-ttu-id="270f9-378">30106</span><span class="sxs-lookup"><span data-stu-id="270f9-378">30106</span></span>
<span data-ttu-id="270f9-379">OneDrive for Business wird für den Benutzer bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="270f9-379">OneDrive for Business is being provisioned for the user.</span></span>

### <a name="30108"></a><span data-ttu-id="270f9-380">30108</span><span class="sxs-lookup"><span data-stu-id="270f9-380">30108</span></span>
<span data-ttu-id="270f9-381">Das persönliche OneDrive for Business des Benutzers konnte nicht abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="270f9-381">The user's personal OneDrive for Business could not be retrieved.</span></span> <span data-ttu-id="270f9-382">Die folgende Tabelle enthält mögliche Ursachen.</span><span class="sxs-lookup"><span data-stu-id="270f9-382">The following table lists some possible causes.</span></span>

| <span data-ttu-id="270f9-383">Ursache</span><span class="sxs-lookup"><span data-stu-id="270f9-383">Cause</span></span> | <span data-ttu-id="270f9-384">Lösung</span><span class="sxs-lookup"><span data-stu-id="270f9-384">Resolution</span></span> |
|:------|:------|
| <span data-ttu-id="270f9-385">Die persönliche Website des Benutzers wurde nicht bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="270f9-385">The user's personal site has not been provisioned.</span></span> | <span data-ttu-id="270f9-386">Der Benutzer sollte OneDrive for Business öffnen und die Anweisungen befolgen, um die Website bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="270f9-386">The user should open OneDrive for Business and follow any instructions to provision the site.</span></span> <span data-ttu-id="270f9-387">Wenn dies fehlschlägt, sollten er sich an seinen Office 365-Mandanten-Administrator wenden.</span><span class="sxs-lookup"><span data-stu-id="270f9-387">If this fails, they should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="270f9-388">Die persönliche Website des Benutzers wird derzeit bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="270f9-388">The user's personal site is currently being provisioned.</span></span> | <span data-ttu-id="270f9-389">Senden Sie die Anforderung später erneut.</span><span class="sxs-lookup"><span data-stu-id="270f9-389">Try the request later.</span></span> |
| <span data-ttu-id="270f9-390">Der Benutzer besitzt keine gültige OneDrive for Business-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="270f9-390">The user does not have a valid OneDrive for Business license.</span></span> | <span data-ttu-id="270f9-391">Der Benutzer sollte sich an seinen Office 365-Mandanten-Administrator wenden.</span><span class="sxs-lookup"><span data-stu-id="270f9-391">The user should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="270f9-392">Die Anfrage konnte aufgrund eines Netzwerkfehlers nicht erfolgreich versendet werden.</span><span class="sxs-lookup"><span data-stu-id="270f9-392">A network issue prevented the request from being successfully sent.</span></span> | <span data-ttu-id="270f9-393">Senden Sie die Anforderung später erneut.</span><span class="sxs-lookup"><span data-stu-id="270f9-393">Try the request later.</span></span> |

### <a name="30109"></a><span data-ttu-id="270f9-394">30109</span><span class="sxs-lookup"><span data-stu-id="270f9-394">30109</span></span>
<span data-ttu-id="270f9-395">Einige Benutzer in der Anforderung sind nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="270f9-395">Some users in the request do not exist.</span></span>

### <a name="30110"></a><span data-ttu-id="270f9-396">30110</span><span class="sxs-lookup"><span data-stu-id="270f9-396">30110</span></span>
<span data-ttu-id="270f9-397">Student Information Services wurde nicht für diesen Mandanten registriert.</span><span class="sxs-lookup"><span data-stu-id="270f9-397">Student Information Services has not been registered for this tenant.</span></span>

### <a name="30111"></a><span data-ttu-id="270f9-398">30111</span><span class="sxs-lookup"><span data-stu-id="270f9-398">30111</span></span>
<span data-ttu-id="270f9-399">Es ist ein allgemeiner Fehler mit Student Information Services aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="270f9-399">There is a generic error with Student Information Services.</span></span>

### <a name="30112"></a><span data-ttu-id="270f9-400">30112</span><span class="sxs-lookup"><span data-stu-id="270f9-400">30112</span></span>
<span data-ttu-id="270f9-401">Mehrere Benutzer, die von dieser Anforderung betroffen waren, besitzen den gleichen Benutzernamen.</span><span class="sxs-lookup"><span data-stu-id="270f9-401">Multiple users affected by the request had the same username.</span></span>

### <a name="30113"></a><span data-ttu-id="270f9-402">30113</span><span class="sxs-lookup"><span data-stu-id="270f9-402">30113</span></span>
<span data-ttu-id="270f9-403">Das Notizbuch ist nicht für Einladungen konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="270f9-403">The notebook is not configured to allow invites.</span></span>

### <a name="30114"></a><span data-ttu-id="270f9-404">30114</span><span class="sxs-lookup"><span data-stu-id="270f9-404">30114</span></span>
<span data-ttu-id="270f9-405">Ein erforderlicher Parameter fehlt.</span><span class="sxs-lookup"><span data-stu-id="270f9-405">There is a required parameter missing.</span></span>

## <a name="codes-from-40001-to-49999"></a><span data-ttu-id="270f9-406">Codes von 40001 bis 49999</span><span class="sxs-lookup"><span data-stu-id="270f9-406">Codes from 40001 to 49999</span></span>
<span data-ttu-id="270f9-407">Der Benutzer oder die Anwendung besitzt nicht die erforderlichen Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="270f9-407">The user or application does not have the correct permissions.</span></span>

### <a name="40001"></a><span data-ttu-id="270f9-408">40001</span><span class="sxs-lookup"><span data-stu-id="270f9-408">40001</span></span>
<span data-ttu-id="270f9-409">Die Anforderung enthält kein gültiges OAuth-Token.</span><span class="sxs-lookup"><span data-stu-id="270f9-409">The request doesn't contain a valid OAuth token.</span></span> <span data-ttu-id="270f9-410">Siehe [Notizberechtigungen](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="270f9-410">See [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

### <a name="40002"></a><span data-ttu-id="270f9-411">40002</span><span class="sxs-lookup"><span data-stu-id="270f9-411">40002</span></span>
<span data-ttu-id="270f9-412">Der Benutzer hat keine Berechtigung, an den angeforderten Ort zu schreiben.</span><span class="sxs-lookup"><span data-stu-id="270f9-412">The user doesn't have permission to write to the requested location.</span></span>

### <a name="40003"></a><span data-ttu-id="270f9-413">40003</span><span class="sxs-lookup"><span data-stu-id="270f9-413">40003</span></span>
<span data-ttu-id="270f9-414">Der Benutzer hat keine Berechtigung, auf die angeforderte Ressource zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="270f9-414">The user doesn't have permission to access the requested resource.</span></span>

### <a name="40004"></a><span data-ttu-id="270f9-415">40004</span><span class="sxs-lookup"><span data-stu-id="270f9-415">40004</span></span>
<span data-ttu-id="270f9-416">Das OAuth-Token hat nicht den erforderlichen Umfang, um die angeforderte Aktion durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="270f9-416">The OAuth token doesn't have the required scopes to perform the requested action.</span></span> <span data-ttu-id="270f9-417">Siehe [Notizberechtigungen](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="270f9-417">See [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

### <a name="40006"></a><span data-ttu-id="270f9-418">40006</span><span class="sxs-lookup"><span data-stu-id="270f9-418">40006</span></span> 
<span data-ttu-id="270f9-419">Das OAuth-Token hat nicht den erforderlichen Umfang, um die angeforderte Aktion durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="270f9-419">The OAuth token doesn't have the required scopes to perform the requested action.</span></span> <span data-ttu-id="270f9-420">Bearbeiten Sie die Berechtigung entsprechend.</span><span class="sxs-lookup"><span data-stu-id="270f9-420">Specifically the edit permission.</span></span> <span data-ttu-id="270f9-421">Siehe [Notizberechtigungen](permissions-reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="270f9-421">See [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

### <a name="40007"></a><span data-ttu-id="270f9-422">40007</span><span class="sxs-lookup"><span data-stu-id="270f9-422">40007</span></span>
<span data-ttu-id="270f9-423">Der Benutzer hat nicht die Berechtigungen, auf diese Ressource zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="270f9-423">The user does not have permissions to access this resource.</span></span>

### <a name="40008"></a><span data-ttu-id="270f9-424">40008</span><span class="sxs-lookup"><span data-stu-id="270f9-424">40008</span></span>
<span data-ttu-id="270f9-425">Der Zugriff ist für diese Ressource nicht zulässig.</span><span class="sxs-lookup"><span data-stu-id="270f9-425">Access is Forbidden for this resource.</span></span>

### <a name="40009"></a><span data-ttu-id="270f9-426">40009</span><span class="sxs-lookup"><span data-stu-id="270f9-426">40009</span></span>
<span data-ttu-id="270f9-427">Der Container wird bereits von einer anderen Ressource verwendet.</span><span class="sxs-lookup"><span data-stu-id="270f9-427">The container is already in use by another resource.</span></span>

## <a name="see-also"></a><span data-ttu-id="270f9-428">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="270f9-428">See also</span></span>

- [<span data-ttu-id="270f9-429">Microsoft Graph-Fehlerantworten und -Ressourcentypen</span><span class="sxs-lookup"><span data-stu-id="270f9-429">Microsoft Graph error responses and resource types</span></span>](errors.md)
- [<span data-ttu-id="270f9-430">OneNote-Referenz</span><span class="sxs-lookup"><span data-stu-id="270f9-430">OneNote reference</span></span>](/graph/api/resources/onenote?view=graph-rest-1.0)

