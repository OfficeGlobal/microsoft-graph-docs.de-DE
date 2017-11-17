# <a name="error-codes-for-onenote-apis-in-microsoft-graph"></a><span data-ttu-id="36b45-101">Fehlercodes für OneNote-APIs in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="36b45-101">Error codes for OneNote APIs in Microsoft Graph</span></span>

<span data-ttu-id="36b45-102">Dieser Artikel beschreibt Fehlercodes, die von der OneNote-API zurückgegeben werden, wenn eine von der API gesendete Anfrage fehlschlägt.</span><span class="sxs-lookup"><span data-stu-id="36b45-102">This topic describes error and warning codes that are returned by the onnvshort API whenever a request sent through the API fails.</span></span>

## <a name="error-response-example"></a><span data-ttu-id="36b45-103">Fehlerantwort-Beispiel</span><span class="sxs-lookup"><span data-stu-id="36b45-103">Error response example</span></span>
<span data-ttu-id="36b45-104">Wenn Ihre Anforderung einen Fehler generiert, hält die OneNote-API die Ausführung der Anforderung an und gibt eine Fehlerantwort als JSON-Objekt zurück.</span><span class="sxs-lookup"><span data-stu-id="36b45-104">When your request generates an error, the OneNote API stops performing the request and returns an error response as a JSON object.</span></span> <span data-ttu-id="36b45-105">Eine Fehlerantwort enthält den zugehörigen Fehlercode, eine Nachricht und einen Link zum entsprechenden Abschnitt dieses Artikels.</span><span class="sxs-lookup"><span data-stu-id="36b45-105">An error response contains the associated error code, a message, and a link to the appropriate section of this article.</span></span> <span data-ttu-id="36b45-106">Im folgenden Beispiel wird eine Fehlerantwort veranschaulicht.</span><span class="sxs-lookup"><span data-stu-id="36b45-106">The following example shows an Autodiscover error response.</span></span>

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

<span data-ttu-id="36b45-107">Weitere Informationen zu Microsoft Graph-Fehlern finden Sie unter [Microsoft Graph-Fehlerantworten und Ressourcentypen](errors.md).</span><span class="sxs-lookup"><span data-stu-id="36b45-107">For more information about Microsoft Graph errors, see [Microsoft Graph error responses and resource types](errors.md).</span></span>

## <a name="codes-from-10001-to-19999"></a><span data-ttu-id="36b45-108">Codes von 10001-19999</span><span class="sxs-lookup"><span data-stu-id="36b45-108">Codes from 10001 to 19999</span></span>
<span data-ttu-id="36b45-109">Der Dienst hat Probleme oder sendet Informationen zur Anwendung.</span><span class="sxs-lookup"><span data-stu-id="36b45-109">The service is having problems or is sending information to the application.</span></span>

### <a name="10001"></a><span data-ttu-id="36b45-110">10001</span><span class="sxs-lookup"><span data-stu-id="36b45-110">10001</span></span>
<span data-ttu-id="36b45-111">Ein unerwarteter Fehler ist aufgetreten, und die Anforderung ist fehlgeschlagen.</span><span class="sxs-lookup"><span data-stu-id="36b45-111">An unexpected error occurred and the request failed.</span></span>

### <a name="10002"></a><span data-ttu-id="36b45-112">10002</span><span class="sxs-lookup"><span data-stu-id="36b45-112">10002</span></span>
<span data-ttu-id="36b45-113">Der Dienst ist derzeit nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="36b45-113">The service is not currently available.</span></span>

### <a name="10003"></a><span data-ttu-id="36b45-114">10003</span><span class="sxs-lookup"><span data-stu-id="36b45-114">10003</span></span>
<span data-ttu-id="36b45-115">Das Konto des aktuellen Benutzers hat die Maximalanzahl an aktiven Anforderungen überschritten.</span><span class="sxs-lookup"><span data-stu-id="36b45-115">The current user’s account has exceeded the maximum number of active requests. Your app will have to repeat the request.</span></span> <span data-ttu-id="36b45-116">Ihre App muss die Anforderung wiederholen.</span><span class="sxs-lookup"><span data-stu-id="36b45-116">Your app will have to repeat the request.</span></span>

### <a name="10004"></a><span data-ttu-id="36b45-117">10004</span><span class="sxs-lookup"><span data-stu-id="36b45-117">10004</span></span>
<span data-ttu-id="36b45-118">Der Dienst kann keine Seite im angeforderten Abschnitt erstellen, da der Abschnitt kennwortgeschützt ist.</span><span class="sxs-lookup"><span data-stu-id="36b45-118">The service can’t create a page in the requested section because that section is protected by a password.</span></span>

### <a name="10005"></a><span data-ttu-id="36b45-119">10005</span><span class="sxs-lookup"><span data-stu-id="36b45-119">10005</span></span>
<span data-ttu-id="36b45-120">Die Anforderung enthält mehr als die Maximalanzahl an Bildtags, wobei das **data-render-src**-Attribut eine PDF enthält.</span><span class="sxs-lookup"><span data-stu-id="36b45-120">The request contains more than the maximum number of image tags in which the **data-render-src** attribute contains a PDF. See  for more information.</span></span> <span data-ttu-id="36b45-121">Siehe [Hinzufügen von Bildern und Dateien](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files)</span><span class="sxs-lookup"><span data-stu-id="36b45-121">See [Add images and files](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files).</span></span>

### <a name="10006"></a><span data-ttu-id="36b45-122">10006</span><span class="sxs-lookup"><span data-stu-id="36b45-122">10006</span></span>
<span data-ttu-id="36b45-123">Die OneNote-API konnte keine Seite im angegebenen Abschnitt erstellen, da dieser Abschnitt beschädigt ist.</span><span class="sxs-lookup"><span data-stu-id="36b45-123">The oncshort API was unable to create a page in the specified section because that section is corrupt.</span></span>

### <a name="10007"></a><span data-ttu-id="36b45-124">10007</span><span class="sxs-lookup"><span data-stu-id="36b45-124">10007</span></span>
<span data-ttu-id="36b45-p104">Der Server ist zu ausgelastet, um die eingehende Anforderung zu bearbeiten. Bitte versuchen Sie es später erneut.</span><span class="sxs-lookup"><span data-stu-id="36b45-p104">The server is too busy to handle the incoming request at this moment. Please try again later.</span></span>

### <a name="10008"></a><span data-ttu-id="36b45-127">10008</span><span class="sxs-lookup"><span data-stu-id="36b45-127">10008</span></span>
<span data-ttu-id="36b45-128">Eine oder mehrere der Dokumentbibliotheken des OneDrive-Benutzers oder der -Gruppe enthalten mehr als 5.000 OneDrive-Elemente (Notizbücher, Abschnitte, Abschnittsgruppen) und können nicht mithilfe der API abgefragt werden.</span><span class="sxs-lookup"><span data-stu-id="36b45-128">One or more of the document libraries on the user or group's OneDrive contains more than 5000 OneNote items (notebooks, sections, section groups), and cannot be queried using the API.</span></span> <span data-ttu-id="36b45-129">Stellen Sie sicher, dass keine der Benutzer- oder Gruppen-Dokumentbibliotheken mehr als 5.000 OneNote-Elemente enthält.</span><span class="sxs-lookup"><span data-stu-id="36b45-129">Please make sure that none of the user or group's document libraries contains more than 5000 OneNote items.</span></span> <span data-ttu-id="36b45-130">Im [OneNote-Entwicklerblog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) finden Sie Informationen zur Reduzierung der Elemente.</span><span class="sxs-lookup"><span data-stu-id="36b45-130">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10012"></a><span data-ttu-id="36b45-131">10012</span><span class="sxs-lookup"><span data-stu-id="36b45-131">10012</span></span>
<span data-ttu-id="36b45-132">Die Entität kann nicht erstellt oder aktualisiert werden, da aus der Bibliothek, die das Notizbuch enthält, Elemente ausgecheckt werden müssen, bevor diese bearbeitet werden können.</span><span class="sxs-lookup"><span data-stu-id="36b45-132">Unable to create or update the entity because the library that contains the notebook requires items to be checked out before they can be edited.</span></span> <span data-ttu-id="36b45-133">Weitere Informationen finden Sie unter https://support.office.com/en-us/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7.</span><span class="sxs-lookup"><span data-stu-id="36b45-133">For more information, see https://support.office.com/en-us/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7.</span></span>

<span data-ttu-id="36b45-134">Entfernen Sie entweder die Anforderung zum Auschecken aus der Bibliothek oder verschieben Sie das Notizbuch.</span><span class="sxs-lookup"><span data-stu-id="36b45-134">Either remove the check-out requirement from the library, or move the notebook.</span></span>

