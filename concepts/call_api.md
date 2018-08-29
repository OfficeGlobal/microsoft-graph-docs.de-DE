# <a name="calling-the-microsoft-graph-api"></a><span data-ttu-id="c0662-101">Aufrufen der Microsoft Graph-API</span><span class="sxs-lookup"><span data-stu-id="c0662-101">Calling the Microsoft Graph API</span></span>

<span data-ttu-id="c0662-102">Wenn Sie auf eine Microsoft Graph-Ressource zugreifen oder diese bearbeiten möchten, müssen Sie die Ressourcen-URLs aufrufen und festlegen, indem Sie einen der folgenden Vorgänge verwenden.</span><span class="sxs-lookup"><span data-stu-id="c0662-102">To access and manipulate a Microsoft Graph resource, you call and specify the resource URLs using one of the following operations:</span></span>   

- <span data-ttu-id="c0662-103">GET</span><span class="sxs-lookup"><span data-stu-id="c0662-103">GET</span></span>
- <span data-ttu-id="c0662-104">POST</span><span class="sxs-lookup"><span data-stu-id="c0662-104">POST</span></span>
- <span data-ttu-id="c0662-105">PATCH</span><span class="sxs-lookup"><span data-stu-id="c0662-105">PATCH</span></span>
- <span data-ttu-id="c0662-106">PUT</span><span class="sxs-lookup"><span data-stu-id="c0662-106">PUT</span></span>
- <span data-ttu-id="c0662-107">DELETE</span><span class="sxs-lookup"><span data-stu-id="c0662-107">DELETE</span></span> 

<span data-ttu-id="c0662-108">Alle Microsoft Graph-API-Anforderungen verwenden das folgende Basis-URL-Muster:</span><span class="sxs-lookup"><span data-stu-id="c0662-108">All Microsoft Graph API requests use the following basic URL pattern:</span></span>

```
    https://graph.microsoft.com/{version}/{resource}?[query_parameters]
```

<span data-ttu-id="c0662-109">Für diese URL:</span><span class="sxs-lookup"><span data-stu-id="c0662-109">For this URL:</span></span>

- <span data-ttu-id="c0662-110">`https://graph.microsoft.com` ist der Microsoft Graph-API-Endpunkt.</span><span class="sxs-lookup"><span data-stu-id="c0662-110">`https://graph.microsoft.com` is the Microsoft Graph API endpoint.</span></span>
- <span data-ttu-id="c0662-111">`{version}` ist die Zieldienstversion, z. B. `v1.0` oder `beta`.</span><span class="sxs-lookup"><span data-stu-id="c0662-111">`{version}` is the target service version, for example, `v1.0` or `beta`.</span></span>
- <span data-ttu-id="c0662-112">`{resource}` ist das Ressourcensegment oder der Pfad, z. B</span><span class="sxs-lookup"><span data-stu-id="c0662-112">`{resource}` is resource segment or path, such as:</span></span>
  - <span data-ttu-id="c0662-113">`users`, `groups`, `devices`, `organization`</span><span class="sxs-lookup"><span data-stu-id="c0662-113"></span></span>
  - <span data-ttu-id="c0662-114">Der Alias `me`, der den angemeldeten Benutzer auflöst.</span><span class="sxs-lookup"><span data-stu-id="c0662-114">The alias `me`, which resolves to the signed-in user</span></span>
   - <span data-ttu-id="c0662-115">Die mit einem Benutzer verknüpften Ressourcen, z. B. `me/events`, `me/drive` oder `me/messages`.</span><span class="sxs-lookup"><span data-stu-id="c0662-115">The resources belonging to a user, such as `me/events`, `me/drive` or `me/messages`</span></span>
  - <span data-ttu-id="c0662-116">Der Alias `myOrganization`, der den Mandanten des bei der Organisation angemeldet Benutzers auflöst.</span><span class="sxs-lookup"><span data-stu-id="c0662-116">The alias `myOrganization`, which resolves to the tenant of the organization signed-in user</span></span>
- <span data-ttu-id="c0662-117">`[query_parameters]` stellt zusätzliche Abfrageparameter dar, z. B. `$filter` und `$select`.</span><span class="sxs-lookup"><span data-stu-id="c0662-117">`[query_parameters]` represents additional query parameters such as `$filter` and `$select`.</span></span>

