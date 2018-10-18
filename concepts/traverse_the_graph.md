# <a name="traverse-microsoft-graph"></a><span data-ttu-id="ab718-101">Durchqueren von Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ab718-101">Traverse Microsoft Graph</span></span>

<span data-ttu-id="ab718-p101">Zusätzlich zur Verwendung der Microsoft Graph-API zum Lesen und Schreiben von Daten können Sie eine Reihe von Anforderungsmustern verwenden, um die Ressourcen in Microsoft Graph zu durchlaufen. Mithilfe des Metadatendokuments erhalten Sie auch einen Einblick in die Datenmodelle der Ressourcen und Beziehungen in Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ab718-p101">In addition to using the Microsoft Graph API to read and write data, you can use a number of request patterns to traverse through the resources in Microsoft Graph. The metadata document also helps you to understand the data model of the resources and relationships in Microsoft Graph.</span></span>

## <a name="microsoft-graph-api-metadata"></a><span data-ttu-id="ab718-104">Microsoft Graph-API-Metadaten</span><span class="sxs-lookup"><span data-stu-id="ab718-104">Microsoft Graph API metadata</span></span>

<span data-ttu-id="ab718-p102">Das Metadatendokument ($metadata) wird im Dienststamm veröffentlicht. Über die folgenden URLs können Sie das Dienstdokument für v1.0 und die Betaversionen der Microsoft Graph-API anzeigen.</span><span class="sxs-lookup"><span data-stu-id="ab718-p102">The metadata document ($metadata) is published at the service root. You can view the service document for the v1.0 and beta versions of the Microsoft Graph API via the following URLs.</span></span>

<span data-ttu-id="ab718-107">**Metadaten für Microsoft Graph-API v1.0**</span><span class="sxs-lookup"><span data-stu-id="ab718-107">**Microsoft Graph API v1.0 metadata**</span></span>
```
    https://graph.microsoft.com/v1.0/$metadata
```

<span data-ttu-id="ab718-108">**Metadaten für Microsoft Graph-API Beta**</span><span class="sxs-lookup"><span data-stu-id="ab718-108">**Microsoft Graph API beta metadata**</span></span>

```
    https://graph.microsoft.com/beta/$metadata
```

<span data-ttu-id="ab718-109">Mithilfe der Metadaten können Sie das Datenmodell von Microsoft Graph sehen und verstehen, einschließlich Entitätstypen, komplexen Typen und Aufzählungen, aus denen Ressourcen bestehen, die in den Anforderungs- und Antwortpaketen dargestellt sind.</span><span class="sxs-lookup"><span data-stu-id="ab718-109">The metadata allows you to see and understand the Microsoft Graph data model, including the entity types, complex types, and enumerations that make up the resources represented in the request and response packets.</span></span>

<span data-ttu-id="ab718-110">Die Metadaten können Sie verwenden, um die Beziehungen zwischen Entitäten in Microsoft Graph zu verstehen und URLs einzurichten, die zwischen diesen Entitäten navigieren.</span><span class="sxs-lookup"><span data-stu-id="ab718-110">You can use the metadata to learn the realtionships between entities in Microsoft Graph and establish URLs that navigate between those entities.</span></span>

<span data-ttu-id="ab718-p103">Bei den Pfad-URL-Ressourcennamen, Abfrageparametern sowie den Aktionsparametern und -werten wird nicht nach Groß-/Kleinschreibung unterschieden. Bei zugewiesenen Werten, Entitäts-IDs und anderen base64-codierten Werten wird nach Groß-/Kleinschreibung unterschieden.</span><span class="sxs-lookup"><span data-stu-id="ab718-p103">Path URL resource names, query parameters, and action parameters and values are not case-sensitive. However, values you assign, entity IDs, and other base-64-encoded values are case-sensitive.</span></span>

## <a name="view-a-collection-of-resources"></a><span data-ttu-id="ab718-113">Anzeigen einer Sammlung von Ressourcen</span><span class="sxs-lookup"><span data-stu-id="ab718-113">View a collection of resources</span></span>

