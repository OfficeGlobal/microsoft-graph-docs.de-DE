# <a name="manage-sessions-and-persistence-in-excel-with-microsoft-graph"></a><span data-ttu-id="236f0-101">Verwalten von Sitzungen und Persistenz in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="236f0-101">Manage sessions and persistence in Excel with Microsoft Graph</span></span>

<span data-ttu-id="236f0-102">Wenn Ihre Anwendung mehr als nur ein oder zwei Aufrufe an die Excel-API durchführen muss, müssen Sie eine Sitzung erstellen und die Sitzungs-ID mit jeder Anforderung übergeben.</span><span class="sxs-lookup"><span data-stu-id="236f0-102">If your application needs to make more than one or two calls to the Excel API, you should create a session and pass the session Id with each request.</span></span> <span data-ttu-id="236f0-103">Indem Sie eine Sitzungs-ID in die Anforderungen einschließen, wird sichergestellt, dass Sie die Excel-API auf möglichst effiziente Weise verwenden.</span><span class="sxs-lookup"><span data-stu-id="236f0-103">The presence of a session Id in the requests ensures that you are using the Excel API in the most efficient way possible.</span></span>

<span data-ttu-id="236f0-104">Excel-APIs können in einem der drei folgenden Modi aufgerufen werden:</span><span class="sxs-lookup"><span data-stu-id="236f0-104">Excel APIs can be called in one of three modes:</span></span>

1. <span data-ttu-id="236f0-105">**Beständige Sitzung**: Alle an der Arbeitsmappe vorgenommenen Änderungen werden gespeichert (beständig gemacht).</span><span class="sxs-lookup"><span data-stu-id="236f0-105">Persistent session - All changes made to the workbook are persisted (saved).</span></span> <span data-ttu-id="236f0-106">Dies ist die effizienteste und leistungsfähigste Möglichkeit zur Verwendung der Excel-API.</span><span class="sxs-lookup"><span data-stu-id="236f0-106">This is the most efficient and best-performing way to use the Excel API.</span></span>
2. <span data-ttu-id="236f0-107">**Nicht beständige Sitzung**: Die von der API vorgenommenen Änderungen werden nicht am Quellspeicherort gespeichert.</span><span class="sxs-lookup"><span data-stu-id="236f0-107">**Non-persistent session**  Changes made by the API are not saved to the source location.</span></span> <span data-ttu-id="236f0-108">Stattdessen behält der Excel-Back-End-Server eine temporäre Kopie der Datei bei, welche die während dieser API-Sitzung vorgenommenen Änderungen enthält.</span><span class="sxs-lookup"><span data-stu-id="236f0-108">Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session.</span></span> <span data-ttu-id="236f0-109">Wenn die Excel-Sitzung abläuft, gehen die Änderungen verloren.</span><span class="sxs-lookup"><span data-stu-id="236f0-109">When the Excel session expires, the changes are lost.</span></span> <span data-ttu-id="236f0-110">Dieser Modus eignet sich für Apps, die Analysen durchführen oder die Ergebnisse einer Berechnung oder eines Diagrammbilds abrufen, aber nicht den Dokumentstatus betreffen.</span><span class="sxs-lookup"><span data-stu-id="236f0-110">This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but do not need to affect the document state.</span></span>
3. <span data-ttu-id="236f0-111">**Sitzungslos**: Die API-Aufrufe übergeben keine Sitzungs-ID. Die Excel-Server müssen die Serverkopie der Arbeitsmappe für jeden Vorgang suchen.</span><span class="sxs-lookup"><span data-stu-id="236f0-111">**Sessionless**  The API calls do not pass a session Id. The Excel servers have to locate the server's copy of the workbook for each operation.</span></span> <span data-ttu-id="236f0-112">Dies ist keine effiziente Methode zum Aufrufen der Excel-API. Sie eignet sich jedoch für bestimmte Arten von isolierten Anforderungen.</span><span class="sxs-lookup"><span data-stu-id="236f0-112">This is not an efficient way to call the Excel API, but it is suitable for making certain types of isolated requests.</span></span>

<span data-ttu-id="236f0-113">Um die Sitzung in der API darzustellen, verwenden Sie den `workbook-session-id: {session-id}`-Header.</span><span class="sxs-lookup"><span data-stu-id="236f0-113">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span>

><span data-ttu-id="236f0-p105">**Hinweis:** Der Sitzungsheader ist für das Funktionieren einer Excel-API nicht erforderlich. Die Verwendung des Sitzungsheaders wird jedoch empfohlen, um die Leistung zu verbessern. Wenn Sie keinen Sitzungsheader verwenden, _werden_ die während des API-Aufrufs vorgenommenen Änderungen in der Datei gespeichert.</span><span class="sxs-lookup"><span data-stu-id="236f0-p105">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="next-step"></a><span data-ttu-id="236f0-117">Nächster Schritt</span><span class="sxs-lookup"><span data-stu-id="236f0-117">Next step</span></span>
<span data-ttu-id="236f0-118">Informationen zum Erstellen und Verwenden von Sitzungen finden Sie unter [Erstellen von Sitzungsreferenzen](../api-reference/v1.0/api/workbook_createsession.md).</span><span class="sxs-lookup"><span data-stu-id="236f0-118">To learn how to create and use sessions, see the [Create session reference topic](../api-reference/v1.0/api/workbook_createsession.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="236f0-119">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="236f0-119">See also</span></span>
* [<span data-ttu-id="236f0-120">Schreiben in eine Excel-Arbeitsmappe mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="236f0-120">Write to an Excel workbook using Microsoft Graph</span></span>](excel-write-to-workbook.md)
* [<span data-ttu-id="236f0-121">Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="236f0-121">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="236f0-122">Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="236f0-122">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="236f0-123">Anzeigen eines Diagrammbilds in Excel mithilfe von Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="236f0-123">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="236f0-124">Verwenden der Excel-REST-API</span><span class="sxs-lookup"><span data-stu-id="236f0-124">Use the Excel REST API</span></span>](../api-reference/v1.0/resources/excel.md)