<span data-ttu-id="c0662-p101">Optional können Sie auch den Mandanten als Teil der Anforderung angeben. Geben Sie bei Verwendung von `me` nicht den Mandanten an. Eine Liste allgemeiner Anforderungen finden Sie unter [Übersicht über Microsoft Graph](overview.md).</span><span class="sxs-lookup"><span data-stu-id="c0662-p101">Optionally, you can also specify the tenant as part of your request. When using `me`, do not specify the tenant. For a list of common requests, see [Overview of Microsoft Graph](overview.md).</span></span>

## <a name="microsoft-graph-api-metadata"></a><span data-ttu-id="c0662-121">Microsoft Graph-API-Metadaten</span><span class="sxs-lookup"><span data-stu-id="c0662-121">Microsoft Graph API metadata</span></span>
<span data-ttu-id="c0662-p102">Das Metadatendokument ($metadata) wird im Dienststamm veröffentlicht. Über die folgenden URLs können Sie das Dienstdokument für v1.0 und die Betaversionen anzeigen.</span><span class="sxs-lookup"><span data-stu-id="c0662-p102">The metadata document ($metadata) is published at the service root. For example, you can view the service document for the v1.0 and beta versions via the following URLs.</span></span>

<span data-ttu-id="c0662-124">Metadaten für Microsoft Graph-API `v1.0`</span><span class="sxs-lookup"><span data-stu-id="c0662-124">Microsoft Graph API `v1.0` metadata.</span></span>
```
    https://graph.microsoft.com/v1.0/$metadata
```
<span data-ttu-id="c0662-125">Metadaten für Microsoft Graph-API `beta`</span><span class="sxs-lookup"><span data-stu-id="c0662-125">Microsoft Graph API `beta` metadata.</span></span>
```
    https://graph.microsoft.com/beta/$metadata
```

<span data-ttu-id="c0662-126">Mithilfe der Metadaten können Sie das Datenmodell von Microsoft Graph sehen und verstehen, einschließlich Entitätstypen und Entitätenmengen, komplexe Typen und Enumerationen, aus denen die Anforderungs- und Antwortpakete bestehen, die an und von Microsoft Graph gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="c0662-126">The metadata allows you to see and understand the data model of Microsoft Graph, including the entity types and sets, complex types, and enums that make up the request and response packets sent to and from Microsoft Graph.</span></span>
<span data-ttu-id="c0662-127">Die Metadaten können Sie verwenden, um die Beziehungen zwischen Entitäten in Microsoft Graph zu verstehen und URLs einzurichten, die zwischen Entitäten navigieren.</span><span class="sxs-lookup"><span data-stu-id="c0662-127">You can use the metadata to understand the realtionships between entities in Microsoft Graph and establish URLs that navigate between entities.</span></span>
<span data-ttu-id="c0662-128">Diese auf Navigation-basierende Vernetzung ist das charakteristische Merkmal von Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="c0662-128">This navigation-based interconnectedness gives Microsoft Graph its unique character.</span></span>

<span data-ttu-id="c0662-129">Bei den Pfad-URL-Ressourcennamen und Abfrageparametern sowie den Aktionsparametern und -werten wird nicht nach Groß-/Kleinschreibung unterschieden.</span><span class="sxs-lookup"><span data-stu-id="c0662-129">Path URL resource names, query parameters, and action parameters and values are case insensitive.</span></span> <span data-ttu-id="c0662-130">Bei zugewiesenen Werten, Entitäts-IDs und anderen base64-codierte Werten wird nach Groß-/Kleinschreibung unterschieden.</span><span class="sxs-lookup"><span data-stu-id="c0662-130">However, values you assign, entity IDs, and other base64-encoded values are case-sensitive.</span></span>

<span data-ttu-id="c0662-131">In den folgenden Abschnitten sind einige grundlegende Programmierungsmusteraufrufe der Microsoft Graph-API dargestellt.</span><span class="sxs-lookup"><span data-stu-id="c0662-131">The following sections show a few basic programming pattern calls to the Microsoft Graph API.</span></span>

## <a name="navigate-from-a-set-to-a-member"></a><span data-ttu-id="c0662-132">Navigation von einer Sammlung zu einem Element</span><span class="sxs-lookup"><span data-stu-id="c0662-132">Navigate from a set to a member</span></span>

