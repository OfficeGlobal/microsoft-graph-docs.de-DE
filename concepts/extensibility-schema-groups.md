---
title: 'Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen '
description: 'Sie werden durch ein Beispiel geführt, um die Verwendung von *Schemaerweiterungen* zu veranschaulichen. '
author: dkershaw10
ms.openlocfilehash: 101e4569d05a36a55cc264ef806df312f2667aa8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353599"
---
# <a name="add-custom-data-to-groups-using-schema-extensions"></a><span data-ttu-id="7cdf8-103">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="7cdf8-103">Add custom data to groups using schema extensions</span></span> 

<span data-ttu-id="7cdf8-104">Sie werden durch ein Beispiel geführt, um die Verwendung von *Schemaerweiterungen* zu veranschaulichen.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-104">We're going to walk you through an example to demonstrate how to use *schema extensions*.</span></span> 

<span data-ttu-id="7cdf8-p101">Angenommen, Sie sind ein Entwickler in einem Unternehmen für Lernverwaltungssoftware mit dem Namen „Graph Learn“, das Schulungskurse und Materialien für Unternehmen erstellt.  Office 365-Gruppen mit ihren vielfältigen Oberflächen für die Zusammenarbeit bieten eine hervorragende Möglichkeit zur Bereitstellung von Kursinhalten und zum Aufzeichnen von Übungen unter Teilnehmern, sowohl für Onlinekurse als auch für Kurse mit Kursleitern.  Es bietet sich an, die Office 365-Gruppen, die für Schulungskurse verwendet werden, leicht erkennbar zu gestalten, sodass andere Entwickler Ihre Gruppen auffinden und vielfältige Oberflächen zusätzlich zu Ihren Lernkursen erstellen können.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-p101">Imagine you're a developer in a Learning Management Software company called “Graph Learn” that builds training courses and materials for businesses.  Office 365 groups, with their rich collaborative experiences, is a fantastic way to deliver course content and record exercises among participants for both online courses and instructor-led courses.  You may want to make those Office 365 groups used for training courses easily identifiable as training courses, which will allow other developers to discover your groups and build rich experiences on top of your learning courses.</span></span>

<span data-ttu-id="7cdf8-108">In diesem Szenario erlernen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="7cdf8-108">For this scenario, we're going to show you how to:</span></span>

1. <span data-ttu-id="7cdf8-109">Anzeigen verfügbarer Schemaerweiterungsdefinitionen, die Sie verwenden können</span><span class="sxs-lookup"><span data-stu-id="7cdf8-109">View available schema extension definitions that you could use.</span></span>
2. <span data-ttu-id="7cdf8-110">Registrieren einer Schemaerweiterungsdefinition, die auf Gruppen für Schulungskurse abzielt</span><span class="sxs-lookup"><span data-stu-id="7cdf8-110">Register a schema extension definition that targets groups for training courses.</span></span>
3. <span data-ttu-id="7cdf8-111">Erstellen einer neuen Gruppe mit erweiterten Daten basierend auf der Schemaerweiterungsdefinition, die Sie soeben registriert haben</span><span class="sxs-lookup"><span data-stu-id="7cdf8-111">Create a new group with extended data based on the schema extension definition that you just registered.</span></span>
4. <span data-ttu-id="7cdf8-112">Hinzufügen, Aktualisieren oder Entfernen von benutzerdefinierten Daten in einer vorhandenen Gruppe basierend auf einer Schemaerweiterungsdefinition</span><span class="sxs-lookup"><span data-stu-id="7cdf8-112">Add, update, or remove custom data in an existing group based on a schema extension definition.</span></span>
5. <span data-ttu-id="7cdf8-113">Einlesen einer Gruppe und der Erweiterungsdaten</span><span class="sxs-lookup"><span data-stu-id="7cdf8-113">Read back a group and the extension data.</span></span>

