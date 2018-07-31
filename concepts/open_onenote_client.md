# <a name="open-the-onenote-client"></a><span data-ttu-id="7efad-101">Öffnen der OneNote-Clients</span><span class="sxs-lookup"><span data-stu-id="7efad-101">Open the OneNote client</span></span>

<span data-ttu-id="7efad-102">Sie können die **Links**-Eigenschaft einer Seite oder eines Notizbuchs verwenden, um eine OneNote-Anwendung für eine bestimmte Seite oder ein Notizbuch zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="7efad-102">You can use the **links** property of a page or notebook to open a OneNote application to a particular page or notebook.</span></span> 

<span data-ttu-id="7efad-103">Die **Links**-Eigenschaft ist ein JSON-Objekt, das zwei URLs enthält.</span><span class="sxs-lookup"><span data-stu-id="7efad-103">The **links** property is a JSON object that contains two URLs.</span></span> <span data-ttu-id="7efad-104">Die URLs öffnen die Seite oder das Notizbuch in der OneNote-Clientanwendung oder in OneNote Online.</span><span class="sxs-lookup"><span data-stu-id="7efad-104">The URLs will open the page or notebook in the OneNote client application or in OneNote Online.</span></span>

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

- <span data-ttu-id="7efad-105">**oneNoteClientUrl**</span><span class="sxs-lookup"><span data-stu-id="7efad-105">**oneNoteClientUrl**</span></span> 

    - <span data-ttu-id="7efad-106">Öffnet den OneNote-Client, wenn dieser bereits auf dem Gerät installiert ist.</span><span class="sxs-lookup"><span data-stu-id="7efad-106">oneNoteClientUrl - Opens the OneNote client if it is already installed on the device.</span></span> <span data-ttu-id="7efad-107">Diese URL enthält das Präfix *onenote*.</span><span class="sxs-lookup"><span data-stu-id="7efad-107">This URL includes the *onenote* prefix.</span></span>
    - <span data-ttu-id="7efad-108">Die sprachspezifische Version wird geöffnet, sofern diese auf dem Gerät installiert ist.</span><span class="sxs-lookup"><span data-stu-id="7efad-108">Opens the language-specific version if one is installed on the device.</span></span> <span data-ttu-id="7efad-109">Andernfalls wird die Spracheinstellung der Plattform verwendet.</span><span class="sxs-lookup"><span data-stu-id="7efad-109">Otherwise, uses the platform language setting.</span></span>

- <span data-ttu-id="7efad-110">**oneNoteWebUrl**</span><span class="sxs-lookup"><span data-stu-id="7efad-110">**oneNoteWebUrl**</span></span> 

    - <span data-ttu-id="7efad-111">Öffnet OneNote Online, wenn der Standardbrowser auf dem Gerät OneNote Online unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7efad-111">oneNoteWebUrl - Opens OneNote Online if the default browser on the device supports it.</span></span> 
    - <span data-ttu-id="7efad-112">Verwendet die Einstellung für die Browsersprache.</span><span class="sxs-lookup"><span data-stu-id="7efad-112">Uses the browser language setting.</span></span>


<span data-ttu-id="7efad-113">Die OneNote-API gibt die **links**-Eigenschaft in der HTTP-Antwort für die folgenden Vorgänge zurück:</span><span class="sxs-lookup"><span data-stu-id="7efad-113">The OneNote API returns the **links** property in the HTTP response for the following operations:</span></span>

- <span data-ttu-id="7efad-114">Erstellen Sie eine Seite durch Senden einer [`POST pages`](../api-reference/v1.0/api/section_post_pages.md)-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7efad-114">Create a page by sending a [`POST pages`](../api-reference/v1.0/api/section_post_pages.md) request</span></span>

- <span data-ttu-id="7efad-115">Erstellen Sie ein Notizbuch durch Senden einer [`POST notebooks`](../api-reference/v1.0/api/onenote_post_notebooks.md)-Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7efad-115">Create a notebook by sending a [`POST notebooks`](../api-reference/v1.0/api/onenote_post_notebooks.md) request</span></span>

- <span data-ttu-id="7efad-116">Rufen Sie Seitenmetadaten durch Senden einer [`GET pages`](../api-reference/v1.0/api/page_get.md)- oder [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md)-Anforderung ab.</span><span class="sxs-lookup"><span data-stu-id="7efad-116">Get page metadata by sending a [`GET pages`](../api-reference/v1.0/api/page_get.md) or [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md) request</span></span>

- <span data-ttu-id="7efad-117">Rufen Sie Notizbuchmetadaten durch Senden einer [`GET notebooks`](../api-reference/v1.0/api/notebook_get.md)- oder [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md)-Anforderung ab.</span><span class="sxs-lookup"><span data-stu-id="7efad-117">Get notebook metadata by sending a [`GET notebooks`](../api-reference/v1.0/api/notebook_get.md) or [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md) request</span></span>

