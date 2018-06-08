# <a name="write-data-to-an-excel-workbook-with-microsoft-graph"></a><span data-ttu-id="a2a7f-101">Schreiben von Daten in eine Excel-Arbeitsmappe mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a2a7f-101">Write data to an Excel workbook with Microsoft Graph</span></span>

<span data-ttu-id="a2a7f-102">Die Excel REST-API bietet eine einfache und plattformunabhängige Methode zum Hochladen von Informationen in eine Excel-Arbeitsmappe.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-102">The Excel REST API provides an easy, platform-agnostic way to upload information to an Excel workbook.</span></span> <span data-ttu-id="a2a7f-103">In diesem Thema wird gezeigt, wie Sie in drei Webentwicklungsframeworks einfache Datensätze in eine Excel-Arbeitsmappe schreiben: ASP.NET, Angular und React.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-103">This topic shows you how to write simple data sets to an Excel workbook on three web development frameworks: ASP.NET, Angular, and React.</span></span> <span data-ttu-id="a2a7f-104">Sie können sich die in diesem Thema enthaltenen Codebeispiele in den [Microsoft Graph Excel-Beispielen auf GitHub](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter) ansehen.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-104">You can look at the code samples featured in this topic by visiting the [Microsoft Graph Excel starter samples on GitHub](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter).</span></span>

