# <a name="write-data-to-an-excel-workbook-with-microsoft-graph"></a>Schreiben von Daten in eine Excel-Arbeitsmappe mit Microsoft Graph

Die Excel REST-API bietet eine einfache und plattformunabhängige Methode zum Hochladen von Informationen in eine Excel-Arbeitsmappe. In diesem Thema wird gezeigt, wie Sie in drei Webentwicklungsframeworks einfache Datensätze in eine Excel-Arbeitsmappe schreiben: ASP.NET, Angular und React. Sie können sich die in diesem Thema enthaltenen Codebeispiele in den [Microsoft Graph Excel-Beispielen auf GitHub](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=excelstarter) ansehen.

> **Hinweis:** In allen drei Beispielen werden Daten in eine Excel-Arbeitsmappe mit dem Namen **demo.xlxs** geschrieben. Diese Arbeitsmappe wird für Sie bereitgestellt, damit Sie sie in Ihr eigenes OneDrive hochladen, Sie können aber auch Microsoft Graph zum Hochladen von Dateien in OneDrive verwenden. Wenn Sie mehr über die REST-Aufrufe erfahren möchten, die Sie zum Hochladen einer Datei eines beliebigen Typs in Ihren OneDrive-Stammordner benötigen, sehen Sie sich [Microsoft Graph – Excel REST-API – ASP.NET – Beispiel Aufgabenliste](https://github.com/microsoftgraph/aspnet-todo-rest-sample) an.

In allen drei Excel-Einstiegsbeispielen werden dieselben Schritte ausgeführt: Abrufen des Namens und der Adresse des angemeldeten Benutzers und Hinzufügen dieser zwei Informationsstücke zu einer neuen Zeile in der Arbeitsmappe **demo.xlsx**. Sie können die Beispiele so ändern, dass zusätzliche Zeilen hinzugefügt werden, indem Sie einfach Informationen zu dem zweidimensionalen Array hinzufügen, das die Zeile bzw. die Zeilen darstellt, die Sie hinzufügen möchten.

## <a name="add-a-row-or-rows-to-an-excel-workbook-with-a-single-rest-request"></a>Hinzufügen von Zeilen zu einer Excel-Arbeitsmappe mit einer einzigen REST-Anforderung

Die Excel-REST-API erfordert, dass Sie eine einfachen Anforderungstext für den REST-Endpunkt bereitstellen, der die Zeilenauflistung einer Excel-Arbeitsmappe darstellt. Wenn Sie mit einem Notizbuch im Stammordner des OneDrive-Konto des angemeldeten Benutzers arbeiten, sieht der REST-Endpunkt wie folgt aus:

`https://graph.microsoft.com/v1.0/me/drive/root:/demo.xlsx:/workbook/tables/Table1/rows/add`

Weitere Informationen dazu, wie Sie Dateien in OneDrive-Ordnern erreichen, finden Sie unter [DriveItem-Ressourcentyp](https://developer.microsoft.com/de-DE/graph/docs/api-reference/v1.0/resources/driveitem) in unserer Referenzdokumentation.

> **Hinweis:** Sie können sich die vorhandene Zeilenauflistung der Arbeitsmappe ansehen, indem Sie eine GET-Anforderung für den Teil des Pfads ausführen, der bei `/rows` endet.

Der POST-Text sieht wie folgt aus:

`{
  "index": null,
  "values": [
    ['alex darrow', 'adarrow@tenant.onmicrosoft.com']
  ]
}`

Der Wert des ersten `index`-Parameters gibt die relative Position der Zeile an, die Sie zu dem nullindizierten Array von Zeilen hinzufügen. Zeilen unterhalb der eingefügten Zeile werden nach unten verschoben. Der `null`-Parameter gibt an, dass die neue Zeile am Ende hinzugefügt wird.

Der Wert des zweiten `values`-Parameters ist ein zweidimensionales Zeichenfolgenarray, das die unformatierten Werte jeder Zeile enthält, die Sie hinzufügen möchten. Das Array im Beispiel enthält nur eine Zeile, aber Sie können weitere Zeilen hinzufügen, indem Sie weitere Zeichenfolgenarrays hinzufügen.

Sie können diese Abfrage mit Ihrem eigenen OneDrive-Konto testen, indem Sie die Datei „demo.xlsx“ in Ihren OneDrive-Stammordner hochladen und diese Abfrage im [Microsoft Graph Explorer](https://developer.microsoft.com/de-DE/graph/graph-explorer) ausführen.

Das ist alles, was Sie wissen müssen, um Daten in eine Excel-Arbeitsmappe zu schreiben. Sie müssen wissen, wie die Anforderung in Ihrem eigenen Framework erstellt und ausgeführt wird. In den Excel-Einstiegsbeispielen werden drei verschiedene Möglichkeiten hierfür dargestellt.

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-aspnet"></a>Hinzufügen von Zeilen zu einer Excel-Arbeitsmappe in ASP.NET

Den ASP.NET-Code, der die Anforderung sendet, finden Sie in den Dateien [GraphResources.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphResources.cs) und [GraphService.cs](https://github.com/microsoftgraph/aspnet-excelstarter-sample/blob/master/Microsoft%20Graph%20Excel%20REST%20ASPNET/Models/GraphService.cs) des [Microsoft Graph Excel-Einstiegsbeispiels für ASP.NET 4.6](https://github.com/microsoftgraph/aspnet-excelstarter-sample).

Die Datei `GraphResources.cs` enthält eine Hilfsklasse zum Schachteln der Benutzerdaten, die Sie von Microsoft Graph abrufen, und des Anforderungstexts, den Sie beim Schreiben in Ihre Arbeitsmappe verwenden.

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

Die `GraphService.cs`-Klasse enthält eine `AddInfoToExcel`-Methode, die diese Klassen auffüllt, die Anforderungsinformationen in ein JSON-Objekt serialisiert und dieses Objekt dann als den POST-Anforderungstext übergibt.

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

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-angular"></a>Hinzufügen von Zeilen zu einer Excel-Arbeitsmappe in Angular

Den Angular-Code, der die Anforderung sendet, finden Sie in der Datei [home.service.ts file](https://github.com/microsoftgraph/angular-excelstarter-sample/blob/master/src/app/home/home.service.ts) des [Microsoft Graph Excel-Einstiegsbeispiels für Angular](https://github.com/microsoftgraph/angular-excelstarter-sample).

Da in diesem Beispiel TypeScript verwendet wird, werden die [Microsoft Graph JavaScript-Clientbibliothek](https://github.com/microsoftgraph/msgraph-sdk-javascript) und die [Microsoft Graph TypeScript-Typen](https://github.com/microsoftgraph/msgraph-typescript-typings) genutzt.

Die `addInfoToExcel`-Funktion der `home.service.ts`-Datei erstellt das zweidimensionalen Zeichenfolgenarray und den Anforderungstext, der das Array enthält. Anschließend wird die Microsoft Graph JavaScript-Clientbibliothek zum Erstellen und Senden der Anforderung verwendet. Die Antwort wird in Form einer Zusage zurückgesendet.

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

## <a name="add-a-row-or-rows-to-an-excel-workbook-in-react"></a>Hinzufügen von Zeilen zu einer Excel-Arbeitsmappe in React

Den React-Code, der die Anforderung sendet, finden Sie in der Datei [home.js file](https://github.com/microsoftgraph/react-excelstarter-sample/blob/master/src/home/home.js) des [Microsoft Graph Excel-Einstiegsbeispiels für React](https://github.com/microsoftgraph/react-excelstarter-sample).

Die `onWriteToExcel`-Funktion erstellt das zweidimensionalen Zeichenfolgenarray und übergibt es als den Anforderungstext. [Axios](https://www.npmjs.com/package/axios) wird für die HTTP-Anforderung verwendet.

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

##<a name="see-also"></a>Siehe auch

* [Verwalten von Sitzungen in Excel mit Microsoft Graph](excel-manage-sessions.md)
* [Verwenden von Arbeitsmappenfunktionen in Excel mit Microsoft Graph](excel-use-functions.md)
* [Aktualisieren eines Bereichsformats in Excel mit Microsoft Graph](excel-update-range-format.md)
* [Anzeigen eines Diagrammbilds in Excel mithilfe von Microsoft Graph](excel-display-chart-image.md)
* [Verwenden der Excel-REST-API](../api-reference/v1.0/resources/excel.md)    