<span data-ttu-id="7efad-118">In den folgenden Beispielen wird gezeigt, wie der Statuscode der Antwort überprüft, die JSON an die richtigen URLs übersandt und der OneNote-Client geöffnet wird.</span><span class="sxs-lookup"><span data-stu-id="7efad-118">The following examples show how to check the status code of the response, parse the JSON to extract the URLs, and then open the OneNote client.</span></span>

## <a name="ios-example"></a><span data-ttu-id="7efad-119">iOS-Beispiel</span><span class="sxs-lookup"><span data-stu-id="7efad-119">iOS example</span></span>

<span data-ttu-id="7efad-120">Im folgenden Beispiel werden die OneNote-Client-URLs aus der JSON-Antwort abgerufen.</span><span class="sxs-lookup"><span data-stu-id="7efad-120">The following example gets the OneNote client URLs from the JSON response.</span></span> <span data-ttu-id="7efad-121">Die AFNetworking-Bibliothek (http://afnetworking.com/) wird verwendet, um die beiden URLs zu extrahieren.</span><span class="sxs-lookup"><span data-stu-id="7efad-121">It uses the AFNetworking library (http://afnetworking.com/) to extract the two URLs.</span></span> <span data-ttu-id="7efad-122">Im Beispiel ist `created` der Zeiger für das **ONSCPSStandardResponse**-Objekt, in dem die Antwortwerte gespeichert wurden, und `responseObject` enthält die analysierte JSON.</span><span class="sxs-lookup"><span data-stu-id="7efad-122">In the example, `created` is a pointer to the ONSCPSStandardResponse object used to store the response values, and `responseObject` holds the parsed JSON.</span></span>

```objc
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

<br/>

<span data-ttu-id="7efad-123">Nachdem Sie die URLs der Antwort analysiert haben, können Sie OneNote mit dem folgenden Code öffnen.</span><span class="sxs-lookup"><span data-stu-id="7efad-123">After you parse the URLs from the response, you can open OneNote by using the following code.</span></span> <span data-ttu-id="7efad-124">Verwenden Sie `oneNoteClientUrl`, um den installierten OneNote-Client zu öffnen, oder `oneNoteWebURL`, um OneNote Online zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="7efad-124">Use `oneNoteClientUrl` to open the installed OneNote client or `oneNoteWebURL` to open OneNote Online.</span></span>

```objc
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a><span data-ttu-id="7efad-125">Android-Beispiel</span><span class="sxs-lookup"><span data-stu-id="7efad-125">Android example</span></span>

<span data-ttu-id="7efad-126">Suchen Sie zunächst nach dem Erfolg-Statuscode, und analysieren Sie dann die JSON.</span><span class="sxs-lookup"><span data-stu-id="7efad-126">First, check for the success status code and then parse the JSON.</span></span> <span data-ttu-id="7efad-127">Das Beispiel setzt voraus, dass eine POST-Anforderung gesendet wurde, und sucht daher nach einem `201 Created`-Statuscode.</span><span class="sxs-lookup"><span data-stu-id="7efad-127">The example assumes a POST request was sent, so it checks for a `201 Created` status code.</span></span> <span data-ttu-id="7efad-128">Wenn Sie eine `GET`-Anforderung durchgeführt haben, suchen Sie stattdessen nach einem `200` Statuscode.</span><span class="sxs-lookup"><span data-stu-id="7efad-128">If you made a `GET` request, check for a `200` status code instead.</span></span>

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

<br/>

<span data-ttu-id="7efad-129">Mit den Antworteigenschaften kann Ihre App OneNote Online öffnen (siehe folgendes Beispiel).</span><span class="sxs-lookup"><span data-stu-id="7efad-129">Using the response properties, your app can open OneNote Online, as shown in the following example.</span></span>

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

<br/>

<span data-ttu-id="7efad-130">Oder Ihre App kann den OneNote-Client auf einem Android-Gerät öffnen.</span><span class="sxs-lookup"><span data-stu-id="7efad-130">Or your app can open the OneNote client on an Android device.</span></span> <span data-ttu-id="7efad-131">Bei Verwendung der `oneNoteClientUrl`-Eigenschaft, müssen Sie die GUID-Zeichenfolgen in geschweifte Klammern `{ }` einfassen, bevor Sie das Internet starten.</span><span class="sxs-lookup"><span data-stu-id="7efad-131">When using the `oneNoteClientUrl` property, you must surround the GUID strings with braces `{ }` before starting the Intent.</span></span> <span data-ttu-id="7efad-132">Im folgenden Beispiel wird dieser Vorgang erklärt.</span><span class="sxs-lookup"><span data-stu-id="7efad-132">The following example shows how to do that.</span></span>

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

## <a name="see-also"></a><span data-ttu-id="7efad-133">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="7efad-133">See also</span></span>

- [<span data-ttu-id="7efad-134">Abrufen von OneNote-Inhalt und -Struktur</span><span class="sxs-lookup"><span data-stu-id="7efad-134">Get OneNote content and structure</span></span>](onenote-get-content.md)
- [<span data-ttu-id="7efad-135">Erstellen von OneNote-Seiten</span><span class="sxs-lookup"><span data-stu-id="7efad-135">Create OneNote pages</span></span>](onenote-create-page.md)