><span data-ttu-id="7cdf8-p102">**Hinweis:** In diesem Artikel erfahren Sie, wie Sie Schemaerweiterungswerte in einer **group**-Ressource erstellen und lesen können (Schritte 3 bis 5).  Diese Methoden werden auch von Ressourcen des Typs **administrativeUnit**, **device**, **event**, **message**, **organization**, **post** und **user** unterstützt.  Sie können also auf jede dieser Ressourcen ähnliche Vorgänge wie die unten beschriebenen Beispielanforderungen anwenden. Beachten Sie, dass  **administrativeUnit** nur im Beta-Endpunkt verfügbar ist.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-p102">**Note:** This topic shows you how to create and read schema extension values on a **group** resource (steps 3-5).  The same methods are supported for the **administrativeUnit**, **device**, **event**, **message**, **organization**, **post**, and **user** resource types as well.  So you can carry out similar operations as the example requests below on any of those resources. Note that **administrativeUnit** is available only in the beta endpoint.</span></span>

## <a name="1-view-available-schema-extensions"></a><span data-ttu-id="7cdf8-118">1. Anzeigen verfügbarer Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="7cdf8-118">1. View available schema extensions</span></span>
<span data-ttu-id="7cdf8-p103">Als Entwickler möchten Sie wahrscheinlich zuerst prüfen, ob es bereits andere Schemaerweiterungsdefinitionen gibt, die Sie für Ihre App wiederverwenden könnten.  Das können Sie durch Abfragen der Ressource **schemaExtension** tun.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-p103">First, as a developer, you might want to find any other schema extension definitions that our app could reuse.  This can be done by querying the **schemaExtension** resource.</span></span>  
<span data-ttu-id="7cdf8-121">Im Beispiel unten fragen Sie eine spezifische Schemaerweiterung anhand ihres **id**-Werts ab.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-121">In the example below, you're going to query for a specific schema extension by **id**.</span></span>

<span data-ttu-id="7cdf8-p104">Beachten Sie: Die in der Antwort zurückgegebene Erweiterung hat den **status**-Wert **Available**. Das bedeutet, dass jede App, die zum Zugriff auf die in der Eigenschaft **targetTypes** definierten Ressourcen berechtigt ist, die Erweiterung verwenden und mit additiven Änderungen aktualisieren kann. Im Allgemeinen gibt dieser Vorgang alle Schemaerweiterungen zurück, die dem angegebenen Filter entsprechen, unabhängig von ihrem **status**-Wert. Bevor Sie eine Erweiterung verwenden, sollten Sie also immer ihren Status überprüfen.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-p104">Notice that the extension returned in the response has **Available** as the **status** value, which indicates that any app which has permission to the resources in the **targetTypes** property can use and update the extension with additive changes. In general, this operation returns any schema extensions that satisfy the specified filter regardless of **status**, so do check the extension status before using it.</span></span>