<span data-ttu-id="ab718-p104">Mit Microsoft Graph können Sie Ressourcen in einem Mandanten mithilfe von HTTP-GET-Abfragen anzeigen. Die Abfrageantwort umfasst Eigenschaften jeder Ressource, wobei jede Ressource von ihrer ID identifiziert wird. Das Format einer Ressourcen-ID kann eine GUID sein und ist in der Regel je nach Ressourcentyp unterschiedlich.</span><span class="sxs-lookup"><span data-stu-id="ab718-p104">Microsoft Graph lets you view resources in a tenant using HTTP GET queries. The query response includes properties of each resource, with each resource identified by its ID. The format of a resource ID can be a GUID, and generally varies according to the resource type.</span></span> 

<span data-ttu-id="ab718-117">Sie können die Sammlung von in einem Mandanten definierten Benutzern beispielsweise folgendermaßen abrufen:</span><span class="sxs-lookup"><span data-stu-id="ab718-117">For example, you can get the collection of users defined in a tenant:</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/users HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="ab718-p105">Wenn der Vorgang erfolgreich ist, erhalten Sie die Antwort 200 OK mit der Auflistung der [user](../api-reference/v1.0/resources/user.md)-Ressourcen in der Nutzlast. Jeder Benutzer wird anhand der **id**-Eigenschaft und seinen Standardeigenschaften identifiziert. Die nachfolgend dargestellte Arbeitslast ist aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ab718-p105">If successful, you'll get a 200 OK response that contains the collection of [user](../api-reference/v1.0/resources/user.md) resources in the payload. Each user is identified by the **id** property and accompanied by its default properties. The payload shown below is truncated for brevity.</span></span>

```no-highlight 
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "id":"f71f1f74-bf1f-4e6b-b266-c777ea76e2c7",
      "businessPhones":[

      ],
      "displayName":"CIE Administrator",
      "givenName":"CIE",
      "jobTitle":null,
      "mail":"admin@contoso.onmicrosoft.com",
      "mobilePhone":"+1 3528700812",
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Administrator",
      "userPrincipalName":"admin@contoso.onmicrosoft.com"
    },
    {
      "id":"d66f2902-9d12-4ff8-ab01-21ec6706079f",
      "businessPhones":[

      ],
      "displayName":"Alan Steiner",
      "givenName":"Alan",
      "jobTitle":"VP Corporate Marketing",
      "mail":"alans@contoso.onmicrosoft.com",
      "mobilePhone":null,
      "officeLocation":null,
      "preferredLanguage":"en-US",
      "surname":"Steiner",
      "userPrincipalName":"alans@contoso.onmicrosoft.com"
    }
  ]
}
```

<span data-ttu-id="ab718-p106">Mit Microsoft Graph können Sie auch Websitesammlungen anzeigen, indem Sie in den Beziehungen von einer Ressource zu einer anderen navigieren. Über die **mailFolders**-Navigationseigenschaft eines Benutzers können Sie beispielsweise die Auflistung von [mailFolder](../api-reference/v1.0/resources/mailfolder.md)-Ressourcen im Benutzerpostfach abfragen:</span><span class="sxs-lookup"><span data-stu-id="ab718-p106">Microsoft Graph also lets you view collections by navigating the relationships of one resource with another. For example, through a user's **mailFolders** navigation property, you can query for the collection of [mailFolder](../api-reference/v1.0/resources/mailfolder.md) resources in the user's mailbox:</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/mailfolders HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="ab718-p107">Wenn der Vorgang erfolgreich ist, erhalten Sie die Antwort 200 OK mit der Auflistung der [mailFolder](../api-reference/v1.0/resources/user.md)-Ressourcen in der Nutzlast. Jeder **mailFolder** wird anhand der **id**-Eigenschaft und seinen Eigenschaften identifiziert. Die nachfolgend dargestellte Arbeitslast ist aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="ab718-p107">If successful, you'll get a 200 OK response that contains the collection of [mailFolder](../api-reference/v1.0/resources/user.md) resources in the payload. Each **mailFolder** is identified by the **id** property and accompanied by its properties. The payload shown below is truncated for brevity.</span></span>