<span data-ttu-id="c0662-p105">Zum Anzeigen von Informationen zu einem Benutzer müssen Sie die `User`-Entität aus der `users`-Sammlung für den jeweiligen durch seinen Bezeichner angegebenen Benutzer abrufen, indem Sie eine HTTPS-GET-Anforderung verwenden. Für eine `User`-Entität kann entweder die `id`- oder `userPrincipalName`-Eigenschaft als Bezeichner verwendet werden. Im folgenden Anforderungsbeispiel wird der `userPrincipalName`-Wert als Benutzer-ID verwendet.</span><span class="sxs-lookup"><span data-stu-id="c0662-p105">To view the information about a user, you get the `User` entity from the `users` collection to the specific user identified by its identifier, using an HTTPS GET request. For a `User` entity, either the `id` or `userPrincipalName` property can be used as the identifier. The following example request uses the `userPrincipalName` value as the user's id.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="c0662-136">Wenn der Vorgang erfolgreich ist, erhalten Sie den Statuscode 200 OK mit der Benutzerressourcendarstellung in der Nutzlast, wie im Folgenden dargestellt:</span><span class="sxs-lookup"><span data-stu-id="c0662-136">If successful, you should get a 200 OK response containing the user resource representation in the payload, as shown as follows:</span></span>

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 982

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
    "city": "Redmond",
    "country": "USA",
    "department": "Help Center",
    "displayName": "John Doe",
    "givenName": "John",
    "userPrincipalName": "john.doe@contoso.onmicrosoft.com",

    ... 
}
```


## <a name="project-from-an-entity-to-properties"></a><span data-ttu-id="c0662-137">Projektion auf eine Entität in Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c0662-137">Project from an entity to properties</span></span>
<span data-ttu-id="c0662-p106">Um nur biographische Daten des Benutzers abzurufen, z. B. die vom Benutzer bereitgestellte Beschreibung im Feld _Über mich_ und seine Qualifikationen, können Sie den _select_-Abfrageparameter zu der vorherigen Anforderung hinzufügen. Beispiel:</span><span class="sxs-lookup"><span data-stu-id="c0662-p106">To retrieve only the user's biographical data, such as the user's provided _About me_ description and their skill set, you can add the _select_ query parameter to the previous request. For example:</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="c0662-140">Bei erfolgreicher Antwort wird der Statuscode 200 OK zurückgegeben und eine Nutzlast im folgenden Format:</span><span class="sxs-lookup"><span data-stu-id="c0662-140">The successful response returns the 200 OK status and a payload of the following format:</span></span>

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 169

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "aboutMe": "A cool and nice guy.",
    "displayName": "John Doe",
    "skills": [
        "n-Lingual",
        "public speaking",
        "doodling"
    ]
}
```

<span data-ttu-id="c0662-141">Statt aller Eigenschaftensätze für die `user`-Entität werden hier nur die `aboutMe`-, `displayName`- und `skills`-Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="c0662-141">Here, instead of the entire property sets on the `user` entity, only the `aboutMe`, `displayName`, and `skills` properties are returned.</span></span>

## <a name="traverse-to-another-resource-via-relationship"></a><span data-ttu-id="c0662-142">Durchlaufen einer anderen Ressource anhand der Beziehung</span><span class="sxs-lookup"><span data-stu-id="c0662-142">Traverse to another resource via relationship</span></span>
<span data-ttu-id="c0662-p107">Ein Vorgesetzter enthält eine `directReports`-Beziehung zu anderen Benutzern, die diesem unterstellt sind. Zum Abfragen der Liste der direkten Mitarbeiter eines Benutzers können Sie die folgende HTTPS-GET-Anforderung zum Navigieren zum gewünschten Ziel über das Durchlaufen von Beziehungen verwenden.</span><span class="sxs-lookup"><span data-stu-id="c0662-p107">A manager holds a `directReports` relationship with the other users reporting to him or her. To query the list of the direct reports of a user, you can use the following HTTPS GET request to navigate to the intended target via relationship traversal.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="c0662-145">Bei erfolgreicher Antwort wird der Statuscode 200 OK zurückgegeben und eine Nutzlast im folgenden Format:</span><span class="sxs-lookup"><span data-stu-id="c0662-145">The successful response returns the 200 OK status and a payload of the following format:</span></span>

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
content-length: 152
    
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.user",
    "id": "c37b074d-fe9d-4e68-83ad-b4401d3be174",
    "department": "Sales & Marketing",
    "displayName": "Bonnie Kearney",

    ...
}
```

<span data-ttu-id="c0662-p108">Ebenso können Sie anhand einer Beziehung zu verwandten Ressourcen navigieren. Die `user => messages`-Beziehung ermöglicht beispielsweise eine Durchquerung von einem Azure AD-Benutzer zu einer Gruppe von Outlook-E-Mail-Nachrichten. Im nachstehenden Beispiel wird gezeigt, wie dies in einem REST-API-Aufruf funktioniert:</span><span class="sxs-lookup"><span data-stu-id="c0662-p108">Similarly, you can follow a relationship to navigate to related resources. For example, the `user => messages` relationship enables traversal from an Azure AD User to a set of Outlook mail messages. The following example shows how to do this in a REST API call:</span></span>


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer <access_token>
```

    
<span data-ttu-id="c0662-149">Bei erfolgreicher Antwort wird der Statuscode 200 OK zurückgegeben und eine Nutzlast im folgenden Format:</span><span class="sxs-lookup"><span data-stu-id="c0662-149">The successful response returns the 200 OK status and a payload of the following format:</span></span>