### <a name="10013"></a><span data-ttu-id="36b45-135">10013</span><span class="sxs-lookup"><span data-stu-id="36b45-135">10013</span></span>
<span data-ttu-id="36b45-136">Eine oder mehrere der Dokumentbibliotheken des OneDrive-Benutzers oder der -Gruppe enthalten mehr als 20.000 Elemente und können nicht für die Abfrage mit der API indexiert werden.</span><span class="sxs-lookup"><span data-stu-id="36b45-136">One or more of the document libraries on the user or group's OneDrive contains more than 20,000 items and cannot be indexed for querying using the API.</span></span> <span data-ttu-id="36b45-137">Stellen Sie sicher, dass keine der Benutzer- oder Gruppen-Dokumentbibliotheken mehr als 20.000 Elemente enthält.</span><span class="sxs-lookup"><span data-stu-id="36b45-137">Please make sure that none of the user or group's document libraries contains more than 20,000 items.</span></span> <span data-ttu-id="36b45-138">Im [OneNote-Entwicklerblog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) finden Sie Informationen zur Reduzierung der Elemente.</span><span class="sxs-lookup"><span data-stu-id="36b45-138">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10014"></a><span data-ttu-id="36b45-139">10014</span><span class="sxs-lookup"><span data-stu-id="36b45-139">10014</span></span>
<span data-ttu-id="36b45-140">Azure Key Vault ist zu ausgelastet, um die eingehende Anforderung zu bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="36b45-140">The server is too busy to handle the incoming request at this moment. Please try again later.</span></span> <span data-ttu-id="36b45-141">Versuchen Sie es später erneut.</span><span class="sxs-lookup"><span data-stu-id="36b45-141">Please try again later.</span></span>

### <a name="10015"></a><span data-ttu-id="36b45-142">10015</span><span class="sxs-lookup"><span data-stu-id="36b45-142">10015</span></span>
<span data-ttu-id="36b45-143">SharePoint ist derzeit nicht verfügbar.</span><span class="sxs-lookup"><span data-stu-id="36b45-143">SharePoint is currently unavailable.</span></span> <span data-ttu-id="36b45-144">Versuchen Sie es später erneut.</span><span class="sxs-lookup"><span data-stu-id="36b45-144">Please try again later.</span></span>

### <a name="10016"></a><span data-ttu-id="36b45-145">10016</span><span class="sxs-lookup"><span data-stu-id="36b45-145">10016</span></span>
<span data-ttu-id="36b45-146">Die Dokumentbibliothek des OneDrive-Benutzers oder der -Gruppe hat den Sicherheitsschwellwert überschritten.</span><span class="sxs-lookup"><span data-stu-id="36b45-146">Document library on the user or group’s OneDrive exceeded unique security scopes threshold limit.</span></span> <span data-ttu-id="36b45-147">Der Sicherheitsschwellwert von 50.000 für die Bibliothek darf nicht überschritten werden.</span><span class="sxs-lookup"><span data-stu-id="36b45-147">The maximum number of unique security scopes set for a library cannot exceed 50,000.</span></span>

### <a name="10017"></a><span data-ttu-id="36b45-148">10017</span><span class="sxs-lookup"><span data-stu-id="36b45-148">10017</span></span>
<span data-ttu-id="36b45-149">Ungültige Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36b45-149">Bad Request</span></span>

### <a name="19999"></a><span data-ttu-id="36b45-150">19999</span><span class="sxs-lookup"><span data-stu-id="36b45-150">19999</span></span>
<span data-ttu-id="36b45-151">Die Anforderung ist fehlgeschlagen, da ein unbekannter Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="36b45-151">The request failed because an undetermined error occurred.</span></span>

## <a name="codes-from-20001-to-29999"></a><span data-ttu-id="36b45-152">Codes von 20001 bis 29999</span><span class="sxs-lookup"><span data-stu-id="36b45-152">Codes from 20001 to 29999</span></span>
<span data-ttu-id="36b45-153">Der Anwendungscode hat einen Fehler gemacht.</span><span class="sxs-lookup"><span data-stu-id="36b45-153">The application code has done something wrong.</span></span>

### <a name="20001"></a><span data-ttu-id="36b45-154">20001</span><span class="sxs-lookup"><span data-stu-id="36b45-154">20001</span></span>

<span data-ttu-id="36b45-155">In der Anforderung fehlt der erforderliche "Präsentation"-Teil.</span><span class="sxs-lookup"><span data-stu-id="36b45-155">The request is missing the required "Presentation" part.</span></span> <span data-ttu-id="36b45-156">Es ist einer erforderlich.</span><span class="sxs-lookup"><span data-stu-id="36b45-156">Exactly one is required.</span></span> 

### <a name="20002"></a><span data-ttu-id="36b45-157">20002</span><span class="sxs-lookup"><span data-stu-id="36b45-157">20002</span></span>
<span data-ttu-id="36b45-158">Die Anforderung enthält zwei oder mehr "Präsentation"-Teile.</span><span class="sxs-lookup"><span data-stu-id="36b45-158">The request contains two or more "Presentation" parts.</span></span> <span data-ttu-id="36b45-159">Es ist einer erforderlich.</span><span class="sxs-lookup"><span data-stu-id="36b45-159">Exactly one is required.</span></span>

### <a name="20003"></a><span data-ttu-id="36b45-160">20003</span><span class="sxs-lookup"><span data-stu-id="36b45-160">20003</span></span>
<span data-ttu-id="36b45-161">Der Inhaltstyp des "Präsentation"-Teils kann nur Text/HTML oder Anwendung/XHTML + XML sein.</span><span class="sxs-lookup"><span data-stu-id="36b45-161">The content type of the "Presentation" part can be only text/HTML or application/XHTML+XML.</span></span> 

### <a name="20004"></a><span data-ttu-id="36b45-162">20004</span><span class="sxs-lookup"><span data-stu-id="36b45-162">20004</span></span>
<span data-ttu-id="36b45-163">Die „Presentation”-Teil-HTML des HTML-Codes enthält ein Bild-Tag mit den festgelegten Eigenschaften **src** und **data-render-src**.</span><span class="sxs-lookup"><span data-stu-id="36b45-163">The "Presentation" part HTML contains an image tag with both the **src** and the **data-render-src** properties set.</span></span> <span data-ttu-id="36b45-164">Die API ignoriert die **src**-Eigenschaft und verwendet die **data-render-src**-Eigenschaft.</span><span class="sxs-lookup"><span data-stu-id="36b45-164">The API will ignore the **src** property and use the **data-render-src** property.</span></span> 

### <a name="20005"></a><span data-ttu-id="36b45-165">20005</span><span class="sxs-lookup"><span data-stu-id="36b45-165">20005</span></span>
<span data-ttu-id="36b45-166">Die Anforderungs-URI ist zu lang.</span><span class="sxs-lookup"><span data-stu-id="36b45-166">The request URI is too long.</span></span> <span data-ttu-id="36b45-167">Der maximale Länge der Anforderungs-URI (einschließlich aller Parameter und Daten) beträgt 16 KB oder 16.384 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="36b45-167">The request URI is too long. The maximum size of the URI (including all parameters and data) is 16 kb or 16,384 characters.</span></span>

### <a name="20006"></a><span data-ttu-id="36b45-168">20006</span><span class="sxs-lookup"><span data-stu-id="36b45-168">20006</span></span>
<span data-ttu-id="36b45-169">Die „Presentation”-Teil-HTML enthält ein Bild-Tag, für das weder eine src- noch eine **data-render-src**-Eigenschaft festgelegt wurde.</span><span class="sxs-lookup"><span data-stu-id="36b45-169">The “Presentation” part HTML contains an image tag with neither the **src** nor the data-render-src properties set. The API will ignore the image tag. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> <span data-ttu-id="36b45-170">Die API ignoriert das **image**-Tag.</span><span class="sxs-lookup"><span data-stu-id="36b45-170">The API will ignore the **image** tag.</span></span> 

### <a name="20007"></a><span data-ttu-id="36b45-171">20007</span><span class="sxs-lookup"><span data-stu-id="36b45-171">20007</span></span>
<span data-ttu-id="36b45-172">Die „Presentation”-Teil-HTML enthält eine Zeichenfolge mit Erstellungsdatum/-Uhrzeit, die keinem zulässigen Format entspricht.</span><span class="sxs-lookup"><span data-stu-id="36b45-172">The “Presentation” part HTML contains a created date/time string that does not match any of the allowed formats. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20008"></a><span data-ttu-id="36b45-173">20008</span><span class="sxs-lookup"><span data-stu-id="36b45-173">20008</span></span>
<span data-ttu-id="36b45-174">Die Anforderung ist zu groß.</span><span class="sxs-lookup"><span data-stu-id="36b45-174">The size of the document is too large.</span></span> 

### <a name="20009"></a><span data-ttu-id="36b45-175">20009</span><span class="sxs-lookup"><span data-stu-id="36b45-175">20009</span></span>
<span data-ttu-id="36b45-176">Die Anforderung enthält Teile mit identischen Namen.</span><span class="sxs-lookup"><span data-stu-id="36b45-176">The request contains parts with duplicate names.</span></span> <span data-ttu-id="36b45-177">Teilnamen müssen eindeutig sein.</span><span class="sxs-lookup"><span data-stu-id="36b45-177">Lookup table names must be unique.</span></span> 