> <span data-ttu-id="a2a7f-105">**Hinweis:** In allen drei Beispielen werden Daten in eine Excel-Arbeitsmappe mit dem Namen **demo.xlxs** geschrieben.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-105">**Note:** All three of the samples write data to an Excel workbook named **demo.xlxs**.</span></span> <span data-ttu-id="a2a7f-106">Diese Arbeitsmappe wird für Sie bereitgestellt, damit Sie sie in Ihr eigenes OneDrive hochladen, Sie können aber auch Microsoft Graph zum Hochladen von Dateien in OneDrive verwenden.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-106">They provide this workbook for you so that you can upload it to your own OneDrive, but you can also use Microsoft Graph to upload files to OneDrive.</span></span> <span data-ttu-id="a2a7f-107">Wenn Sie mehr über die REST-Aufrufe erfahren möchten, die Sie zum Hochladen einer Datei eines beliebigen Typs in Ihren OneDrive-Stammordner benötigen, sehen Sie sich [Microsoft Graph – Excel REST-API – ASP.NET – Beispiel Aufgabenliste](https://github.com/microsoftgraph/aspnet-todo-rest-sample) an.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-107">If you're interested in learning the REST calls you need to upload a file of any type to your root OneDrive folder, see the [Microsoft Graph Excel REST API ASP.NET to-do list sample](https://github.com/microsoftgraph/aspnet-todo-rest-sample).</span></span>

<span data-ttu-id="a2a7f-108">In allen drei Excel-Einstiegsbeispielen werden dieselben Schritte ausgeführt: Abrufen des Namens und der Adresse des angemeldeten Benutzers und Hinzufügen dieser zwei Informationsstücke zu einer neuen Zeile in der Arbeitsmappe **demo.xlsx**.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-108">All three of the Excel starter samples do the same thing: retrieve the name and address of the signed-in user and add those two pieces of information to a new row in the **demo.xlsx** workbook.</span></span> <span data-ttu-id="a2a7f-109">Sie können die Beispiele so ändern, dass zusätzliche Zeilen hinzugefügt werden, indem Sie einfach Informationen zu dem zweidimensionalen Array hinzufügen, das die Zeile bzw. die Zeilen darstellt, die Sie hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-109">You can modify the samples to add additional rows simply by adding information to the two-dimensional array that represents the row or rows that you want to add.</span></span>

## <a name="add-a-row-or-rows-to-an-excel-workbook-with-a-single-rest-request"></a><span data-ttu-id="a2a7f-110">Hinzufügen von Zeilen zu einer Excel-Arbeitsmappe mit einer einzigen REST-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a2a7f-110">Add a row or rows to an Excel workbook with a single REST request</span></span>

<span data-ttu-id="a2a7f-111">Die Excel-REST-API erfordert, dass Sie eine einfachen Anforderungstext für den REST-Endpunkt bereitstellen, der die Zeilenauflistung einer Excel-Arbeitsmappe darstellt.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-111">The Excel REST API requires you to POST a simple request body to the REST endpoint that represents the row collection of an Excel workbook.</span></span> <span data-ttu-id="a2a7f-112">Wenn Sie mit einem Notizbuch im Stammordner des OneDrive-Konto des angemeldeten Benutzers arbeiten, sieht der REST-Endpunkt wie folgt aus:</span><span class="sxs-lookup"><span data-stu-id="a2a7f-112">If you're working with a notebook in the root folder of the signed-in user's OneDrive account, the REST endpoint will look like this:</span></span>

`https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add`

<span data-ttu-id="a2a7f-113">Weitere Informationen dazu, wie Sie Dateien in OneDrive-Ordnern erreichen, finden Sie unter [DriveItem-Ressourcentyp](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/driveitem) in unserer Referenzdokumentation.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-113">For more information about how to reach files in OneDrive folders, see the [DriveItem resource type](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/driveitem) in our reference documentation.</span></span>

> <span data-ttu-id="a2a7f-114">**Hinweis:** Sie können sich die vorhandene Zeilenauflistung der Arbeitsmappe ansehen, indem Sie eine GET-Anforderung für den Teil des Pfads ausführen, der bei `/rows` endet.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-114">**Note:** You can look at the existing row collection of the workbook by making a GET request to the part of the path that ends at `/rows`.</span></span>

<span data-ttu-id="a2a7f-115">Der POST-Text sieht wie folgt aus:</span><span class="sxs-lookup"><span data-stu-id="a2a7f-115">The POST body looks like this:</span></span>

`{
  "index": null,
  "values": [
    ['alex darrow', 'adarrow@tenant.onmicrosoft.com']
  ]
}`

<span data-ttu-id="a2a7f-116">Der Wert des ersten `index`-Parameters gibt die relative Position der Zeile an, die Sie zu dem nullindizierten Array von Zeilen hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-116">The value of the first `index` parameter specifies the relative position of the row that you're adding to the zero-indexed array of rows.</span></span> <span data-ttu-id="a2a7f-117">Zeilen unterhalb der eingefügten Zeile werden nach unten verschoben.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-117">Rows below the inserted row will be shifted downwards.</span></span> <span data-ttu-id="a2a7f-118">Der `null`-Parameter gibt an, dass die neue Zeile am Ende hinzugefügt wird.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-118">The `null` parameter indicates that the new row will be added to the end.</span></span>

<span data-ttu-id="a2a7f-119">Der Wert des zweiten `values`-Parameters ist ein zweidimensionales Zeichenfolgenarray, das die unformatierten Werte jeder Zeile enthält, die Sie hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-119">The value of the second `values` parameter is a two-dimensional string array that contains the unformatted values of each row that you want to add.</span></span> <span data-ttu-id="a2a7f-120">Das Array im Beispiel enthält nur eine Zeile, aber Sie können weitere Zeilen hinzufügen, indem Sie weitere Zeichenfolgenarrays hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-120">The array in the sample contains only one row, but you can add more rows by adding more string arrays.</span></span>

<span data-ttu-id="a2a7f-121">Sie können diese Abfrage mit Ihrem eigenen OneDrive-Konto testen, indem Sie die Datei „demo.xlsx“ in Ihren OneDrive-Stammordner hochladen und diese Abfrage im [Microsoft Graph Explorer](https://developer.microsoft.com/de-DE/graph/graph-explorer) ausführen.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-121">You can test this query with your own OneDrive account by uploading the demo.xlsx file to your OneDrive root folder and executing this query on the [Microsoft Graph Explorer](https://developer.microsoft.com/de-DE/graph/graph-explorer).</span></span>

<span data-ttu-id="a2a7f-122">Das ist alles, was Sie wissen müssen, um Daten in eine Excel-Arbeitsmappe zu schreiben.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-122">That is all you need to know in order to write data to an Excel workbook.</span></span> <span data-ttu-id="a2a7f-123">Sie müssen wissen, wie die Anforderung in Ihrem eigenen Framework erstellt und ausgeführt wird. In den Excel-Einstiegsbeispielen werden drei verschiedene Möglichkeiten hierfür dargestellt.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-123">You do need to know how to construct and make the request in your own framework, and the Excel starter samples demonstrate three separate ways of doing this.</span></span>

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-aspnet"></a><span data-ttu-id="a2a7f-124">Hinzufügen von Zeilen zu einer Excel-Arbeitsmappe in ASP.NET</span><span class="sxs-lookup"><span data-stu-id="a2a7f-124">Add a row or rows to an Excel workbook in ASP.NET</span></span>

<span data-ttu-id="a2a7f-125">Den ASP.NET-Code, der die Anforderung sendet, finden Sie in den Dateien [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) und [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) des [Microsoft Graph Excel-Einstiegsbeispiels für ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-excelstarter-sample).</span><span class="sxs-lookup"><span data-stu-id="a2a7f-125">You'll find the ASP.NET code that constructs and sends the request in the [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) and [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) files of the [Microsoft Graph Excel Starter Sample for ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-excelstarter-sample).</span></span>

<span data-ttu-id="a2a7f-126">Die Datei `GraphResources.cs` enthält eine Hilfsklasse zum Schachteln der Benutzerdaten, die Sie von Microsoft Graph abrufen, und des Anforderungstexts, den Sie beim Schreiben in Ihre Arbeitsmappe verwenden.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-126">The `GraphResources.cs` file provides a helper class for encapsulating both the user data you're retrieving from Microsoft Graph and the request body that you'll use when you write to your workbook.</span></span>

    public class UserInfo
    {
        public string Name { get; set; }
        public string Address { get; set; }

    }

    public class UserInfoRequest
    {
        public string index { get; set; }
        public string[][] values { get; set; }
    }

<span data-ttu-id="a2a7f-127">Die `GraphService.cs`-Klasse enthält eine `AddInfoToExcel`-Methode, die diese Klassen auffüllt, die Anforderungsinformationen in ein JSON-Objekt serialisiert und dieses Objekt dann als den POST-Anforderungstext übergibt.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-127">The `GraphService.cs` class contains an `AddInfoToExcel` method that populates these classes, serializes the request information into a JSON object, and then passes that object as the POST request body.</span></span>

        public async Task<string> AddInfoToExcel(string accessToken, string name, string address)
        {
            string endpoint = "https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add";
            using (var client = new HttpClient())
            {
                using (var request = new HttpRequestMessage(HttpMethod.Post, endpoint))
                {
                    // Populate UserInfoRequest object
                    string[] userInfo = { name, address  };
                    string[][] userInfoArray = { userInfo };
                    UserInfoRequest userInfoRequest = new UserInfoRequest();
                    userInfoRequest.index = null;
                    userInfoRequest.values = userInfoArray;

                    // Serialize the information in the UserInfoRequest object
                    string jsonBody = JsonConvert.SerializeObject(userInfoRequest);
                    request.Headers.Accept.Add(new MediaTypeWithQualityHeaderValue("application/json"));
                    request.Headers.Authorization = new AuthenticationHeaderValue("Bearer", accessToken);
                    request.Content = new StringContent(jsonBody, Encoding.UTF8, "application/json");

                    using (var response = await client.SendAsync(request))
                    {
                        if (response.IsSuccessStatusCode)
                        {
                            return Resource.Graph_UploadToExcel_Success_Result;
                        }
                        return response.ReasonPhrase;
                    }
                }
            }
        }

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-angular"></a><span data-ttu-id="a2a7f-128">Hinzufügen von Zeilen zu einer Excel-Arbeitsmappe in Angular</span><span class="sxs-lookup"><span data-stu-id="a2a7f-128">Add a row or rows to an Excel workbook in Angular</span></span>

<span data-ttu-id="a2a7f-129">Den Angular-Code, der die Anforderung sendet, finden Sie in der Datei [home.service.ts file](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts) des [Microsoft Graph Excel-Einstiegsbeispiels für Angular](https://github.com/microsoftgraph/angular-excelstarter-sample).</span><span class="sxs-lookup"><span data-stu-id="a2a7f-129">You'll find the Angular code that constructs and sends the request in the [home.service.ts file](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts) of the [Microsoft Graph Excel Starter Sample for Angular](https://github.com/microsoftgraph/angular-excelstarter-sample).</span></span>

<span data-ttu-id="a2a7f-130">Da in diesem Beispiel TypeScript verwendet wird, werden die [Microsoft Graph JavaScript-Clientbibliothek](https://github.com/microsoftgraph/msgraph-sdk-javascript) und die [Microsoft Graph TypeScript-Typen](https://github.com/microsoftgraph/msgraph-typescript-typings) genutzt.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-130">Since this sample uses TypeScript, it takes advantage of the [Microsoft Graph JavaScript Client Library](https://github.com/microsoftgraph/msgraph-sdk-javascript) and the [ Microsoft Graph TypeScript Types](https://github.com/microsoftgraph/msgraph-typescript-typings).</span></span>

<span data-ttu-id="a2a7f-131">Die `addInfoToExcel`-Funktion der `home.service.ts`-Datei erstellt das zweidimensionalen Zeichenfolgenarray und den Anforderungstext, der das Array enthält.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-131">The `addInfoToExcel` function in the `home.service.ts` file constructs the two-dimensional string array and the request body that contains the array.</span></span> <span data-ttu-id="a2a7f-132">Anschließend wird die Microsoft Graph JavaScript-Clientbibliothek zum Erstellen und Senden der Anforderung verwendet.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-132">It then uses the Microsoft Graph JavaScript Client Library to construct and send the request.</span></span> <span data-ttu-id="a2a7f-133">Die Antwort wird in Form einer Zusage zurückgesendet.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-133">The response comes back in the form of a Promise.</span></span>

      addInfoToExcel(user: MicrosoftGraph.User) {
        const userInfo = [];
        const userEmail = user.mail || user.userPrincipalName;    
        userInfo.push([user.displayName, userEmail]);

        const userInfoRequestBody = {
          index: null,
          values: userInfo
        };   

        const body = JSON.stringify(userInfoRequestBody);

        var client = this.getClient();
        var url = `${this.url}/me/drive/root:/${this.file}:/workbook/tables/${this.table}/rows/add`
        return Observable.fromPromise(client
        .api(url)
        .post(body)
        );
      }

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-react"></a><span data-ttu-id="a2a7f-134">Hinzufügen von Zeilen zu einer Excel-Arbeitsmappe in React</span><span class="sxs-lookup"><span data-stu-id="a2a7f-134">Add a row or rows to an Excel workbook in React</span></span>

<span data-ttu-id="a2a7f-135">Den React-Code, der die Anforderung sendet, finden Sie in der Datei [home.js file](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js) des [Microsoft Graph Excel-Einstiegsbeispiels für React](https://github.com/microsoftgraph/react-excelstarter-sample).</span><span class="sxs-lookup"><span data-stu-id="a2a7f-135">You'll find the code that constructs and sends the request in the [home.js file](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js) of the [Microsoft Graph Excel Starter Sample for React](https://github.com/microsoftgraph/react-excelstarter-sample).</span></span>

<span data-ttu-id="a2a7f-136">Die `onWriteToExcel`-Funktion erstellt das zweidimensionalen Zeichenfolgenarray und übergibt es als den Anforderungstext.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-136">The `onWriteToExcel` function constructs the two-dimensional string array and passes it as the request body.</span></span> <span data-ttu-id="a2a7f-137">[Axios](https://www.npmjs.com/package/axios) wird für die HTTP-Anforderung verwendet.</span><span class="sxs-lookup"><span data-stu-id="a2a7f-137">It uses [axios](https://www.npmjs.com/package/axios) to make the HTTP request.</span></span>

      onWriteToExcel() {
        const { token, me } = this.state;

        const myEmailAddress = me.mail || me.userPrincipalName;
        const values = [];

        values.push([me.displayName, myEmailAddress]);

        axios
          .post('https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add',
            { index: null, values },
            { headers: { Authorization: `Bearer ${token}` }}
          )
          .then(res => {
                          console.log(res);
                          const successMessage = "Successfully wrote your data to demo.xlsx!";
                          this.setState ({ successMessage });
                         })
          .catch(err => console.error(err));
      }

##<a name="see-also"></a><span data-ttu-id="a2a7f-138">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="a2a7f-138">See also</span></span>

* [<span data-ttu-id="a2a7f-139">Verwalten von Sitzungen in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a2a7f-139">Manage sessions in Excel with Microsoft Graph</span></span>](excel-manage-sessions.md)
* [<span data-ttu-id="a2a7f-140">Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a2a7f-140">Use workbook functions in Excel with Microsoft Graph</span></span>](excel-use-functions.md)
* [<span data-ttu-id="a2a7f-141">Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a2a7f-141">Update a range’s format in Excel with Microsoft Graph</span></span>](excel-update-range-format.md)
* [<span data-ttu-id="a2a7f-142">Anzeigen eines Diagrammbilds in Excel mithilfe von Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a2a7f-142">Display a chart image in Excel with Microsoft Graph</span></span>](excel-display-chart-image.md)
* [<span data-ttu-id="a2a7f-143">Verwenden der Excel-REST-API</span><span class="sxs-lookup"><span data-stu-id="a2a7f-143">Use the Excel REST API</span></span>](../api-reference/v1.0/resources/excel.md)    