```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal
odata-version: 4.0
content-length: 147
    
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/Messages",
  "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/messages?$top=1&$skip=1",
  "value": [
    {
      "@odata.etag": "W/\"FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej\"",
      "id": "<id-value>",
      "createdDateTime": "2015-11-14T00:24:42Z",
      "lastModifiedDateTime": "2015-11-14T00:24:42Z",
      "changeKey": "FwAAABYAAABMR67yw0CmT4x0kVgQUH/3AAJL+Kej",
      "categories": [],
      "receivedDateTime": "2015-11-14T00:24:42Z",
      "sentDateTime": "2015-11-14T00:24:28Z",
      "hasAttachments": false,
      "subject": "Did you see last night's game?",
      "body": {
        "ContentType": "HTML",
        "Content": "<content>"
      },
      "BodyPreview": "it was great!",
      "Importance": "Normal",
            
       ...
    }
  ]
}
```

## <a name="project-from-entities-to-properties"></a><span data-ttu-id="c0662-150">Projektion auf Entitäten in Eigenschaften</span><span class="sxs-lookup"><span data-stu-id="c0662-150">Project from entities to properties</span></span>
<span data-ttu-id="c0662-p109">Neben der Projektion auf eine Entität in ihren Eigenschaften können Sie auch die ähnliche `select`-Abfrageoption auf eine Entitätssammlung anwenden, um eine Projektion auf eine Sammlung mit einigen Eigenschaften durchzuführen. Senden Sie zum Abfragen des Namens der Laufwerkelemente vom angemeldeten Benutzer die folgende HTTPS-GET-Anforderung:</span><span class="sxs-lookup"><span data-stu-id="c0662-p109">In addition to projection from a single entity to its properties, you can also apply the similar `select` query option to an entity collection to project them to a collection of some of their properties. For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request:</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="c0662-153">Bei einer erfolgreichen Antwort werden der Statuscode 200 OK und eine Nutzlast mit den Namen und Typen der freigegebenen Dateien zurückgegeben, wie im folgenden Beispiel dargestellt:</span><span class="sxs-lookup"><span data-stu-id="c0662-153">The successful response returns a 200 OK status code and a payload containing the names and types of the shared files, as shown in the following example:</span></span>

```no-highlight 
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('john.doe%40contoso.onmicrosoft.com')/drive/root/children(name,type)",
  "value": [
    {
      "@odata.etag": "\"{896A8E4D-27BF-424B-A0DA-F073AE6570E2},2\"",
      "name": "Shared with Everyone"
    },
    {
      "@odata.etag": "\"{B39D5D2E-E968-491A-B0EB-D5D0431CB423},1\"",
      "name": "Documents"
    },
    {
      "@odata.etag": "\"{9B51EA38-3EE6-4DC1-96A6-230E325EF054},2\"",
      "name": "newFile.txt"
    }
  ]
}
```

## <a name="query-a-subset-of-users-with-the-filtering-query-option"></a><span data-ttu-id="c0662-154">Abfragen einer Teilmenge von Benutzern mit der Filterabfrageoption</span><span class="sxs-lookup"><span data-stu-id="c0662-154">Query a subset of users with the filtering query option</span></span>
<span data-ttu-id="c0662-p110">Wenn Sie nach Mitarbeitern mit einer bestimmten Position innerhalb Ihrer Organisation suchen möchten, können Sie aus der Benutzersammlung eine _filter_-Abfrageoption angeben. Nachfolgend ein Beispiel:</span><span class="sxs-lookup"><span data-stu-id="c0662-p110">To find the employees of a specific job title within an organization, you can navigate from the users collection and then specify a _filter_ query option. An example is shown as follows:</span></span>

    
```no-highlight 
GET https://graph.microsoft.com/v1.0/users/?$filter=jobTitle+eq+%27Helper%27 HTTP/1.1
Authorization : Bearer <access_token>
```