### <a name="20010"></a><span data-ttu-id="36b45-178">20010</span><span class="sxs-lookup"><span data-stu-id="36b45-178">20010</span></span>
<span data-ttu-id="36b45-179">Die Kopfzeile „Content-Disposition“ wurde nicht für den angegebenen Inhaltstyp festgelegt.</span><span class="sxs-lookup"><span data-stu-id="36b45-179">The Content-Disposition header was not supplied for the specified content type.</span></span> 

### <a name="20011"></a><span data-ttu-id="36b45-180">20011</span><span class="sxs-lookup"><span data-stu-id="36b45-180">20011</span></span>
<span data-ttu-id="36b45-181">Die Anforderung enthält eine ungültige mehrteilige Nutzlast.</span><span class="sxs-lookup"><span data-stu-id="36b45-181">The request contains a malformed multipart payload.</span></span> <span data-ttu-id="36b45-182">Das Problem kann durch fehlende Leerzeilen, eine fehlende letzten Zeile, falsch formatierte Teil-Trennzeichen usw. ausgelöst werden.</span><span class="sxs-lookup"><span data-stu-id="36b45-182">Problems could include missing blank lines, a missing last line, incorrectly formatted part separators, and so on.</span></span> <span data-ttu-id="36b45-183">Wenn Sie die mehrteilige Nachricht manuell erstellen, überprüfen Sie sorgfältig die Logik oder ziehen Sie eine Drittanbieter-Bibliothek hinzu.</span><span class="sxs-lookup"><span data-stu-id="36b45-183">If you're building the multipart message by hand, carefully check the logic, or consider using a third-party library.</span></span> 

### <a name="20012"></a><span data-ttu-id="36b45-184">20012</span><span class="sxs-lookup"><span data-stu-id="36b45-184">20012</span></span>
<span data-ttu-id="36b45-185">Die Anforderung stellt keinen Inhaltstyp für das angegebene Teil zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="36b45-185">The request doesn't supply a content type for the specified part.</span></span> 
### <a name="20013"></a><span data-ttu-id="36b45-186">20013</span><span class="sxs-lookup"><span data-stu-id="36b45-186">20013</span></span>
<span data-ttu-id="36b45-187">Die Anforderung stellt keinen Inhaltstyp und keine Kopfzeile für die Content-Disposition für das angegebene Teil zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="36b45-187">The request doesn’t supply Content-Type and Content-Disposition headers for the specified part.</span></span> 

### <a name="20014"></a><span data-ttu-id="36b45-188">20014</span><span class="sxs-lookup"><span data-stu-id="36b45-188">20014</span></span>
<span data-ttu-id="36b45-189">Die Länge eines Teils in der mehrteiligen Nachricht überschreitet die maximale Größe von 25 MB.</span><span class="sxs-lookup"><span data-stu-id="36b45-189">The length of a part in the multi-part message exceeds the maximum size of 25 MB. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20015"></a><span data-ttu-id="36b45-190">20015</span><span class="sxs-lookup"><span data-stu-id="36b45-190">20015</span></span>
<span data-ttu-id="36b45-191">Die Anzahl der Teile in der mehrteiligen Nachricht überschreitet die Begrenzung von 500.</span><span class="sxs-lookup"><span data-stu-id="36b45-191">The count of parts in the multi-part message exceeds the limit of 500. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20016"></a><span data-ttu-id="36b45-192">20016</span><span class="sxs-lookup"><span data-stu-id="36b45-192">20016</span></span>
<span data-ttu-id="36b45-193">Die Länge der mehrteiligen Nachricht überschreitet die maximale Größe von 75 MB.</span><span class="sxs-lookup"><span data-stu-id="36b45-193">The length of the multi-part message exceeds the limit of 75 MB. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20017"></a><span data-ttu-id="36b45-194">20017</span><span class="sxs-lookup"><span data-stu-id="36b45-194">20017</span></span>
<span data-ttu-id="36b45-195">Die E-Mail-MIME ist fehlerhaft.</span><span class="sxs-lookup"><span data-stu-id="36b45-195">The email MIME was malformed.</span></span> 

### <a name="20018"></a><span data-ttu-id="36b45-196">20018</span><span class="sxs-lookup"><span data-stu-id="36b45-196">20018</span></span>
<span data-ttu-id="36b45-197">Die Besprechungs-MIME oder -ICal ist fehlerhaft.</span><span class="sxs-lookup"><span data-stu-id="36b45-197">The meeting MIME or ICal was malformed.</span></span> 

### <a name="20019"></a><span data-ttu-id="36b45-198">20019</span><span class="sxs-lookup"><span data-stu-id="36b45-198">20019</span></span>
<span data-ttu-id="36b45-199">Es wurde kein ICal gefunden.</span><span class="sxs-lookup"><span data-stu-id="36b45-199">No ICal was found.</span></span> 

### <a name="20020"></a><span data-ttu-id="36b45-200">20020</span><span class="sxs-lookup"><span data-stu-id="36b45-200">20020</span></span>
<span data-ttu-id="36b45-201">Es wurde ein fehlerhafter Json-Anforderungstext gefunden.</span><span class="sxs-lookup"><span data-stu-id="36b45-201">Encountered malformed Json in request body.</span></span> 

### <a name="20100"></a><span data-ttu-id="36b45-202">20100</span><span class="sxs-lookup"><span data-stu-id="36b45-202">20100</span></span>
<span data-ttu-id="36b45-203">Etwas stimmt mit der Syntax der Anforderung nicht.</span><span class="sxs-lookup"><span data-stu-id="36b45-203">Something is wrong with the syntax of your request.</span></span> 
### <a name="20101"></a><span data-ttu-id="36b45-204">20101</span><span class="sxs-lookup"><span data-stu-id="36b45-204">20101</span></span>
<span data-ttu-id="36b45-205">Die angeforderte Eigenschaft ist nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="36b45-205">The property that you requested doesn’t exist.</span></span>

### <a name="20102"></a><span data-ttu-id="36b45-206">20102</span><span class="sxs-lookup"><span data-stu-id="36b45-206">20102</span></span>
<span data-ttu-id="36b45-207">Sie haben eine Ressource angefordert, die nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="36b45-207">You requested a resource that doesn’t exist.</span></span>