##### <a name="request"></a><span data-ttu-id="7cdf8-124">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cdf8-124">Request</span></span>
```http
GET https://graph.microsoft.com/v1.0/schemaExtensions?$filter=id eq 'graphlearn_test'
```
##### <a name="response"></a><span data-ttu-id="7cdf8-125">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cdf8-125">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420
{
    "value": [
        {
            "id":"graphlearn_test",
            "description": "Yet another test schema",
            "targetTypes": [
                "User", "Group"
            ],
            "status": "Available",
            "owner": "24d3b144-21ae-4080-943f-7067b395b913",
            "properties": [
                {
                    "name": "testName",
                    "type": "String"
                }
            ]
        }
    ]
}
```
## <a name="2-register-a-schema-extension-definition-that-describes-a-training-course"></a><span data-ttu-id="7cdf8-126">2. Registrieren einer Schemaerweiterungsdefinition, die einen Schulungskurs beschreibt</span><span class="sxs-lookup"><span data-stu-id="7cdf8-126">2. Register a schema extension definition that describes a training course</span></span>
<span data-ttu-id="7cdf8-127">Wenn Sie keine Schemaerweiterung finden, die ihren Anforderungen *bereits entspricht*, können Sie eine neue Erweiterungsdefinition für Schulungskurse in der **group**-Ressource erstellen und registrieren.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-127">If you can't find a schema extension that *is* appropriate for your needs, you can create and register a new extension definition for training courses on the **group** resource.</span></span>  

<span data-ttu-id="7cdf8-p105">Beim Erstellen einer Schemaerweiterungsdefinition sollten Sie eine Zeichenfolge für die **id**-Eigenschaft angeben. Sie können auf zwei Arten vorgehen: Das folgende Beispiel zeigt die bevorzugte Methode, die einen Vanity-Domänennamen (`graphlearn.com`) verwendet, der mit Ihrem Mandanten überprüft wurde. Verketten Sie den überprüften Domänennamen (`graphlearn`) mit einem Namen für die Schemaerweiterung (`courses`), und weisen Sie **id** mit der resultierenden Zeichenfolge, `graphlearn_courses`, zu.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-p105">When creating a schema extension definition, you should provide a string for the **id** property. There are two ways to do this. The following example shows the preferred way, which uses a vanity domain name (`graphlearn.com`) that has been verified with your tenant. Concatenate the verified domain name (`graphlearn`) with a name for the schema extension (`courses`), and assign **id** with the resultant string, `graphlearn_courses`.</span></span>  

<span data-ttu-id="7cdf8-p106">Geben Sie dann eine Beschreibung (zwecks Erkennbarkeit), die Zieltypen (d. h. die Ressourcen, auf die die Erweiterung angewendet werden kann) und die benutzerdefinierten Eigenschaften an, die das Schema bilden sollen.  In diesem Beispiel geben Sie die benutzerdefinierten Eigenschaften `courseId`, `courseName` und `courseType` sowie deren Typen an.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-p106">Then, specify a description (to enable discoverability), target types (defining which resources this extension applies to), and the custom properties that make up the schema.  In this example, specify the `courseId`, `courseName` and `courseType` custom properties and their types.</span></span>

<span data-ttu-id="7cdf8-134">Sehen Sie sich ein [Beispiel für die andere Möglichkeit zum Zuweisen von **id** in der Anforderung](/graph/api/schemaextension-post-schemaextensions?view=graph-rest-1.0#request-2) an, für die nur ein Schemaname angegeben werden muss.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-134">See an [example of the other way to assign **id** in the request](/graph/api/schemaextension-post-schemaextensions?view=graph-rest-1.0#request-2), that requires you to provide only a schema name.</span></span>

<span data-ttu-id="7cdf8-p107">Beachten Sie: Bei der Ersterstellung einer Schemaerweiterung hat diese den Status **InDevelopment**. Sie können die Erweiterung während der weiteren Entwicklung in diesem Status belassen. Dann kann die Erweiterung nur von der App mit additiven Änderungen aktualisiert oder gelöscht werden, von der sie erstellt wurde. Sobald die Erweiterung für andere Apps verfügbar sein soll, können Sie den Wert **status** auf **Available** setzen.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-p107">Notice that when you initially create a schema extension, its status is **InDevelopment**. While you're developing the extension, you can keep it in this status, during which only your app that created it can update it with additive changes or delete it. When you are ready to share the extension for use by other apps, set **status** to **Available**.</span></span>

##### <a name="request"></a><span data-ttu-id="7cdf8-138">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cdf8-138">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/schemaExtensions
Content-type: application/json
{
    "id":"graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```