```no-highlight 
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('16f5a7b6-5a15-4568-aa5a-31bb117e9967')/mailFolders",
  "value":[
    {
      "id":"AAMkADRm9AABDGisXAAA=",
      "displayName":"Archive",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AQMkADRm0AAAIBXAAAAA==",
      "displayName":"Sales reports",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":0,
      "unreadItemCount":0,
      "totalItemCount":0
    },
    {
      "id":"AAMkADRCxI9AAAT6CAIAAA=",
      "displayName":"Conversation History",
      "parentFolderId":"AQMkADRmZWj0AAAIBCAAAAA==",
      "childFolderCount":1,
      "unreadItemCount":0,
      "totalItemCount":0
    }
  ]
}
```




## <a name="view-a-specific-resource-from-a-collection-by-id"></a><span data-ttu-id="ab718-126">Anzeigen einer bestimmten Ressource aus einer Sammlung nach ID</span><span class="sxs-lookup"><span data-stu-id="ab718-126">View a specific resource from a collection by ID</span></span>

<span data-ttu-id="ab718-p108">Wir verwenden weiterhin **user** als Beispiel. Zum Anzeigen der Informationen zu einem Benutzer verwenden Sie eine HTTPS GET-Anforderung, um einen bestimmten Benutzer anhand der Benutzer-ID abzurufen. Für eine **user**-Entität können Sie entweder die **id**- oder die **userPrincipalName**-Eigenschaft als Bezeichner verwenden. Im folgenden Anforderungsbeispiel wird der **userPrincipalName**-Wert als Benutzer-ID verwendet.</span><span class="sxs-lookup"><span data-stu-id="ab718-p108">Continuing with using **user** as an example - to view the information about a user, use an HTTPS GET request to get a specific user by the user's ID. For a **user** entity, you can use either the **id** or **userPrincipalName** property as the identifier. The following request example uses the **userPrincipalName** value as the user's ID.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="ab718-130">Wenn der Vorgang erfolgreich ist, erhalten Sie den Statuscode 200 OK mit der Benutzerressourcendarstellung in der Nutzlast, wie im Folgenden dargestellt.</span><span class="sxs-lookup"><span data-stu-id="ab718-130">If successful, you'll get a 200 OK response that contains the user resource representation in the payload, as shown.</span></span>

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

## <a name="read-specific-properties-of-a-resource"></a><span data-ttu-id="ab718-131">Lesen der spezifischen Eigenschaften einer Ressource</span><span class="sxs-lookup"><span data-stu-id="ab718-131">Read specific properties of a resource</span></span>
<span data-ttu-id="ab718-132">Um nur biographische Daten des Benutzers abzurufen, z. B. die vom Benutzer bereitgestellte Beschreibung im Feld _Über mich_ und seine Qualifikationen, können Sie den [select](query_parameters.md)-Abfrageparameter zu der vorherigen Anforderung hinzufügen, wie im folgenden Beispiel dargestellt.</span><span class="sxs-lookup"><span data-stu-id="ab718-132">To retrieve only the user's biographical data, such as the user's provided _About me_ description and their skill set, you can add the [$select](query_parameters.md) query parameter to the previous request, as shown in the following example.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com?$select=displayName,aboutMe,skills HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="ab718-133">Bei erfolgreicher Antwort wird der Statuscode 200 OK und eine Nutzlast zurückgegeben, wie dargestellt.</span><span class="sxs-lookup"><span data-stu-id="ab718-133">The successful response returns the 200 OK status and a payload, as shown.</span></span>

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
<span data-ttu-id="ab718-134">Statt aller Eigenschaftensätze für die **user**-Entität werden hier nur die grundlegenden **aboutMe**-, **displayName**- und **skills**-Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ab718-134">Here, instead of the entire property sets on the **user** entity, only the **aboutMe**, **displayName**, and **skills** basic properties are returned.</span></span>

