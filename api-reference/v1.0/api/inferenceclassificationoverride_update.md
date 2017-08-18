# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="a20a1-101">inferenceclassificationoverride aktualisieren</span><span class="sxs-lookup"><span data-stu-id="a20a1-101">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="a20a1-102">Ändert das **classifyAs**-Feld einer Außerkraftsetzung wie angegeben.</span><span class="sxs-lookup"><span data-stu-id="a20a1-102">Change the **classifyAs** field of an override as specified.</span></span> 

<span data-ttu-id="a20a1-103">Sie können PATCH nicht zum Ändern von anderen Feldern in einer [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md)-Instanz verwenden.</span><span class="sxs-lookup"><span data-stu-id="a20a1-103">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) instance.</span></span> 

<span data-ttu-id="a20a1-104">Wenn eine Außerkraftsetzung für einen Absender vorhanden ist und der Absender den Anzeigenamen ändert, können Sie [POST](inferenceclassification_post_overrides.md) zum Erzwingen einer Aktualisierung des Namensfelds in der vorhandenen Außerkraftsetzung verwenden.</span><span class="sxs-lookup"><span data-stu-id="a20a1-104">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification_post_overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="a20a1-105">Wenn eine Außerkraftsetzung für einen Absender vorhanden ist und der Absender die SMTP-Adresse ändert, können Sie die Außerkraftsetzung für diesen Absender nur „aktualisieren“, indem Sie die vorhandene Außerkraftsetzung [löschen](inferenceclassificationoverride_delete.md) und eine neue Außerkraftsetzung mit der neuen SMTP-Adresse [erstellen](inferenceclassification_post_overrides.md).</span><span class="sxs-lookup"><span data-stu-id="a20a1-105">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride_delete.md) the existing override and [creating](inferenceclassification_post_overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a20a1-106">Voraussetzungen</span><span class="sxs-lookup"><span data-stu-id="a20a1-106">Prerequisites</span></span>
<span data-ttu-id="a20a1-107">Die folgenden **Bereiche** sind erforderlich, um diese API auszuführen: *Mail.ReadWrite*</span><span class="sxs-lookup"><span data-stu-id="a20a1-107">The following **scopes** are required to execute this API: *Mail.ReadWrite*</span></span>
## <a name="http-request"></a><span data-ttu-id="a20a1-108">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a20a1-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a20a1-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a20a1-109">Request headers</span></span>
| <span data-ttu-id="a20a1-110">Name</span><span class="sxs-lookup"><span data-stu-id="a20a1-110">Name</span></span>       | <span data-ttu-id="a20a1-111">Typ</span><span class="sxs-lookup"><span data-stu-id="a20a1-111">Type</span></span> | <span data-ttu-id="a20a1-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a20a1-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a20a1-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="a20a1-113">Authorization</span></span>  | <span data-ttu-id="a20a1-114">string</span><span class="sxs-lookup"><span data-stu-id="a20a1-114">string</span></span>  | <span data-ttu-id="a20a1-p101">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a20a1-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a20a1-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a20a1-117">Content-Type</span></span> | <span data-ttu-id="a20a1-118">string</span><span class="sxs-lookup"><span data-stu-id="a20a1-118">string</span></span>  | <span data-ttu-id="a20a1-p102">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a20a1-p102">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a20a1-121">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a20a1-121">Request body</span></span>
<span data-ttu-id="a20a1-p103">Geben Sie im Anforderungstext den neuen Wert für **classifyAs** an. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="a20a1-p103">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="a20a1-124">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a20a1-124">Property</span></span>     | <span data-ttu-id="a20a1-125">Typ</span><span class="sxs-lookup"><span data-stu-id="a20a1-125">Type</span></span>   |<span data-ttu-id="a20a1-126">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a20a1-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a20a1-127">classifyAs</span><span class="sxs-lookup"><span data-stu-id="a20a1-127">classifyAs</span></span>|<span data-ttu-id="a20a1-128">string</span><span class="sxs-lookup"><span data-stu-id="a20a1-128">string</span></span>| <span data-ttu-id="a20a1-p104">Gibt an, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen. Mögliche Werte: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="a20a1-p104">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="a20a1-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="a20a1-131">Response</span></span>

<span data-ttu-id="a20a1-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a20a1-132">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a20a1-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a20a1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a20a1-134">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a20a1-134">Request</span></span>
<span data-ttu-id="a20a1-135">Im folgenden Beispiel wird die Außerkraftsetzung für die SMTP-Adresse „randiw@adatum.onmicrosoft.com“ von `other` zu `focused` geändert.</span><span class="sxs-lookup"><span data-stu-id="a20a1-135">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_inferenceclassificationoverride"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/inferenceClassification/overrides/{id}
Content-type: application/json

{
  "classifyAs": "focused"
}
```
##### <a name="response"></a><span data-ttu-id="a20a1-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="a20a1-136">Response</span></span>
<span data-ttu-id="a20a1-p105">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a20a1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "classifyAs": "focused",
  "senderEmailAddress": {
    "name": "Randi Welch",
    "address": "randiw@adatum.onmicrosoft.com"
  },
  "id": "98f5bdef-576a-404d-a2ea-07a3cf34af4r"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update inferenceclassificationoverride",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->