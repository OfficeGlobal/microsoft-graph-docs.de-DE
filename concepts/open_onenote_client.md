# <a name="open-the-onenote-client"></a>Öffnen der OneNote-Clients

Sie können die **Links**-Eigenschaft einer Seite oder eines Notizbuchs verwenden, um eine OneNote-Anwendung für eine bestimmte Seite oder ein Notizbuch zu öffnen. 

Die **Links**-Eigenschaft ist ein JSON-Objekt, das zwei URLs enthält. Die URLs öffnen die Seite oder das Notizbuch in der OneNote-Clientanwendung oder in OneNote Online.

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

- **oneNoteClientUrl** 

    - Öffnet den OneNote-Client, wenn dieser bereits auf dem Gerät installiert ist. Diese URL enthält das Präfix *onenote*.
    - Die sprachspezifische Version wird geöffnet, sofern diese auf dem Gerät installiert ist. Andernfalls wird die Spracheinstellung der Plattform verwendet.

- **oneNoteWebUrl** 

    - Öffnet OneNote Online, wenn der Standardbrowser auf dem Gerät OneNote Online unterstützt. 
    - Verwendet die Einstellung für die Browsersprache.


Die OneNote-API gibt die **links**-Eigenschaft in der HTTP-Antwort für die folgenden Vorgänge zurück:

- Erstellen Sie eine Seite durch Senden einer [`POST pages`](../api-reference/v1.0/api/section_post_pages.md)-Anforderung.

- Erstellen Sie ein Notizbuch durch Senden einer [`POST notebooks`](../api-reference/v1.0/api/onenote_post_notebooks.md)-Anforderung.

- Rufen Sie Seitenmetadaten durch Senden einer [`GET pages`](../api-reference/v1.0/api/page_get.md)- oder [`GET pages/{id}`](../api-reference/v1.0/api/page_get.md)-Anforderung ab.

- Rufen Sie Notizbuchmetadaten durch Senden einer [`GET notebooks`](../api-reference/v1.0/api/notebook_get.md)- oder [`GET notebooks/{id}`](../api-reference/v1.0/api/notebook_get.md)-Anforderung ab.

In den folgenden Beispielen wird gezeigt, wie der Statuscode der Antwort überprüft, die JSON an die richtigen URLs übersandt und der OneNote-Client geöffnet wird.

## <a name="ios-example"></a>iOS-Beispiel

Im folgenden Beispiel werden die OneNote-Client-URLs aus der JSON-Antwort abgerufen. Die AFNetworking-Bibliothek (http://afnetworking.com/) wird verwendet, um die beiden URLs zu extrahieren. Im Beispiel ist `created` der Zeiger für das **ONSCPSStandardResponse**-Objekt, in dem die Antwortwerte gespeichert wurden, und `responseObject` enthält die analysierte JSON.

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

Nachdem Sie die URLs der Antwort analysiert haben, können Sie OneNote mit dem folgenden Code öffnen. Verwenden Sie `oneNoteClientUrl`, um den installierten OneNote-Client zu öffnen, oder `oneNoteWebURL`, um OneNote Online zu öffnen.

```objc
NSURL *url = [NSURL URLWithString:standardResponse.oneNoteWebUrl];
[[UIApplication sharedApplication] openURL:url];
```

## <a name="android-example"></a>Android-Beispiel

Suchen Sie zunächst nach dem Erfolg-Statuscode, und analysieren Sie dann die JSON. Das Beispiel setzt voraus, dass eine POST-Anforderung gesendet wurde, und sucht daher nach einem `201 Created`-Statuscode. Wenn Sie eine `GET`-Anforderung durchgeführt haben, suchen Sie stattdessen nach einem `200` Statuscode.

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

Mit den Antworteigenschaften kann Ihre App OneNote Online öffnen (siehe folgendes Beispiel).

```java 
if (response.getResponseCode() == 201) {
    Uri uriUrl = Uri.parse(response.getOneNoteWebUrl);  
    Intent launchBrowser = new Intent(Intent.ACTION_VIEW, uriUrl); 
    startActivity(launchBrowser);
}
```

<br/>

Oder Ihre App kann den OneNote-Client auf einem Android-Gerät öffnen. Bei Verwendung der `oneNoteClientUrl`-Eigenschaft, müssen Sie die GUID-Zeichenfolgen in geschweifte Klammern `{ }` einfassen, bevor Sie das Internet starten. Im folgenden Beispiel wird dieser Vorgang erklärt.

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

## <a name="see-also"></a>Siehe auch

- [Abrufen von OneNote-Inhalt und -Struktur](onenote-get-content.md)
- [Erstellen von OneNote-Seiten](onenote-create-page.md)