## <a name="read-specific-properties-of-the-resources-in-a-collection"></a><span data-ttu-id="ab718-135">Lesen der spezifischen Eigenschaften der Ressourcen in einer Sammlung</span><span class="sxs-lookup"><span data-stu-id="ab718-135">Read specific properties of the resources in a collection</span></span>
<span data-ttu-id="ab718-p109">Zusätzlich zum Lesen spezifischer Eigenschaften einer einzelnen Ressource können Sie auch den ähnlichen Abfrageparameter [$select](query_parameters.md) auf eine Sammlung anwenden, um alle Ressourcen in der Sammlung mit nur den spezifischen Eigenschaften zurückzugeben, die jeweils zurückgegeben werden. Senden Sie zum Abfragen des Namens der Laufwerkelemente vom angemeldeten Benutzer die folgende HTTPS-GET-Anforderung:</span><span class="sxs-lookup"><span data-stu-id="ab718-p109">In addition to reading specific properties of a single resource, you can also apply the similar [$select](query_parameters.md) query parameter to a collection to get back all resources in the collection with just the specific properties returned on each. For example, to query the name of the signed-in user's drive items, you can submit the following HTTPS GET request.</span></span>

```no-highlight 
GET https://graph.microsoft.com/v1.0/me/drive/root/children?$select=name HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="ab718-138">Bei einer erfolgreichen Antwort werden der Statuscode 200 OK und eine Nutzlast mit den Namen der freigegebenen Dateien zurückgegeben, wie im folgenden Beispiel dargestellt:</span><span class="sxs-lookup"><span data-stu-id="ab718-138">The successful response returns a 200 OK status code and a payload that contains only the names of the shared files, as shown in the following example.</span></span>

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

## <a name="traverse-from-one-resource-to-another-via-relationship"></a><span data-ttu-id="ab718-139">Durchqueren von einer Ressource zu einer anderen anhand der Beziehung</span><span class="sxs-lookup"><span data-stu-id="ab718-139">Traverse from one resource to another via relationship</span></span>
<span data-ttu-id="ab718-p110">Ein Vorgesetzter enthält eine **directReports**-Beziehung zu anderen Benutzern, die diesem unterstellt sind. Zum Abfragen der Liste der direkten Mitarbeiter eines Benutzers können Sie die folgende HTTPS-GET-Anforderung zum Navigieren zum gewünschten Ziel über das Durchlaufen von Beziehungen verwenden.</span><span class="sxs-lookup"><span data-stu-id="ab718-p110">A manager holds a **directReports** relationship with the other users reporting to him or her. To query the list of the direct reports of a user, you can use the following HTTPS GET request to navigate to the intended target via relationship traversal.</span></span> 

```no-highlight 
GET https://graph.microsoft.com/v1.0/users/john.doe@contoso.onmicrosoft.com/directReports HTTP/1.1
Authorization : Bearer {access_token}
```

<span data-ttu-id="ab718-142">Bei erfolgreicher Antwort wird der Statuscode 200 OK und eine Nutzlast zurückgegeben, wie dargestellt.</span><span class="sxs-lookup"><span data-stu-id="ab718-142">The successful response returns the 200 OK status and a payload, as shown.</span></span>

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

<span data-ttu-id="ab718-p111">Ebenso können Sie anhand einer Beziehung zu verwandten Ressourcen navigieren. Die user-messages-Beziehung ermöglicht beispielsweise eine Durchquerung von einem Azure Active Directory-Benutzer zu einer Gruppe von Outlook-E-Mail-Nachrichten. Im nachstehenden Beispiel wird gezeigt, wie dies in einem REST-API-Aufruf funktioniert:</span><span class="sxs-lookup"><span data-stu-id="ab718-p111">Similarly, you can follow a relationship to navigate to related resources. For example, the user-messages relationship enables traversal from an Azure Active Directory (Azure AD) User to a set of Outlook mail messages. The following example shows how to do this in a REST API call.</span></span>


```no-highlight 
GET https://graph.microsoft.com/v1.0/me/messages HTTP/1.1
Authorization : Bearer {access_token}
```

    
<span data-ttu-id="ab718-146">Bei erfolgreicher Antwort wird der Statuscode 200 OK und eine Nutzlast zurückgegeben, wie dargestellt.</span><span class="sxs-lookup"><span data-stu-id="ab718-146">The successful response returns the 200 OK status and a payload, as shown.</span></span>


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
<span data-ttu-id="ab718-147">Sie können alle Beziehungen in einer bestimmten Ressource anzeigen, indem Sie zu den Metadaten wechseln, den EntityType suchen und sich alle NavigationProperties für diesen EntityType ansehen.</span><span class="sxs-lookup"><span data-stu-id="ab718-147">You can see all the relationships on a given resource by going to the metadata, finding the EntityType, and looking at all NavigationProperties for that EntityType.</span></span>

## <a name="call-functions"></a><span data-ttu-id="ab718-148">Aufruffunktionen</span><span class="sxs-lookup"><span data-stu-id="ab718-148">Call functions</span></span>
<span data-ttu-id="ab718-p112">Microsoft Graph unterstützt auch _Funktionen_ zum Bearbeiten von Ressourcen auf andere Art und Weise als einfache CRUD-Vorgänge (Erstellen, Lesen, Aktualisieren und Löschen). Diese liegen häufig in der Form von HTTPS-POST-Anforderungen vor, um Argumente für die Funktion aufzunehmen. Die folgende HTTPS-POST-Anforderung z. B. ermöglicht es dem angemeldeten Benutzer (`me`), eine E-Mail zu senden.</span><span class="sxs-lookup"><span data-stu-id="ab718-p112">Microsoft Graph also supports _functions_ to manipulate resources in ways that are not simply create, read, update, and delete (CRUD) operations. They are often in the shape of HTTPS POST requests in order to intake arguments for the function. For example, the following function lets the signed-in user (`me`) send an email message.</span></span>

```no-highlight 
POST https://graph.microsoft.com/v1.0/me/sendMail HTTP/1.1
authorization: bearer {access_token}
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