### <a name="20103"></a><span data-ttu-id="36b45-208">20103</span><span class="sxs-lookup"><span data-stu-id="36b45-208">20103</span></span>
<span data-ttu-id="36b45-209">Die **expand**-Abfrage wird für diese Anforderung nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="36b45-209">The **expand** query is not supported for this request.</span></span> <span data-ttu-id="36b45-210">Siehe [Unterstützte Zeichenfolge-Optionen für OData-Anfragen](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-get-content#query-options).</span><span class="sxs-lookup"><span data-stu-id="36b45-210">Supported OData query string options</span></span>

### <a name="20104"></a><span data-ttu-id="36b45-211">20104</span><span class="sxs-lookup"><span data-stu-id="36b45-211">20104 (SectionNameInvalidChar)</span></span>
<span data-ttu-id="36b45-212">Die **pagelevel**-Abfrageoption wird nur unterstützt, wenn Sie eine Abfrage für die Seitensammlung in einem Abschnitt oder für eine bestimmte Seite ausführen.</span><span class="sxs-lookup"><span data-stu-id="36b45-212">The **pagelevel** query option is supported only when querying for the pages collection in a section or for a specific page. For example:</span></span> <span data-ttu-id="36b45-213">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="36b45-213">For example:</span></span>  

```http
GET ../sections/{id}/pages?pagelevel=true
GET ../pages/{id}?pagelevel=true
```

### <a name="20106"></a><span data-ttu-id="36b45-214">20106</span><span class="sxs-lookup"><span data-stu-id="36b45-214">20106</span></span>
<span data-ttu-id="36b45-215">Ihre Anforderung enthält einen Abfrageoperator, der nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="36b45-215">Your request contains a query operator that is not supported. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20108"></a><span data-ttu-id="36b45-216">20108</span><span class="sxs-lookup"><span data-stu-id="36b45-216">20108</span></span>
<span data-ttu-id="36b45-217">Die Anforderung enthält nicht unterstützte OData-Abfrageparameter.</span><span class="sxs-lookup"><span data-stu-id="36b45-217">Your request contains unsupported OData query parameters.</span></span>

### <a name="20109"></a><span data-ttu-id="36b45-218">20109</span><span class="sxs-lookup"><span data-stu-id="36b45-218">20109</span></span>
<span data-ttu-id="36b45-219">Die Nutzlast in der PATCH-Anforderung wurde nicht ordnungsgemäß erstellt.</span><span class="sxs-lookup"><span data-stu-id="36b45-219">The payload in the PATCH request is not constructed correctly.</span></span>

### <a name="20110"></a><span data-ttu-id="36b45-220">20110</span><span class="sxs-lookup"><span data-stu-id="36b45-220">20110</span></span>
<span data-ttu-id="36b45-221">Bei Anfragen für die Erstellung von Seiten mit Datenteilen muss der Inhalt mehrteilig sein und einen „Präsentation“-Teil enthalten.</span><span class="sxs-lookup"><span data-stu-id="36b45-221">Page create requests with data parts require the content to be multi-part, with a “Presentation” part. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20111"></a><span data-ttu-id="36b45-222">20111</span><span class="sxs-lookup"><span data-stu-id="36b45-222">20111</span></span>
<span data-ttu-id="36b45-223">Ihre Anforderung verwendet ein OData-Feature, das nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="36b45-223">Your request uses an OData feature that isn’t supported.</span></span>

### <a name="20112"></a><span data-ttu-id="36b45-224">20112</span><span class="sxs-lookup"><span data-stu-id="36b45-224">20112</span></span>
<span data-ttu-id="36b45-225">Ihre Anfrage enthält eine ungültige ID für das Ziel-Notebook, die Abschnittsgruppe, den Abschnitt oder die Seitenentität.</span><span class="sxs-lookup"><span data-stu-id="36b45-225">Your request contains an invalid ID for the target notebook, section group, section, or page entity.</span></span>

### <a name="20113"></a><span data-ttu-id="36b45-226">20113</span><span class="sxs-lookup"><span data-stu-id="36b45-226">20113</span></span>
<span data-ttu-id="36b45-227">Die in der Anforderung angegebene Ressource wurde gelöscht.</span><span class="sxs-lookup"><span data-stu-id="36b45-227">The resource specified in the request has been deleted.</span></span>

### <a name="20115"></a><span data-ttu-id="36b45-228">20115</span><span class="sxs-lookup"><span data-stu-id="36b45-228">20115</span></span>
<span data-ttu-id="36b45-229">Der Name enthält ungültige Zeichen.</span><span class="sxs-lookup"><span data-stu-id="36b45-229">The name contains invalid characters.</span></span> <span data-ttu-id="36b45-230">Der Name des Notizbuchs darf die folgenden Zeichen nicht enthalten: `? * \ / : < > | ' "`</span><span class="sxs-lookup"><span data-stu-id="36b45-230">The name contains invalid characters. A notebook name cannot contain any of the following characters: ?*\/:<>|'"</span></span>

### <a name="20117"></a><span data-ttu-id="36b45-231">20117</span><span class="sxs-lookup"><span data-stu-id="36b45-231">20117</span></span>
<span data-ttu-id="36b45-232">Ein Element mit dem angegebenen Namen ist bereits im angegebenen Ort vorhanden.</span><span class="sxs-lookup"><span data-stu-id="36b45-232">An item with the name you specified already exists in the location that you specified.</span></span>

### <a name="20119"></a><span data-ttu-id="36b45-233">20119</span><span class="sxs-lookup"><span data-stu-id="36b45-233">20119</span></span>
<span data-ttu-id="36b45-234">Die HTML im „Presentation“-Teil enthält ein **data-attachment**-Attribut, das kein gültiges Format hat oder einen oder mehrere dieser ungültigen Zeichen für einen Dateinamen enthält: `\ / : * ? < > | "`.</span><span class="sxs-lookup"><span data-stu-id="36b45-234">The HTML in the 'Presentation' part contains a data-attachment attribute that either doesn’t have a valid format or includes one or more of these invalid characters for a file name: \/:*?<>|". The request substituted the value indicated in the error message.</span></span> <span data-ttu-id="36b45-235">Die Anforderung hat den Wert in der Fehlermeldung ersetzt.</span><span class="sxs-lookup"><span data-stu-id="36b45-235">The request substituted the value indicated in the error message.</span></span>

### <a name="20120"></a><span data-ttu-id="36b45-236">20120</span><span class="sxs-lookup"><span data-stu-id="36b45-236">20120</span></span>
<span data-ttu-id="36b45-237">Die Anforderung gibt ein PATCH-Ziel an, das nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="36b45-237">Your request specifies a PATCH target that can’t be located.</span></span>

### <a name="20121"></a><span data-ttu-id="36b45-238">20121</span><span class="sxs-lookup"><span data-stu-id="36b45-238">20121</span></span>
<span data-ttu-id="36b45-239">Die Anforderung enthält ein ungültiges PATCH-Argument.</span><span class="sxs-lookup"><span data-stu-id="36b45-239">Your request contains an invalid PATCH argument. See Update page content.</span></span> <span data-ttu-id="36b45-240">Siehe [Aktualisieren von Seiteninhalt](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="36b45-240">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20122"></a><span data-ttu-id="36b45-241">20122</span><span class="sxs-lookup"><span data-stu-id="36b45-241">20122</span></span>
<span data-ttu-id="36b45-242">Ihre Anforderung gibt eine nicht unterstützte PATCH-Aktion an.</span><span class="sxs-lookup"><span data-stu-id="36b45-242">Your request specifies an unsupported PATCH action. See Update page content.</span></span> <span data-ttu-id="36b45-243">Siehe [Aktualisieren von Seiteninhalt](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="36b45-243">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20123"></a><span data-ttu-id="36b45-244">20123</span><span class="sxs-lookup"><span data-stu-id="36b45-244">20123</span></span>
<span data-ttu-id="36b45-245">Die PATCH-Anforderung kann die angegebene Seite nicht ändern.</span><span class="sxs-lookup"><span data-stu-id="36b45-245">The PATCH request is unable to alter the specified page.</span></span>

### <a name="20124"></a><span data-ttu-id="36b45-246">20124</span><span class="sxs-lookup"><span data-stu-id="36b45-246">20124</span></span>
<span data-ttu-id="36b45-247">Die mehrteilige PATCH-Anforderung beinhaltet keinen „Befehle“-Teil mit der PATCH-Aktion-JSON-Struktur.</span><span class="sxs-lookup"><span data-stu-id="36b45-247">Your multi-part PATCH request doesn’t include a 'commands' part with the PATCH action JSON structure. See Update page content.</span></span> <span data-ttu-id="36b45-248">Siehe [Aktualisieren von Seiteninhalt](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="36b45-248">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20125"></a><span data-ttu-id="36b45-249">20125</span><span class="sxs-lookup"><span data-stu-id="36b45-249">20125</span></span>
<span data-ttu-id="36b45-250">Die PATCH-Anforderung enthält keine Aktionen.</span><span class="sxs-lookup"><span data-stu-id="36b45-250">Your PATCH request contains no actions. See Update page content.</span></span> <span data-ttu-id="36b45-251">Siehe [Aktualisieren von Seiteninhalt](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="36b45-251">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20126"></a><span data-ttu-id="36b45-252">20126</span><span class="sxs-lookup"><span data-stu-id="36b45-252">20126</span></span>
<span data-ttu-id="36b45-253">Der Nachrichtentext enthält entweder falsch formatierten JSON-Code oder Felder, die für diesen Vorgang nicht unterstützt werden.</span><span class="sxs-lookup"><span data-stu-id="36b45-253">The message body contains either incorrectly formatted JSON or fields that are not supported for this operation.</span></span>

### <a name="20127"></a><span data-ttu-id="36b45-254">20127</span><span class="sxs-lookup"><span data-stu-id="36b45-254">20127</span></span>
<span data-ttu-id="36b45-255">Die Anfrage gibt den Namen einer unbekannten Eigenschaft an.</span><span class="sxs-lookup"><span data-stu-id="36b45-255">Your request specifies the name of an unknown property.</span></span>

### <a name="20128"></a><span data-ttu-id="36b45-256">20128</span><span class="sxs-lookup"><span data-stu-id="36b45-256">20128</span></span>
<span data-ttu-id="36b45-257">Die Anforderung enthält einen OData-Syntaxfehler an der in der Nachricht angegebenen Position.</span><span class="sxs-lookup"><span data-stu-id="36b45-257">Your request contains an OData syntax error at the position indicated in the message.</span></span>

### <a name="20129"></a><span data-ttu-id="36b45-258">20129</span><span class="sxs-lookup"><span data-stu-id="36b45-258">20129</span></span>
<span data-ttu-id="36b45-259">Die Anforderung enthält eine **top**-Abfrage-Zeichenfolgeoption, deren Wert zu hoch ist.</span><span class="sxs-lookup"><span data-stu-id="36b45-259">Your request contains a $top query whose value is too high.</span></span> <span data-ttu-id="36b45-260">Der Maximalwert für Seitenabfragen beträgt 100, und der Standardwert ist 20.</span><span class="sxs-lookup"><span data-stu-id="36b45-260">For page queries, the maximum value is 100, and the default value is 20.</span></span>

### <a name="20130"></a><span data-ttu-id="36b45-261">20130</span><span class="sxs-lookup"><span data-stu-id="36b45-261">20130</span></span>
<span data-ttu-id="36b45-262">Die Anforderung enthält einen URI, der zu einer HTTP-Ressource zeigt, die nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="36b45-262">Your request contains a URI that points to an HTTP resource that can’t be found.</span></span>

### <a name="20131"></a><span data-ttu-id="36b45-263">20131</span><span class="sxs-lookup"><span data-stu-id="36b45-263">20131</span></span>
<span data-ttu-id="36b45-264">Die Anforderung enthält einen ungültigen Wert für den Inhaltstyp.</span><span class="sxs-lookup"><span data-stu-id="36b45-264">Your request contains an invalid data-tag attribute value.</span></span> <span data-ttu-id="36b45-265">Verwenden Sie den in der Nachricht angegeben Wert.</span><span class="sxs-lookup"><span data-stu-id="36b45-265">Use the value indicated in the message.</span></span> 

### <a name="20132"></a><span data-ttu-id="36b45-266">20132</span><span class="sxs-lookup"><span data-stu-id="36b45-266">20132</span></span>
<span data-ttu-id="36b45-267">Die Anforderung enthält ungültige Inhalte.</span><span class="sxs-lookup"><span data-stu-id="36b45-267">Your request contains an invalid PATCH argument. See Update page content.</span></span> <span data-ttu-id="36b45-268">Häufige Ursachen hierfür sind eine fehlende Kopfzeile für die Inhaltstyp-Anfrage und/oder keine Inhalte im Textkörper der Anfrage.</span><span class="sxs-lookup"><span data-stu-id="36b45-268">Your request contains invalid content. Common causes for this are a missing Content-Type request header and/or no content in the body of the request. See OneNote API referencehttp://dev.onenote.com/docs for more information.</span></span> 

### <a name="20133"></a><span data-ttu-id="36b45-269">20133</span><span class="sxs-lookup"><span data-stu-id="36b45-269">20133</span></span>
<span data-ttu-id="36b45-270">Die Anforderung gibt ein PATCH-Ziel an, das nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="36b45-270">Your request specifies a PATCH target that is not supported.  See Update page content.</span></span> <span data-ttu-id="36b45-271">Siehe [Aktualisieren von Seiteninhalt](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="36b45-271">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20134"></a><span data-ttu-id="36b45-272">20134</span><span class="sxs-lookup"><span data-stu-id="36b45-272">20134</span></span>
<span data-ttu-id="36b45-273">Ihre Anforderung gibt ein ungültiges Element als Ziel der PATCH-Aktion an.</span><span class="sxs-lookup"><span data-stu-id="36b45-273">Your request specifies an invalid element as the target of the PATCH action.</span></span> <span data-ttu-id="36b45-274">Wenn das Ziel den **data-id**-Bezeichner verwendet, müssen Sie sicherstellen, dass ein Nummernzeichen (#) vorangestellt ist.</span><span class="sxs-lookup"><span data-stu-id="36b45-274">Your request specifies an invalid element as the target of the PATCH action. If the target uses the **data-id** identifier, make sure it's prefixed with a # symbol. See Update page content.</span></span> <span data-ttu-id="36b45-275">Siehe [Aktualisieren von Seiteninhalt](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="36b45-275">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20135"></a><span data-ttu-id="36b45-276">20135</span><span class="sxs-lookup"><span data-stu-id="36b45-276">20135</span></span>
<span data-ttu-id="36b45-277">Die Anforderung gibt einen Entitätstyp an, der für den PATCH-Vorgang nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="36b45-277">Your request specifies an entity type that is not supported for the PATCH operation.</span></span> <span data-ttu-id="36b45-278">Siehe [Aktualisieren von Seiteninhalt](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="36b45-278">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20136"></a><span data-ttu-id="36b45-279">20136</span><span class="sxs-lookup"><span data-stu-id="36b45-279">20136</span></span>
<span data-ttu-id="36b45-280">Ihre Anforderung enthält ein ungültiges oder fehlendes **data-render-src**- oder **data-render-method**-Attribut.</span><span class="sxs-lookup"><span data-stu-id="36b45-280">Your request contains an invalid or missing **data-render-src** or **data-render-method** attribute. See  Enrich captured content with the OneNote API.</span></span> <span data-ttu-id="36b45-281">Siehe [Extrahieren von Daten aus Bildschirmausschnitten](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data).</span><span class="sxs-lookup"><span data-stu-id="36b45-281">See [Extract data from captures](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-extract-data).</span></span>

### <a name="20137"></a><span data-ttu-id="36b45-282">20137</span><span class="sxs-lookup"><span data-stu-id="36b45-282">20137</span></span>
<span data-ttu-id="36b45-283">Die Zielseite unterstützt keine PATCH-Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="36b45-283">The target page does not support PATCH requests.</span></span>

### <a name="20138"></a><span data-ttu-id="36b45-284">20138</span><span class="sxs-lookup"><span data-stu-id="36b45-284">20138</span></span>
<span data-ttu-id="36b45-285">Das Ziel in der PATCH-Anforderung unterstützt die angegebene **append**Aktion nicht.</span><span class="sxs-lookup"><span data-stu-id="36b45-285">The target element type in your PATCH request doesn't support the **append** action. See Update page content.</span></span> <span data-ttu-id="36b45-286">Siehe [Aktualisieren von Seiteninhalt](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="36b45-286">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20139"></a><span data-ttu-id="36b45-287">20139</span><span class="sxs-lookup"><span data-stu-id="36b45-287">20139</span></span>
<span data-ttu-id="36b45-288">Die Anforderung enthält einen ungültigen **data-tag**-Attributwert.</span><span class="sxs-lookup"><span data-stu-id="36b45-288">Your request contains an invalid **data-tag** attribute value.</span></span> <span data-ttu-id="36b45-289">Siehe [Verwenden von Notiztags](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags).</span><span class="sxs-lookup"><span data-stu-id="36b45-289">Use note tags</span></span>

### <a name="20140"></a><span data-ttu-id="36b45-290">20140</span><span class="sxs-lookup"><span data-stu-id="36b45-290">20140</span></span>
<span data-ttu-id="36b45-291">Die Anforderung enthält einen ungültigen **data-tag**-Statuswert.</span><span class="sxs-lookup"><span data-stu-id="36b45-291">Your request contains an invalid **data-tag** attribute value.</span></span> <span data-ttu-id="36b45-292">Kontrollkästchen-Notiztags können den Status **completed** besitzen.</span><span class="sxs-lookup"><span data-stu-id="36b45-292">Check box note tags can have a **completed** status.</span></span> <span data-ttu-id="36b45-293">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="36b45-293">Example:</span></span>
```html
    <p data-tag="to-do:completed">To-do note tag in completed state (checked box in the UI)</p>
```
<span data-ttu-id="36b45-294">Siehe [Verwenden von Notiztags](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-note-tags).</span><span class="sxs-lookup"><span data-stu-id="36b45-294">Use note tags</span></span>

### <a name="20141"></a><span data-ttu-id="36b45-295">20141</span><span class="sxs-lookup"><span data-stu-id="36b45-295">20141</span></span>
<span data-ttu-id="36b45-296">Der Zielelementtyp in der PATCH-Anforderung unterstützt die angegebene Aktion nicht.</span><span class="sxs-lookup"><span data-stu-id="36b45-296">The target in your PATCH request doesn't support the specified action.  See Update page content.</span></span> <span data-ttu-id="36b45-297">Siehe [Aktualisieren von Seiteninhalt](../api-reference/v1.0/api/page_update.md).</span><span class="sxs-lookup"><span data-stu-id="36b45-297">[Update page content](../api-reference/v1.0/api/page_update.md)</span></span>

### <a name="20142"></a><span data-ttu-id="36b45-298">20142</span><span class="sxs-lookup"><span data-stu-id="36b45-298">20142</span></span>
<span data-ttu-id="36b45-299">Ihre Anforderung enthält einen **expand**-Ausdruck für ein übergeordnetes Element untergeordneter Entitäten oder ein untergeordnetes Element übergeordneter Entitäten, der nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="36b45-299">Your request contains an **expand** expression for a parent of child entities or a child of parent entities, which  is not supported. See Supported OData query options.</span></span> <span data-ttu-id="36b45-300">Siehe [Unterstützte Zeichenfolge-Optionen für OData-Anfragen](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-get-content#query-options).</span><span class="sxs-lookup"><span data-stu-id="36b45-300">Supported OData query string options</span></span>

### <a name="20143"></a><span data-ttu-id="36b45-301">20143</span><span class="sxs-lookup"><span data-stu-id="36b45-301">20143</span></span>
<span data-ttu-id="36b45-302">Die OData-Abfrage ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="36b45-302">The OData query is invalid.</span></span>

### <a name="20144"></a><span data-ttu-id="36b45-303">20144</span><span class="sxs-lookup"><span data-stu-id="36b45-303">20144</span></span>
<span data-ttu-id="36b45-304">Die Anforderung enthält einen **expand**-Ausdruck für eine Nicht-Navigationseigenschaft.</span><span class="sxs-lookup"><span data-stu-id="36b45-304">Your request contains  an **expand** expression for a  non-navigation property. Only navigation properties can be expanded.</span></span> <span data-ttu-id="36b45-305">Nur Navigationseigenschaften können erweitert werden.</span><span class="sxs-lookup"><span data-stu-id="36b45-305">Only navigation properties can be expanded.</span></span>

### <a name="20145"></a><span data-ttu-id="36b45-306">20145</span><span class="sxs-lookup"><span data-stu-id="36b45-306">20145</span></span>
<span data-ttu-id="36b45-307">Der **select**- oder **expand**-Ausdruck in der Anforderung enthält einen ungültigen Term.</span><span class="sxs-lookup"><span data-stu-id="36b45-307">The **select** or **expand** expression in your request contains an invalid term.</span></span>

### <a name="20146"></a><span data-ttu-id="36b45-308">20146</span><span class="sxs-lookup"><span data-stu-id="36b45-308">20146</span></span>
<span data-ttu-id="36b45-309">Das `style="position:absolute"`-Attribut wurde für ein Element angegeben, aber das **body**-Element gibt `data-absolute-enabled="true"` nicht an, das jedoch für die Unterstützung der Positionierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="36b45-309">The **style="position:absolute"`style="position:absolute"` attribute is specified on an element, but  the body** element does not specify data-absolute-enabled="true"`data-absolute-enabled="true"`, which is required to support positioning.  All position settings are ignored.</span></span> <span data-ttu-id="36b45-310">Alle Positionseinstellungen werden ignoriert.</span><span class="sxs-lookup"><span data-stu-id="36b45-310">All position settings will be ignored.</span></span> <span data-ttu-id="36b45-311">Siehe [Erstellen von absolut positionierten Elementen](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span><span class="sxs-lookup"><span data-stu-id="36b45-311">See [Create absolute positioned elements](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span></span>

### <a name="20147"></a><span data-ttu-id="36b45-312">20147</span><span class="sxs-lookup"><span data-stu-id="36b45-312">20147</span></span>
<span data-ttu-id="36b45-313">Das `style="position:absolute"`-Attribut ist für ein Element angegeben, das kein direkt untergeordnetes Element des **body**-Elemente ist, welches nicht unterstützt wird.</span><span class="sxs-lookup"><span data-stu-id="36b45-313">The `style="position:absolute"` attribute is specified on an element that is not a direct child of the **body** element, which is not supported.</span></span> <span data-ttu-id="36b45-314">Wenn das Element **div**, **img** oder **object** ist, muss es als untergeordnetes Element des Textkörpers angegeben werden; andernfalls werden die Positionseinstellungen ignoriert und die dazugehörigen Inhalte werden als absolut positioniertes div dargestellt.</span><span class="sxs-lookup"><span data-stu-id="36b45-314">20147 The **style="position:absolute"** attribute is specified on an element that is not a direct child of the **body** element, which is not supported. If the element is a **div**, img, or object, make it a direct child of the body; otherwise the position settings will be ignored and its content will render inside an absolutely positioned div.</span></span> <span data-ttu-id="36b45-315">Siehe [Erstellen von absolut positionierten Elementen](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span><span class="sxs-lookup"><span data-stu-id="36b45-315">See [Create absolute positioned elements](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span></span>

### <a name="20148"></a><span data-ttu-id="36b45-316">20148</span><span class="sxs-lookup"><span data-stu-id="36b45-316">20148</span></span>
<span data-ttu-id="36b45-317">Das `style="position:absolute"`-Attribut ist für einen nicht unterstützten Elementyp angegeben.</span><span class="sxs-lookup"><span data-stu-id="36b45-317">20148  The  style="position:absolute"`style="position:absolute"` attribute is specified on an element type that does not  support it.  Only div, img, and object elements support positioning.</span></span> <span data-ttu-id="36b45-318">Nur **div**-, **img**- und **object**-Elemente, die direkt untergeordnete Elemente des Seitentextes sind, unterstützten die Positionierung.</span><span class="sxs-lookup"><span data-stu-id="36b45-318">The  **style="position:absolute"** attribute is specified on an element type that does not  support it.  Only **div**, **img**, and object elements that are direct children of the page body support positioning.</span></span> <span data-ttu-id="36b45-319">Siehe [Erstellen von absolut positionierten Elementen](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span><span class="sxs-lookup"><span data-stu-id="36b45-319">See [Create absolute positioned elements](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-abs-pos).</span></span>

### <a name="20149"></a><span data-ttu-id="36b45-320">20149</span><span class="sxs-lookup"><span data-stu-id="36b45-320">20149</span></span>
<span data-ttu-id="36b45-321">Die Anforderung gibt ein Zielelement an, das nicht gefunden werden kann.</span><span class="sxs-lookup"><span data-stu-id="36b45-321">Your request specifies a target element that cannot be found.</span></span>

### <a name="20150"></a><span data-ttu-id="36b45-322">20150</span><span class="sxs-lookup"><span data-stu-id="36b45-322">20150</span></span>
<span data-ttu-id="36b45-323">Die Anforderung ist für diesen Authentifizierungstyp nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="36b45-323">The request is not valid for this authentication type. Use the ../me/notes/ path  instead.</span></span> <span data-ttu-id="36b45-324"> Verwenden Sie stattdessen den `../me/onenote/`-Pfad.</span><span class="sxs-lookup"><span data-stu-id="36b45-324">Use the `../me/onenote/` path instead.</span></span>

### <a name="20151"></a><span data-ttu-id="36b45-325">20151</span><span class="sxs-lookup"><span data-stu-id="36b45-325">20151</span></span>
<span data-ttu-id="36b45-326">Die Anforderung ist für diesen Authentifizierungstyp nicht gültig.</span><span class="sxs-lookup"><span data-stu-id="36b45-326">The request is not valid for this authentication type. Use the ../me/notes/ path  instead.</span></span> <span data-ttu-id="36b45-327">Verwenden Sie den `../me/onenote/section/{id}/pages`-Endpunkt, um eine Seite in einem bestimmten Abschnitt zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="36b45-327">The request is not valid for this authentication type. Use the ../me/notes/section/{id}/pages`../me/onenote/section/{id}/pages` endpoint to create a page in a specific section.</span></span>

### <a name="20152"></a><span data-ttu-id="36b45-328">20152</span><span class="sxs-lookup"><span data-stu-id="36b45-328">20152 (EntityNameEmpty)</span></span>
<span data-ttu-id="36b45-329">Es ist kein Namenswert für die Entität vorhanden.</span><span class="sxs-lookup"><span data-stu-id="36b45-329">There is no name value specified for the entity. The name must be defined, and it cannot contain whitespaces only.</span></span> <span data-ttu-id="36b45-330">Der Name muss definiert werden und darf nicht nur Leerzeichen enthalten.</span><span class="sxs-lookup"><span data-stu-id="36b45-330">There is no name value specified for the entity. The name must be defined, and it cannot contain whitespaces only.</span></span>

### <a name="20153"></a><span data-ttu-id="36b45-331">20153</span><span class="sxs-lookup"><span data-stu-id="36b45-331">20153 (EntityNameInvalidChar)</span></span>
<span data-ttu-id="36b45-332">Der Entitätsname enthält ungültige Zeichen.</span><span class="sxs-lookup"><span data-stu-id="36b45-332">The entity name contains invalid characters.</span></span> <span data-ttu-id="36b45-333">Der Name darf die folgenden Zeichen nicht enthalten: `? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="36b45-333">The entity name contains invalid characters. The name cannot contain the following characters: ?*\/:<>|&#''%~</span></span>

### <a name="20154"></a><span data-ttu-id="36b45-334">20154</span><span class="sxs-lookup"><span data-stu-id="36b45-334">20154 (EntityNameInvalidStart)</span></span>
<span data-ttu-id="36b45-335">Der Entitätsname darf nicht mit einem Leerzeichen beginnen.</span><span class="sxs-lookup"><span data-stu-id="36b45-335">The entity name cannot start with a space.</span></span>

### <a name="20155"></a><span data-ttu-id="36b45-336">20155</span><span class="sxs-lookup"><span data-stu-id="36b45-336">20155 (EntityNameTooLong)</span></span>
<span data-ttu-id="36b45-337">Der Entitätsname ist zu lang.</span><span class="sxs-lookup"><span data-stu-id="36b45-337">The name is too long.</span></span> <span data-ttu-id="36b45-338">Namen für Notizbücher dürfen maximal 128 Zeichen lang sein.</span><span class="sxs-lookup"><span data-stu-id="36b45-338">Notebook names have a 128-character limit.</span></span> <span data-ttu-id="36b45-339">Andere Entitätsnamen dürfen maximal 50 Zeichen lang sein.</span><span class="sxs-lookup"><span data-stu-id="36b45-339">Other entity names have a 50-character limit.</span></span>

### <a name="20156"></a><span data-ttu-id="36b45-340">20156</span><span class="sxs-lookup"><span data-stu-id="36b45-340">20156</span></span>
<span data-ttu-id="36b45-341">Die angegebene ID für die Zielressource ist nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="36b45-341">The specified ID for the destination resource does not exist.</span></span>

### <a name="20157"></a><span data-ttu-id="36b45-342">20157</span><span class="sxs-lookup"><span data-stu-id="36b45-342">20157</span></span>
<span data-ttu-id="36b45-343">Die angegebene ID für die Zielentität ist ungültig.</span><span class="sxs-lookup"><span data-stu-id="36b45-343">The specified ID for the destination entity is invalid.</span></span>

### <a name="20158"></a><span data-ttu-id="36b45-344">20158</span><span class="sxs-lookup"><span data-stu-id="36b45-344">20158</span></span>
<span data-ttu-id="36b45-345">Die Metadaten für die Website-URL in der angegebenen Anfrage können nicht abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="36b45-345">Unable to get metadata for the site URL specified in the request.</span></span> <span data-ttu-id="36b45-346">Überprüfen Sie das Format der angegebenen URL.</span><span class="sxs-lookup"><span data-stu-id="36b45-346">Check the format of the supplied URL.</span></span> <span data-ttu-id="36b45-347">Zu den unterstützten Formate gehören `https://domain.sharepoint.com/site-a` und `https://domain.com/sites/site-a`.</span><span class="sxs-lookup"><span data-stu-id="36b45-347">Supported formats include `https://domain.sharepoint.com/site-a` and `https://domain.com/sites/site-a`.</span></span>

### <a name="20160"></a><span data-ttu-id="36b45-348">20160</span><span class="sxs-lookup"><span data-stu-id="36b45-348">20160</span></span>
<span data-ttu-id="36b45-349">Es kann keine einheitliche Office 365-Gruppe mit der angegebenen ID gefunden werden.</span><span class="sxs-lookup"><span data-stu-id="36b45-349">Unable to find an Office 365 unified group that has the specified ID.</span></span>

### <a name="20161"></a><span data-ttu-id="36b45-350">20161</span><span class="sxs-lookup"><span data-stu-id="36b45-350">20161</span></span>
<span data-ttu-id="36b45-351">Der Kontext gibt keine gültige Benutzer-ID an.</span><span class="sxs-lookup"><span data-stu-id="36b45-351">The context does not specify a valid user ID.</span></span> <span data-ttu-id="36b45-352">Ein häufiger Fehler ist, dass die PUID/CID in Langform statt als Hexadezimalwert übergeben wurde.</span><span class="sxs-lookup"><span data-stu-id="36b45-352">The  context does not specify a valid user ID. One common error is that PUID/CID was passed in as a long instead of a hex.</span></span>

### <a name="20166"></a><span data-ttu-id="36b45-353">20166</span><span class="sxs-lookup"><span data-stu-id="36b45-353">20166</span></span>
<span data-ttu-id="36b45-354">Die Anwendung hat zu viele Anfragen im Auftrag eines Benutzers innerhalb eines kurzen Zeitraums ausgegeben.</span><span class="sxs-lookup"><span data-stu-id="36b45-354">The application has issued too many requests on behalf of a user in a short period of time.</span></span> <span data-ttu-id="36b45-355">Um sicherzustellen, dass die OneNote-API stabil und reaktionsschnell bleibt, gibt die API den Statuscode 429 und diesen Fehler aus, wenn sie erkennt, dass eine Anwendung zu viele Ressourcen verwendet.</span><span class="sxs-lookup"><span data-stu-id="36b45-355">To help ensure that the OneNote API remains stable and responsive, the API returns a 429 status code and this error when it detects that an application is using too many resources.</span></span> 

<span data-ttu-id="36b45-356">Weitere Informationen finden Sie unter [Drosselung von OneNote-API und wie Sie dies vermeiden](http://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span><span class="sxs-lookup"><span data-stu-id="36b45-356">For more information, see [OneNote API throttling and how to avoid it](http://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span></span>

### <a name="20168"></a><span data-ttu-id="36b45-357">20168</span><span class="sxs-lookup"><span data-stu-id="36b45-357">20168</span></span>
<span data-ttu-id="36b45-358">Die in der Anfrage angegebene Video-Quelle wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="36b45-358">The video source specified in the request is not supported.</span></span> <span data-ttu-id="36b45-359">Eine aktuelle Liste finden Sie unter [Unterstützte Video-Websites](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos).</span><span class="sxs-lookup"><span data-stu-id="36b45-359">See [Supported video sites](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-images-files#videos) for the current list.</span></span>


## <a name="codes-from-30001-to-39999"></a><span data-ttu-id="36b45-360">Codes von 30001 bis 39999</span><span class="sxs-lookup"><span data-stu-id="36b45-360">Codes from 30001 to 39999</span></span>
<span data-ttu-id="36b45-361">Etwas stimmt nicht mit dem Benutzerkonto.</span><span class="sxs-lookup"><span data-stu-id="36b45-361">Something is wrong with the user’s account.</span></span>

### <a name="30101"></a><span data-ttu-id="36b45-362">30101</span><span class="sxs-lookup"><span data-stu-id="36b45-362">30101</span></span>
<span data-ttu-id="36b45-363">Das Benutzerkonto hat das OneDrive-Kontingent überschritten.</span><span class="sxs-lookup"><span data-stu-id="36b45-363">The user account has exceeded its OneDrive quota.</span></span> <span data-ttu-id="36b45-364">Siehe [OneDrive](https://onedrive.live.com/about/en-us/).</span><span class="sxs-lookup"><span data-stu-id="36b45-364">See [OneDrive](https://onedrive.live.com/about/en-us/).</span></span>

### <a name="30102"></a><span data-ttu-id="36b45-365">30102</span><span class="sxs-lookup"><span data-stu-id="36b45-365">30102</span></span>
<span data-ttu-id="36b45-366">Es kann nichts mehr zum angeforderten Abschnitt hinzugefügt werden, da dieser seine maximale Größe ereicht hat.</span><span class="sxs-lookup"><span data-stu-id="36b45-366">Nothing more can be added to the requested section because it has reached its maximum size.</span></span>

### <a name="30103"></a><span data-ttu-id="36b45-367">30103</span><span class="sxs-lookup"><span data-stu-id="36b45-367">30103</span></span>
<span data-ttu-id="36b45-368">Der Ressourceverbrauch ist zu hoch für die Anforderung.</span><span class="sxs-lookup"><span data-stu-id="36b45-368">Resource consumption is too high for the request.</span></span> <span data-ttu-id="36b45-369">Entweder weist das Benutzerkonto ein zu großes Datenset auf, oder der Dienst erhält eine große Anzahl konkurrierender Anforderungen für dieselbe Website (z. B. die persönliche Website des Benutzers oder eine Teamwebsite).</span><span class="sxs-lookup"><span data-stu-id="36b45-369">The level of resource consumption is too high. Either the target user account  has a large dataset or the service is receiving a high number of concurrent requests to the same site (for example, the user's personal site or a team site).</span></span>

### <a name="30104"></a><span data-ttu-id="36b45-370">30104</span><span class="sxs-lookup"><span data-stu-id="36b45-370">30104</span></span>
<span data-ttu-id="36b45-371">Das Benutzerkonto wurde angehalten.</span><span class="sxs-lookup"><span data-stu-id="36b45-371">The user account has been suspended.</span></span>

### <a name="30105"></a><span data-ttu-id="36b45-372">30105</span><span class="sxs-lookup"><span data-stu-id="36b45-372">30105</span></span>
<span data-ttu-id="36b45-373">Die persönliche OneDrive for Business-Website des Benutzers, die für den Zugriff auf Notizbücher erforderlich ist,  wird nicht bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="36b45-373">The user's personal OneDrive for Business site is not provisioned, which is required to access notebooks.</span></span> <span data-ttu-id="36b45-374">Der OneNote-Dienst stellt die Seite jetzt bereit.</span><span class="sxs-lookup"><span data-stu-id="36b45-374">The OneNote service will provision the site now.</span></span> <span data-ttu-id="36b45-375">Dieser Vorgang kann mehrere Minuten dauern.</span><span class="sxs-lookup"><span data-stu-id="36b45-375">This process may take several minutes.</span></span>

### <a name="30106"></a><span data-ttu-id="36b45-376">30106</span><span class="sxs-lookup"><span data-stu-id="36b45-376">30106</span></span>
<span data-ttu-id="36b45-377">OneDrive for Business wird für den Benutzer bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="36b45-377">OneDrive for Business is being provisioned for the user.</span></span>

### <a name="30108"></a><span data-ttu-id="36b45-378">30108</span><span class="sxs-lookup"><span data-stu-id="36b45-378">30108</span></span>
<span data-ttu-id="36b45-379">Das persönliche OneDrive for Business des Benutzers konnte nicht abgerufen werden.</span><span class="sxs-lookup"><span data-stu-id="36b45-379">The user's personal OneDrive for Business could not be retrieved.</span></span> <span data-ttu-id="36b45-380">Die folgende Tabelle enthält mögliche Ursachen.</span><span class="sxs-lookup"><span data-stu-id="36b45-380">The following table lists some possible causes.</span></span>

| <span data-ttu-id="36b45-381">Ursache</span><span class="sxs-lookup"><span data-stu-id="36b45-381">Cause</span></span> | <span data-ttu-id="36b45-382">Lösung</span><span class="sxs-lookup"><span data-stu-id="36b45-382">Resolution</span></span> |
|:------|:------|
| <span data-ttu-id="36b45-383">Die persönliche Website des Benutzers wurde nicht bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="36b45-383">The user's personal site has not been provisioned.</span></span> | <span data-ttu-id="36b45-384">Der Benutzer sollte OneDrive for Business öffnen und die Anweisungen befolgen, um die Website bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="36b45-384">The user should open OneDrive for Business and follow any instructions to provision the site.</span></span> <span data-ttu-id="36b45-385">Wenn dies fehlschlägt, sollten er sich an seinen Office 365-Mandanten-Administrator wenden.</span><span class="sxs-lookup"><span data-stu-id="36b45-385">If this fails, they should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="36b45-386">Die persönliche Website des Benutzers wird derzeit bereitgestellt.</span><span class="sxs-lookup"><span data-stu-id="36b45-386">The user's personal site is currently being provisioned.</span></span> | <span data-ttu-id="36b45-387">Senden Sie die Anforderung später erneut.</span><span class="sxs-lookup"><span data-stu-id="36b45-387">Try the request later.</span></span> |
| <span data-ttu-id="36b45-388">Der Benutzer besitzt keine gültige OneDrive for Business-Lizenz.</span><span class="sxs-lookup"><span data-stu-id="36b45-388">The user does not have a valid OneDrive for Business license.</span></span> | <span data-ttu-id="36b45-389">Der Benutzer sollte sich an seinen Office 365-Mandanten-Administrator wenden.</span><span class="sxs-lookup"><span data-stu-id="36b45-389">The user should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="36b45-390">Die Anfrage konnte aufgrund eines Netzwerkfehlers nicht erfolgreich versendet werden.</span><span class="sxs-lookup"><span data-stu-id="36b45-390">A network issue prevented the request from being successfully sent.</span></span> | <span data-ttu-id="36b45-391">Senden Sie die Anforderung später erneut.</span><span class="sxs-lookup"><span data-stu-id="36b45-391">Try the request later.</span></span> |

### <a name="30109"></a><span data-ttu-id="36b45-392">30109</span><span class="sxs-lookup"><span data-stu-id="36b45-392">30109</span></span>
<span data-ttu-id="36b45-393">Einige Benutzer in der Anforderung sind nicht vorhanden.</span><span class="sxs-lookup"><span data-stu-id="36b45-393">Some users in the request do not exist.</span></span>

### <a name="30110"></a><span data-ttu-id="36b45-394">30110</span><span class="sxs-lookup"><span data-stu-id="36b45-394">30110</span></span>
<span data-ttu-id="36b45-395">Student Information Services wurde nicht für diesen Mandanten registriert.</span><span class="sxs-lookup"><span data-stu-id="36b45-395">Student Information Services has not been registered for this tenant.</span></span>

### <a name="30111"></a><span data-ttu-id="36b45-396">30111</span><span class="sxs-lookup"><span data-stu-id="36b45-396">30111</span></span>
<span data-ttu-id="36b45-397">Es ist ein allgemeiner Fehler mit Student Information Services aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="36b45-397">There is a generic error with Student Information Services.</span></span>

### <a name="30112"></a><span data-ttu-id="36b45-398">30112</span><span class="sxs-lookup"><span data-stu-id="36b45-398">30112</span></span>
<span data-ttu-id="36b45-399">Mehrere Benutzer, die von dieser Anforderung betroffen waren, besitzen den gleichen Benutzernamen.</span><span class="sxs-lookup"><span data-stu-id="36b45-399">Multiple users affected by the request had the same username.</span></span>

### <a name="30113"></a><span data-ttu-id="36b45-400">30113</span><span class="sxs-lookup"><span data-stu-id="36b45-400">30113</span></span>
<span data-ttu-id="36b45-401">Das Notizbuch ist nicht für Einladungen konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="36b45-401">The notebook is not configured to allow invites.</span></span>

### <a name="30114"></a><span data-ttu-id="36b45-402">30114</span><span class="sxs-lookup"><span data-stu-id="36b45-402">30114</span></span>
<span data-ttu-id="36b45-403">Ein erforderlicher Parameter fehlt.</span><span class="sxs-lookup"><span data-stu-id="36b45-403">There is a required parameter missing.</span></span>

## <a name="codes-from-40001-to-49999"></a><span data-ttu-id="36b45-404">Codes von 40001 bis 49999</span><span class="sxs-lookup"><span data-stu-id="36b45-404">Codes from 40001 to 49999</span></span>
<span data-ttu-id="36b45-405">Der Benutzer oder die Anwendung besitzt nicht die erforderlichen Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="36b45-405">The user or application does not have the correct permissions.</span></span>

### <a name="40001"></a><span data-ttu-id="36b45-406">40001</span><span class="sxs-lookup"><span data-stu-id="36b45-406">40001</span></span>
<span data-ttu-id="36b45-407">Die Anforderung enthält kein gültiges OAuth-Token.</span><span class="sxs-lookup"><span data-stu-id="36b45-407">The request doesn’t contain a valid OAuth token. See  and  for more information.</span></span> <span data-ttu-id="36b45-408">Siehe [Notizberechtigungen](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="36b45-408">See [Notes permissions](permissions_reference.md#notes-permissions).</span></span>

### <a name="40002"></a><span data-ttu-id="36b45-409">40002</span><span class="sxs-lookup"><span data-stu-id="36b45-409">40002</span></span>
<span data-ttu-id="36b45-410">Der Benutzer hat keine Berechtigung, an den angeforderten Ort zu schreiben.</span><span class="sxs-lookup"><span data-stu-id="36b45-410">The user doesn’t have permission to write to the requested location.</span></span>

### <a name="40003"></a><span data-ttu-id="36b45-411">40003</span><span class="sxs-lookup"><span data-stu-id="36b45-411">40003</span></span>
<span data-ttu-id="36b45-412">Der Benutzer hat keine Berechtigung, auf die angeforderte Ressource zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="36b45-412">The user doesn’t have permission to get access to the requested resource.</span></span>

### <a name="40004"></a><span data-ttu-id="36b45-413">40004</span><span class="sxs-lookup"><span data-stu-id="36b45-413">40004</span></span>
<span data-ttu-id="36b45-414">Das OAuth-Token hat nicht den erforderlichen Umfang, um die angeforderte Aktion durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="36b45-414">The OAuth token doesn’t have the required scopes to perform the requested action. See  for more information.</span></span> <span data-ttu-id="36b45-415">Siehe [Notizberechtigungen](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="36b45-415">See [Notes permissions](permissions_reference.md#notes-permissions).</span></span>

### <a name="40006"></a><span data-ttu-id="36b45-416">40006</span><span class="sxs-lookup"><span data-stu-id="36b45-416">40006</span></span> 
<span data-ttu-id="36b45-417">Das OAuth-Token hat nicht den erforderlichen Umfang, um die angeforderte Aktion durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="36b45-417">The OAuth token doesn’t have the required scopes to perform the requested action. See  for more information.</span></span> <span data-ttu-id="36b45-418">Bearbeiten Sie die Berechtigung entsprechend.</span><span class="sxs-lookup"><span data-stu-id="36b45-418">Specifically the edit permission.</span></span> <span data-ttu-id="36b45-419">Siehe [Notizberechtigungen](permissions_reference.md#notes-permissions).</span><span class="sxs-lookup"><span data-stu-id="36b45-419">See [Notes permissions](permissions_reference.md#notes-permissions).</span></span>

### <a name="40007"></a><span data-ttu-id="36b45-420">40007</span><span class="sxs-lookup"><span data-stu-id="36b45-420">40007</span></span>
<span data-ttu-id="36b45-421">Der Benutzer hat nicht die Berechtigungen, auf diese Ressource zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="36b45-421">The user does not have permissions to access this resource.</span></span>

### <a name="40008"></a><span data-ttu-id="36b45-422">40008</span><span class="sxs-lookup"><span data-stu-id="36b45-422">40008</span></span>
<span data-ttu-id="36b45-423">Der Zugriff ist für diese Ressource nicht zulässig.</span><span class="sxs-lookup"><span data-stu-id="36b45-423">Access is Forbidden for this resource.</span></span>

### <a name="40009"></a><span data-ttu-id="36b45-424">40009</span><span class="sxs-lookup"><span data-stu-id="36b45-424">40009</span></span>
<span data-ttu-id="36b45-425">Der Container wird bereits von einer anderen Ressource verwendet.</span><span class="sxs-lookup"><span data-stu-id="36b45-425">The container is already in use by another resource.</span></span>

## <a name="see-also"></a><span data-ttu-id="36b45-426">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="36b45-426">See also</span></span>

- [<span data-ttu-id="36b45-427">Microsoft Graph-Fehlerantworten und -Ressourcentypen</span><span class="sxs-lookup"><span data-stu-id="36b45-427">Microsoft Graph error responses and resource types</span></span>](errors.md)
- [<span data-ttu-id="36b45-428">OneNote-Referenz</span><span class="sxs-lookup"><span data-stu-id="36b45-428">OneNote JavaScript API reference</span></span>](../api-reference/v1.0/resources/onenote.md)