<span data-ttu-id="c0662-157">Bei einer erfolgreichen Antwort werden der Statuscode 200 OK und eine Liste von Benutzern mit der angegebenen Position (`'Helper'`) zurückgegeben, wie im folgenden Beispiel dargestellt:</span><span class="sxs-lookup"><span data-stu-id="c0662-157">The successful response returns the 200 OK status code and a list of users with the specified job title (`'Helper'`), as shown in the following example:</span></span>

```no-highlight 
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
odata-version: 4.0
content-length: 986

{
    "@odata.context": "https://graph.microsoft.com/v1.0/contoso.onmicrosoft.com/$metadata#users",
    "value": [
        {
            "id": "c95e3b3a-c33b-48da-a6e9-eb101e8a4205",
            "city": "Redmond",
            "country": "USA",
            "department": "Help Center",
            "displayName": "Jane Doe",
            "givenName": "Jane",
            "jobTitle": "Helper",
            ......
            "mailNickname": "Jane",
            "mobile": null,
            "otherMails": [
                "jane.doe@contoso.onmicrosoft.com"
            ],
            ......
            "surname": "Doe",
            "usageLocation": "US",
            "userPrincipalName": "help@contoso.onmicrosoft.com",
            "userType": "Member"
        },
        
        ...
    ]
}
```

## <a name="call-actions-or-functions"></a><span data-ttu-id="c0662-158">Aufrufen von Aktionen oder Funktionen</span><span class="sxs-lookup"><span data-stu-id="c0662-158">Call actions or functions</span></span>
<span data-ttu-id="c0662-p111">Microsoft Graph unterstützt auch _Aktionen_ und _Funktionen_ für die Manipulation von Ressourcen auf eine Art und Weise, wie sie mit Standard-HTTP-Methoden nicht einfach zu realisieren ist. Die folgende HTTPS-POST-Anforderung z. B. ermöglicht es dem angemeldeten Benutzer (`me`), eine E-Mail zu senden:</span><span class="sxs-lookup"><span data-stu-id="c0662-p111">Microsoft Graph also supports _actions_ and _functions_ to manipulate resources in ways that are not a simple fit with standard HTTP methods. For example, the following HTTPS POST request lets the signed-in user (`me`) send an email message:</span></span>
```no-highlight 
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer <access_token>
content-type: application/json
content-length: 96

{
  "message": {
    "subject": "Meet for lunch?",
    "body": {
      "contentType": "Text",
      "content": "The new cafeteria is open."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "garthf@a830edad9050849NDA1.onmicrosoft.com"
        }
      }
    ],
    "attachments": [
      {
        "@odata.type": "microsoft.graph.fileAttachment",
        "name": "menu.txt",
        "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
      }
    ]
  },
  "saveToSentItems": "false"
}
```

<span data-ttu-id="c0662-161">Die Anforderungsnutzlast enthält die Eingabe für die `sendMail`-Aktion, welche auch in $metadata definiert ist.</span><span class="sxs-lookup"><span data-stu-id="c0662-161">The request payload contains the input to the `sendMail` action, which is also defined in the $metadata.</span></span>

## <a name="use-microsoft-graph-client-libraries"></a><span data-ttu-id="c0662-162">Verwenden von Microsoft Graph-Clientbibliotheken</span><span class="sxs-lookup"><span data-stu-id="c0662-162">Use Microsoft Graph client libraries</span></span>
<span data-ttu-id="c0662-p112">Sie bevorzugen die Benutzerfreundlichkeit und die leistungsstarken Funktionen von SDKs? Zwar können Sie Microsoft Graph jederzeit über die REST-API aufrufen; wir stellen jedoch auch SDKs für viele beliebte Plattformen zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="c0662-p112">Like the power and ease of SDKs? While you can always call Microsoft Graph using the REST API, we also provide SDKs for many popular platforms.</span></span>

<span data-ttu-id="c0662-165">Informieren Sie sich unter diesem Link über unsere [SDKs](https://graph.microsoft.io/en-us/code-samples-and-sdks).</span><span class="sxs-lookup"><span data-stu-id="c0662-165">Explore our [SDKs](https://graph.microsoft.io/en-us/code-samples-and-sdks).</span></span>