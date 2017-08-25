# <a name="update-inferenceclassificationoverride"></a><span data-ttu-id="150a0-101">inferenceclassificationoverride aktualisieren</span><span class="sxs-lookup"><span data-stu-id="150a0-101">Update inferenceclassificationoverride</span></span>

<span data-ttu-id="150a0-102">Ändert das **classifyAs**-Feld einer Außerkraftsetzung wie angegeben.</span><span class="sxs-lookup"><span data-stu-id="150a0-102">Change the **classifyAs** field of an override as specified.</span></span> 

<span data-ttu-id="150a0-103">Sie können PATCH nicht zum Ändern von anderen Feldern in einer [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md)-Instanz verwenden.</span><span class="sxs-lookup"><span data-stu-id="150a0-103">You cannot use PATCH to change any other fields in an [inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) instance.</span></span> 

<span data-ttu-id="150a0-104">Wenn eine Außerkraftsetzung für einen Absender vorhanden ist und der Absender den Anzeigenamen ändert, können Sie [POST](inferenceclassification_post_overrides.md) zum Erzwingen einer Aktualisierung des Namensfelds in der vorhandenen Außerkraftsetzung verwenden.</span><span class="sxs-lookup"><span data-stu-id="150a0-104">If an override exists for a sender and the sender changes his/her display name, you can use [POST](inferenceclassification_post_overrides.md) to force an update to the name field in the existing override.</span></span>

<span data-ttu-id="150a0-105">Wenn eine Außerkraftsetzung für einen Absender vorhanden ist und der Absender die SMTP-Adresse ändert, können Sie die Außerkraftsetzung für diesen Absender nur „aktualisieren“, indem Sie die vorhandene Außerkraftsetzung [löschen](inferenceclassificationoverride_delete.md) und eine neue Außerkraftsetzung mit der neuen SMTP-Adresse [erstellen](inferenceclassification_post_overrides.md).</span><span class="sxs-lookup"><span data-stu-id="150a0-105">If an override exists for a sender and the sender changes his/her SMTP address, [deleting](inferenceclassificationoverride_delete.md) the existing override and [creating](inferenceclassification_post_overrides.md) a new one with the new SMTP address is the only way to "update" the override for this sender.</span></span>

## <a name="permissions"></a><span data-ttu-id="150a0-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="150a0-106">Permissions</span></span>
<span data-ttu-id="150a0-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="150a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="150a0-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="150a0-109">Permission type</span></span>      | <span data-ttu-id="150a0-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="150a0-110">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="150a0-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="150a0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="150a0-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="150a0-112">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="150a0-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="150a0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="150a0-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="150a0-114">Mail.ReadWrite</span></span>    | 
|<span data-ttu-id="150a0-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="150a0-115">Application</span></span> | <span data-ttu-id="150a0-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="150a0-116">Mail.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="150a0-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="150a0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/inferenceClassification/overrides/{id}
PATCH /users/{id}/inferenceClassification/overrides/{id}
```

## <a name="request-headers"></a><span data-ttu-id="150a0-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="150a0-118">Request headers</span></span>
| <span data-ttu-id="150a0-119">Name</span><span class="sxs-lookup"><span data-stu-id="150a0-119">Name</span></span>       | <span data-ttu-id="150a0-120">Typ</span><span class="sxs-lookup"><span data-stu-id="150a0-120">Type</span></span> | <span data-ttu-id="150a0-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="150a0-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="150a0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="150a0-122">Authorization</span></span>  | <span data-ttu-id="150a0-123">string</span><span class="sxs-lookup"><span data-stu-id="150a0-123">string</span></span>  | <span data-ttu-id="150a0-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="150a0-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="150a0-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="150a0-126">Content-Type</span></span> | <span data-ttu-id="150a0-127">string</span><span class="sxs-lookup"><span data-stu-id="150a0-127">string</span></span>  | <span data-ttu-id="150a0-p103">Die Art der Daten im Textkörper einer Entität. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="150a0-p103">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="150a0-130">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="150a0-130">Request body</span></span>
<span data-ttu-id="150a0-p104">Geben Sie im Anforderungstext den neuen Wert für **classifyAs** an. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="150a0-p104">In the request body, supply the new value for **classifyAs**. For best performance you shouldn't include existing values that are not changing.</span></span>

| <span data-ttu-id="150a0-133">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="150a0-133">Property</span></span>     | <span data-ttu-id="150a0-134">Typ</span><span class="sxs-lookup"><span data-stu-id="150a0-134">Type</span></span>   |<span data-ttu-id="150a0-135">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="150a0-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="150a0-136">classifyAs</span><span class="sxs-lookup"><span data-stu-id="150a0-136">classifyAs</span></span>|<span data-ttu-id="150a0-137">string</span><span class="sxs-lookup"><span data-stu-id="150a0-137">string</span></span>| <span data-ttu-id="150a0-p105">Gibt an, wie eingehende Nachrichten von einem bestimmten Absender immer klassifiziert werden sollen. Mögliche Werte: `focused`, `other`.</span><span class="sxs-lookup"><span data-stu-id="150a0-p105">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|

## <a name="response"></a><span data-ttu-id="150a0-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="150a0-140">Response</span></span>

<span data-ttu-id="150a0-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="150a0-141">If successful, this method returns a `200 OK` response code and updated [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="150a0-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="150a0-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="150a0-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="150a0-143">Request</span></span>
<span data-ttu-id="150a0-144">Im folgenden Beispiel wird die Außerkraftsetzung für die SMTP-Adresse „randiw@adatum.onmicrosoft.com“ von `other` zu `focused` geändert.</span><span class="sxs-lookup"><span data-stu-id="150a0-144">The following example changes the override for the SMTP address randiw@adatum.onmicrosoft.com from `other` to `focused`.</span></span>

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
##### <a name="response"></a><span data-ttu-id="150a0-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="150a0-145">Response</span></span>
<span data-ttu-id="150a0-p106">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="150a0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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