# <a name="open-the-onenote-client"></a><span data-ttu-id="fdfc9-101">Öffnen der OneNote-Clients</span><span class="sxs-lookup"><span data-stu-id="fdfc9-101">Open the Postman client.</span></span>

<span data-ttu-id="fdfc9-102">Sie können die **Links**-Eigenschaft einer Seite oder eines Notizbuchs verwenden, um eine OneNote-Anwendung für eine bestimmte Seite oder ein Notizbuch zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-102">You can use the **links** property of a page or notebook to open a OneNote application to a particular page or notebook.</span></span> 

<span data-ttu-id="fdfc9-103">Die **Links**-Eigenschaft ist ein JSON-Objekt, das zwei URLs enthält.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-103">The **links** property is a JSON object that contains two URLs.</span></span> <span data-ttu-id="fdfc9-104">Die URLs öffnen die Seite oder das Notizbuch in der OneNote-Clientanwendung oder in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-104">The URLs will open the page or notebook in the OneNote client application or in OneNote Online.</span></span>

```json
{ 
    "links": {
        "oneNoteClientUrl": {
            "href": "onenote:https://..."
        },
        "oneNoteWebUrl": {
            "href": "https://..."
        }
    }
}
```

- <span data-ttu-id="fdfc9-105">Die **OneNoteClientUrl** öffnet den OneNote-Client, wenn dieser bereits auf dem Gerät installiert ist.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-105">**oneNoteClientUrl** - Opens the OneNote client if it is already installed on the device.</span></span> <span data-ttu-id="fdfc9-106">Diese URL enthält das Präfix *onenote*.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-106">This URL includes the *onenote* prefix.</span></span>
<span data-ttu-id="fdfc9-107">Die sprachspezifische Version wird geöffnet, sofern diese auf dem Gerät installiert ist.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-107">Opens the language-specific version if one is installed on the device.</span></span> <span data-ttu-id="fdfc9-108">Andernfalls wird die Spracheinstellung der Plattform verwendet.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-108">Otherwise, uses the platform language setting.</span></span>
- <span data-ttu-id="fdfc9-109">**OneNoteWebUrl** öffnet OneNote Online, wenn der Standardbrowser auf dem Gerät OneNote Online unterstützt.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-109">**oneNoteWebUrl** - Opens OneNote Online if the default browser on the device supports it.</span></span> <span data-ttu-id="fdfc9-110">Verwendet die Einstellung für die Browsersprache.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-110">Uses the browser language setting.</span></span>


<span data-ttu-id="fdfc9-111">Die OneNote-API gibt die **links**-Eigenschaft in der HTTP-Antwort für die folgenden Vorgänge zurück:</span><span class="sxs-lookup"><span data-stu-id="fdfc9-111">The OneNote API returns the **links** property in the HTTP response for the following operations:</span></span>

- <span data-ttu-id="fdfc9-112">Erstellen einer Seite durch Senden einer [ `POST pages` ](../api-reference/v1.0/api/section_post_pages.md)-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fdfc9-112">Create a page by sending a [`POST pages`](../api-reference/v1.0/api/section_post_pages.md) request</span></span>
- <span data-ttu-id="fdfc9-113">Erstellen eines Notizbuchs durch Senden einer [ `POST notebooks` ](../api-reference/v1.0/api/onenote_post_notebooks.md)-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fdfc9-113">Create a notebook by sending a [`POST notebooks`](../api-reference/v1.0/api/onenote_post_notebooks.md) request</span></span>
- <span data-ttu-id="fdfc9-114">Abrufen von Seitenmetadaten durch Senden einer [ `GET pages` ](../api-reference/v1.0/api/page_get.md)- oder [ `GET pages/{id}` ](../api-reference/v1.0/api/page_get.md)-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fdfc9-114">Get page metadata by sending a [`GET pages`](../api-reference/v1.0/api/page_get.md) or [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md) request</span></span>
- <span data-ttu-id="fdfc9-115">Abrufen von Seitenmetadaten durch Senden einer [ `GET notebooks` ](../api-reference/v1.0/api/notebook_get.md)- oder [ `GET notebooks/{id}` ](../api-reference/v1.0/api/notebook_get.md)-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fdfc9-115">Get notebook metadata by sending a [`GET notebooks`](../api-reference/v1.0/api/notebook_get.md) or [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md) request</span></span>