<span data-ttu-id="ab718-p113">Sie können alle verfügbaren Funktionen in den Metadaten sehen. Sie werden als Funktionen oder Aktionen angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ab718-p113">You can see all the functions that are available in the metadata. They appear as Functions or Actions.</span></span>

## <a name="use-the-microsoft-graph-sdks"></a><span data-ttu-id="ab718-154">Verwendung der Microsoft Graph-SDKs</span><span class="sxs-lookup"><span data-stu-id="ab718-154">Use the Microsoft Graph SDKs</span></span>

<span data-ttu-id="ab718-p114">Sie bevorzugen die Benutzerfreundlichkeit und die leistungsstarken Funktionen von SDKs? Zwar können Sie Microsoft Graph jederzeit über REST-APIs aufrufen; wir stellen jedoch auch SDKs für viele beliebte Plattformen zur Verfügung. Unter [Codebeispiele und SDKs](https://graph.microsoft.io/en-us/code-samples-and-sdks) können Sie die verfügbaren SDKs erkunden.</span><span class="sxs-lookup"><span data-stu-id="ab718-p114">Like the power and ease of SDKs? While you can always use REST APIs to call Microsoft Graph, we also provide SDKs for many popular platforms. To explore the SDKs that are available, see [Code samples and SDKs](https://graph.microsoft.io/en-us/code-samples-and-sdks).</span></span>

## <a name="see-also"></a><span data-ttu-id="ab718-158">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="ab718-158">See also</span></span>

- [<span data-ttu-id="ab718-159">Verwenden der Microsoft Graph-API</span><span class="sxs-lookup"><span data-stu-id="ab718-159">Use the Microsoft Graph API</span></span>](use_the_api.md)
- [<span data-ttu-id="ab718-160">Authentifizierungstoken abrufen</span><span class="sxs-lookup"><span data-stu-id="ab718-160">Get auth tokens</span></span>](auth_overview.md)