##### <a name="response"></a><span data-ttu-id="7cdf8-139">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cdf8-139">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "graphlearn_courses",
    "description": "Graph Learn training courses extensions",
    "targetTypes": [
        "Group"
    ],
    "status": "InDevelopment",
    "owner": "24d3b144-21ae-4080-943f-7067b395b913",
    "properties": [
        {
            "name": "courseId",
            "type": "Integer"
        },
        {
            "name": "courseName",
            "type": "String"
        },
        {
            "name": "courseType",
            "type": "String"
        }
    ]
}
```

## <a name="3-create-a-new-group-with-extended-data"></a><span data-ttu-id="7cdf8-140">3. Erstellen einer neuen Gruppe mit erweiterten Daten</span><span class="sxs-lookup"><span data-stu-id="7cdf8-140">3. Create a new group with extended data</span></span> 
<span data-ttu-id="7cdf8-p108">Erstellen Sie eine _neue_ Gruppe, und erweitern Sie sie unter Verwendung der soeben registrierten Schemaerweiterungsdefinition `graphlearn_courses` mit zusätzlichen Daten.  Dies ist ein standardmäßiger ```POST``` für die **group**-Ressource, wobei die zusätzliche Erweiterung `graphlearn_courses` mit komplexem Typ im Anforderungstext definiert ist.  Die Antwort spiegelt keine Datenerweiterungen wider. Für die Erweiterung muss explizit ```$select``` anhand des Namens unter Verwendung eines ```GET```-Vorgangs durchgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-p108">Create a _new_ group and extend it with extra data using the `graphlearn_courses` schema extension definition that we just registered.  This is a standard ```POST``` to the **group** resource, with the additional `graphlearn_courses` complex type extension defined in the request body.  The response will not mirror back any data extensions. We need to explicitly ```$select``` the extension by name using a ```GET``` operation.</span></span>

##### <a name="request"></a><span data-ttu-id="7cdf8-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cdf8-145">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
{
    "displayName": "New Managers March 2017",
    "description": "New Managers training course for March 2017",
    "groupTypes": ["Unified"],
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "graphlearn_courses": {
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }
}
```
##### <a name="response"></a><span data-ttu-id="7cdf8-146">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cdf8-146">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420
{
    "id": "dfc8016f-db97-4c47-a582-49cb8f849355",
    "createdDateTime": "2017-02-09T00:17:05Z",
    "description": "New Managers training course for March 2017",
    "displayName": "New Managers March 2017",
    "groupTypes": [
        "Unified"
    ],
    "mail": "newMan201703@graphlearn.com",
    "mailEnabled": true,
    "mailNickname": "newMan201703",
    "securityEnabled": false,
    "theme": null,
    "visibility": "Public"
}
```

## <a name="4-add-update-or-remove-custom-data-in-an-existing-group"></a><span data-ttu-id="7cdf8-147">4. Hinzufügen, Aktualisieren oder Entfernen von benutzerdefinierten Daten in einer vorhandenen Gruppe</span><span class="sxs-lookup"><span data-stu-id="7cdf8-147">4. Add, update, or remove custom data in an existing group</span></span>
<span data-ttu-id="7cdf8-148">Sie können eine _vorhandene_ Gruppeninstanz mit der zusätzlichen Erweiterung `graphlearn_courses` mit komplexem Typ, die im Textkörper einer ```PATCH```-Anforderung definiert ist, erweitern und ihr benutzerdefinierte Daten hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-148">You can extend and add custom data to an _existing_ group instance with the additional `graphlearn_courses` complex type extension defined in the body of a ```PATCH``` request.</span></span>  

##### <a name="request"></a><span data-ttu-id="7cdf8-149">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cdf8-149">Request</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/groups/dfc8016f-db97-4c47-a582-49cb8f849355
Content-type: application/json
Content-length: 230
{
    "graphlearn_courses":{
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
    }   
}
```
##### <a name="response"></a><span data-ttu-id="7cdf8-150">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cdf8-150">Response</span></span>
```http
HTTP/1.1 204 No Content
```

<span data-ttu-id="7cdf8-151">Wenn Sie die Werte der Erweiterungsdaten aktualisieren möchten, platzieren Sie die gesamte Erweiterung des komplexen Typs im Textkörper einer ```PATCH```-Anforderung (ähnlich wie das Hinzufügen von benutzerdefinierten Daten zu einer vorhandenen Ressource).</span><span class="sxs-lookup"><span data-stu-id="7cdf8-151">If you want to update the values of the extension data, put the entire extension complex type in the body of a ```PATCH``` request (similar to adding custom data to an existing resource).</span></span>

<span data-ttu-id="7cdf8-152">Sie können benutzerdefinierte Daten, die einer Ressourceninstanz hinzugefügt wurden, auch entfernen, indem Sie die entsprechende Erweiterungseigenschaft auf NULL festlegen.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-152">You can also remove custom data added to a resource instance by setting the corresponding extension property to null.</span></span> 

<span data-ttu-id="7cdf8-153">Um eine Schemaerweiterung aus einer Ressourceninstanz zu entfernen, legen Sie die Erweiterung mit komplexem Typ in der betreffenden Instanz auf NULL fest.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-153">To remove a schema extension from a resource instance, set the extension complex type in that instance to null.</span></span>


## <a name="5-get-a-group-and-its-extension-data"></a><span data-ttu-id="7cdf8-154">5. Abrufen einer Gruppe und ihrer Erweiterungsdaten</span><span class="sxs-lookup"><span data-stu-id="7cdf8-154">5. Get a group and its extension data</span></span>
<span data-ttu-id="7cdf8-155">Eine praktische Möglichkeit zum Suchen nach einer Gruppe (oder Gruppen) ist die Verwendung von `$filter`, um bestimmte Erweiterungseigenschaftswerte abzugleichen, z. B. Erweiterungsname oder -ID.</span><span class="sxs-lookup"><span data-stu-id="7cdf8-155">A handy way to look for a group (or groups) is to use `$filter` to match for specific extension property values, such as an extension name or ID.</span></span> 