<span data-ttu-id="fdfc9-116">In den folgenden Beispielen wird gezeigt, wie der Statuscode der Antwort überprüft, die JSON an die richtigen URLs übersandt und der OneNote-Client geöffnet wird.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-116">The following examples show how to check the status code of the response, parse the JSON to extract the URLs, and then open the OneNote client.</span></span>

## <a name="ios-example"></a><span data-ttu-id="fdfc9-117">iOS-Beispiel</span><span class="sxs-lookup"><span data-stu-id="fdfc9-117">iOS example</span></span>

<span data-ttu-id="fdfc9-118">Im folgenden Beispiel werden die OneNote-Client-URLs aus der JSON-Antwort abgerufen.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-118">The following example gets the OneNote client URLs from the JSON response.</span></span> <span data-ttu-id="fdfc9-119">Die AFNetworking-Bibliothek (http://afnetworking.com/) wird verwendet, um die beiden URLs zu extrahieren.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-119">It uses the AFNetworking library (http://afnetworking.com/) to extract the two URLs.</span></span> <span data-ttu-id="fdfc9-120">Im Beispiel ist `created` der Zeiger für das ONSCPSStandardResponse-Objekt, in dem die Antwortwerte gespeichert wurden, und `responseObject` enthält die analysierte JSON.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-120">The following example gets the oncshort client URLs from the JSON response. It uses the AFNetworking library (http://afnetworking.com/http://afnetworking.com/) to extract the two URLs. In the example, created`created` is a pointer to the ONSCPSStandardResponse`responseObject` object used to store the response values, and responseObject holds the parsed JSON.</span></span>

```objectivec
    /* Import the JSON library */
    #import "AFURLRequestSerialization.h"

    - (void)connectionDidFinishLoading:(NSURLConnection *)connection {
            if(delegate) {
                  int status = [returnResponse statusCode];
                  ONSCPSStandardResponse *standardResponse = nil;
                  if (status == 201) {
                        ONSCPSCreateSuccessResponse *created = 
                              [[ONSCPSCreateSuccessResponse alloc] init];
                        created.httpStatusCode = status;
                        NSError *jsonError;
                        NSDictionary *responseObject = 
                              [NSJSONSerialization JSONObjectWithData:returnData options:0 error:&jsonError];
                        if(responseObject && !jsonError) {
                              created.oneNoteClientUrl = ((NSDictionary *)
                                    ((NSDictionary *)responseObject[@"links"])[@"oneNoteClientUrl"])[@"href"];
                              created.oneNoteWebUrl = ((NSDictionary *)
                                    ((NSDictionary *)responseObject[@"links"])[@"oneNoteWebUrl"])[@"href"];
                        }
                  standardResponse = created;
                  }
                  else {
                        ONSCPSStandardErrorResponse *error = [[ONSCPSStandardErrorResponse alloc] init];
                        error.httpStatusCode = status;
                        error.message = [[NSString alloc] initWithData:returnData 
                              encoding:NSUTF8StringEncoding];
                        standardResponse = error;
                  }
                  // Send the response back to the client.
                  if (standardResponse) {
                        [delegate exampleServiceActionDidCompleteWithResponse: standardResponse];
                  }
            }
      }
``` 

<span data-ttu-id="fdfc9-121">Nachdem Sie die URLs der Antwort analysiert haben, können Sie OneNote mit dem folgenden Code öffnen.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-121">After you parse the URLs from the response, you can open OneNote by using the following code.</span></span> <span data-ttu-id="fdfc9-122">Verwenden Sie `oneNoteClientUrl`, um den installierten OneNote-Client zu öffnen, oder `oneNoteWebURL`, um OneNote Online zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-122">Use `oneNoteClientUrl` to open the installed OneNote client or `oneNoteWebURL` to open OneNote Online.</span></span>

```objectivec
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a><span data-ttu-id="fdfc9-123">Android-Beispiel</span><span class="sxs-lookup"><span data-stu-id="fdfc9-123">Android example</span></span>

<span data-ttu-id="fdfc9-124">Suchen Sie zunächst nach dem für den Erfolg-Statuscode und analysieren Sie dann die JSON.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-124">First, check for the success status code and then parse the JSON.</span></span> <span data-ttu-id="fdfc9-125">Das Beispiel setzt voraus, dass eine POST-Anforderung gesendet wurde, und sucht daher nach einem `201 Created`-Statuscode.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-125">The example assumes a POST request was sent, so it checks for a `201 Created` status code.</span></span> <span data-ttu-id="fdfc9-126">Wenn Sie eine `GET`-Anforderung durchgeführt haben, suchen Sie stattdessen nach einem `200` Statuscode.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-126">If you made a `GET` request, check for a `200` status code instead.</span></span>

```java
public ApiResponse getResponse() throws Exception {
    /* Get the HTTP response code and message from the connection object */
    int responseCode = mUrlConnection.getResponseCode();
    String responseMessage = mUrlConnection.getResponseMessage();
    String responseBody = null;

    /* Get the response if the new page was created successfully. */
    if ( responseCode == 201) {
        InputStream is = mUrlConnection.getInputStream();

        /* Verify that this byte array is big enough. */
        byte[] b1 = new byte[1024];
        StringBuffer buffer = new StringBuffer();

        /* Copy the body of the response into the new string. */
        /* Make sure the buffer is big enough. */
        while ( is.read(b1) != -1)
            buffer.append(new String(b1));

      /* When the returned data is complete, close the connection 
         and convert the byte array into a string. */
        mUrlConnection.disconnect();
        responseBody =  buffer.toString();
    }

    /* Create a new JSON object, and an object to hold the response URLs. */
    JSONObject responseObject = null;
    ApiResponse response = new ApiResponse();
    try {

        /* Store and verify the HTTP response code. */
        response.setResponseCode(responseCode);
        response.setResponseMessage(responseMessage);
        if ( responseCode == 201) {

            /* Retrieve the two URLs from the links property. */
            responseObject = new JSONObject(responseBody);
            String clientUrl = responseObject.getJSONObject(
                "links").getJSONObject("oneNoteClientUrl").getString("href");
            String webUrl = responseObject.getJSONObject(
                "links").getJSONObject("oneNoteWebUrl").getString("href");
            response.setOneNoteClientUrl(clientUrl);
            response.setOneNoteWebUrl(webUrl);
        }
    } catch (JSONException ex) {

        /* If the JSON was malformed or incomplete... */
        String msg = ex.getMessage();
        msg = msg;
    }
    return response;
}
```

<span data-ttu-id="fdfc9-127">Mit den Antworteigenschaften kann Ihre App OneNote Online öffnen (siehe folgendes Beispiel).</span><span class="sxs-lookup"><span data-stu-id="fdfc9-127">Using the response properties, your app can open OneNote Online, as shown in the following example.</span></span>

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```
 
<span data-ttu-id="fdfc9-128">Oder Ihre App kann den OneNote-Client auf einem Android-Gerät öffnen.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-128">Or your app can open the OneNote client on an Android device.</span></span> <span data-ttu-id="fdfc9-129">Bei Verwendung der `oneNoteClientUrl`-Eigenschaft, müssen Sie die GUID-Zeichenfolgen in geschweifte Klammern `{ }` einfassen, bevor Sie das Internet starten.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-129">When using the `oneNoteClientUrl` property, you must surround the GUID strings with braces `{ }` before starting the Intent.</span></span> <span data-ttu-id="fdfc9-130">Im folgenden Beispiel wird dieser Vorgang erklärt.</span><span class="sxs-lookup"><span data-stu-id="fdfc9-130">The following example shows how to:</span></span>

```java 
if (response.getResponseCode() == 201) {

    // Get the URL from the OneNote API JSON response.
    String onenoteClientUrl = obtainClientLinkFromJSONResponse();
    String androidClientUrl = 
        onenoteClientUrl.replaceAll(
            "=([0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12})&",
            "={$1}&");

    // Open the URL: Open the newly created OneNote page.
    Uri uriUrl = Uri.parse(androidClientUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

## <a name="see-also"></a><span data-ttu-id="fdfc9-131">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="fdfc9-131">See also</span></span>

- [<span data-ttu-id="fdfc9-132">Abrufen von OneNote-Inhalt und -Struktur</span><span class="sxs-lookup"><span data-stu-id="fdfc9-132">Get OneNote content and structure</span></span>](https://msdn.microsoft.com/en-us/office/office365/howto/onenote-get-content)
- [<span data-ttu-id="fdfc9-133">Erstellen von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="fdfc9-133">Create OneNote pages</span></span>](../api-reference/v1.0/api/section_post_pages.md)