<span data-ttu-id="7cdf8-156">Um die benutzerdefinierten Daten in einer Gruppe abzurufen, verwenden Sie dann `$select` zum Einschließen der Erweiterung nach Name (in diesem Fall `graphlearn_courses`).</span><span class="sxs-lookup"><span data-stu-id="7cdf8-156">Then, to get the custom data in a group, use `$select` to include the extension by name (in this case by `graphlearn_courses`).</span></span>

<span data-ttu-id="7cdf8-p109">Im folgenden Beispiel wird nach der Gruppe mit der Erweiterung `graphlearn_courses` gesucht, deren `courseId`-Eigenschaft den Wert `123` hat, und es werden die Gruppeneigenschaften **displayName**, **id** und **description** sowie die benutzerdefinierten Daten in der Erweiterung `graphlearn_courses` abgerufen. (Denken Sie daran, in der tatsächlichen Abfrage URL-Codierung nach Bedarf anzuwenden.)</span><span class="sxs-lookup"><span data-stu-id="7cdf8-p109">The following example looks for the group that has the `graphlearn_courses` extension with a `courseId` property value matching `123`, and gets the group properties **displayName**, **id**, and **description**, and the custom data in the `graphlearn_courses` extension. (In the actual query, make sure you apply URL encoding as necessary.)</span></span>

#### <a name="request"></a><span data-ttu-id="7cdf8-159">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7cdf8-159">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


##### <a name="response"></a><span data-ttu-id="7cdf8-160">Antwort</span><span class="sxs-lookup"><span data-stu-id="7cdf8-160">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
  "value": [
    {
      "displayName": "New Managers March 2017",
      "id": "14429ae5-3e74-41a2-9fa8-028fbb984637",
      "description": "New Managers training course for March 2017",
      "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
      }
    }
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="7cdf8-161">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="7cdf8-161">See also</span></span>

- [<span data-ttu-id="7cdf8-162">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="7cdf8-162">Add custom data to resources using extensions</span></span>](extensibility-overview.md)
- [<span data-ttu-id="7cdf8-163">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="7cdf8-163">Add custom data to users using open extensions (preview)</span></span>](extensibility-open-users.md)
- [<span data-ttu-id="7cdf8-164">Office 365-Domänen</span><span class="sxs-lookup"><span data-stu-id="7cdf8-164">Office 365 domains</span></span>](https://technet.microsoft.com/de-DE/library/office-365-domains.aspx)
- [<span data-ttu-id="7cdf8-165">Hinzufügen und Überprüfen einer Domäne für das NEUE Office 365</span><span class="sxs-lookup"><span data-stu-id="7cdf8-165">Adding and Verifying a Domain for the NEW Office 365</span></span>](https://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [<span data-ttu-id="7cdf8-166">schemaExtension-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="7cdf8-166">schemaExtension resource type</span></span>](/graph/api/resources/schemaextension?view=graph-rest-1.0)
- [<span data-ttu-id="7cdf8-167">schemaExtensions aufführen</span><span class="sxs-lookup"><span data-stu-id="7cdf8-167">List schemaExtensions</span></span>](/graph/api/schemaextension-list?view=graph-rest-1.0)
- [<span data-ttu-id="7cdf8-168">schemaExtension erstellen</span><span class="sxs-lookup"><span data-stu-id="7cdf8-168">Create schemaExtension</span></span>](/graph/api/schemaextension-post-schemaextensions?view=graph-rest-1.0)
- [<span data-ttu-id="7cdf8-169">schemaExtension abrufen</span><span class="sxs-lookup"><span data-stu-id="7cdf8-169">Get schemaExtension</span></span>](/graph/api/schemaextension-get?view=graph-rest-1.0)
- [<span data-ttu-id="7cdf8-170">schemaExtension aktualisieren</span><span class="sxs-lookup"><span data-stu-id="7cdf8-170">Update schemaExtension</span></span>](/graph/api/schemaextension-update?view=graph-rest-1.0)
- [<span data-ttu-id="7cdf8-171">schemaExtension löschen</span><span class="sxs-lookup"><span data-stu-id="7cdf8-171">Delete schemaExtension</span></span>](/graph/api/schemaextension-delete?view=graph-rest-1.0)
