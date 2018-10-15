# <a name="update-educationclass-properties"></a><span data-ttu-id="b8455-101">Educationclass-Eigenschaften aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b8455-101">Update educationclass properties</span></span>

<span data-ttu-id="b8455-102">Dient zum Aktualisieren der Eigenschaften einer Klasse.</span><span class="sxs-lookup"><span data-stu-id="b8455-102">Update the properties of a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8455-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="b8455-103">Permissions</span></span>
<span data-ttu-id="b8455-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="b8455-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b8455-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="b8455-106">Permission type</span></span>      | <span data-ttu-id="b8455-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="b8455-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8455-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="b8455-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="b8455-109">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8455-109">Not supported.</span></span>  |
|<span data-ttu-id="b8455-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="b8455-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8455-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="b8455-111">Not supported.</span></span>   |
|<span data-ttu-id="b8455-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="b8455-112">Application</span></span> | <span data-ttu-id="b8455-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8455-113">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b8455-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8455-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b8455-115">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="b8455-115">Request headers</span></span>
| <span data-ttu-id="b8455-116">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="b8455-116">Header</span></span>       | <span data-ttu-id="b8455-117">Wert</span><span class="sxs-lookup"><span data-stu-id="b8455-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8455-118">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="b8455-118">Authorization</span></span>  | <span data-ttu-id="b8455-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="b8455-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b8455-121">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="b8455-121">Content-Type</span></span>  | <span data-ttu-id="b8455-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b8455-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8455-123">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="b8455-123">Request body</span></span>
<span data-ttu-id="b8455-124">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="b8455-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b8455-125">Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet.</span><span class="sxs-lookup"><span data-stu-id="b8455-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b8455-126">Geben Sie aus Gründen der Leistung vorhandene Werte, die nicht geändert wurden, nicht an.</span><span class="sxs-lookup"><span data-stu-id="b8455-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b8455-127">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="b8455-127">Property</span></span>     | <span data-ttu-id="b8455-128">Typ</span><span class="sxs-lookup"><span data-stu-id="b8455-128">Type</span></span>   |<span data-ttu-id="b8455-129">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8455-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8455-130">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="b8455-130">description</span></span>|<span data-ttu-id="b8455-131">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8455-131">String</span></span>| <span data-ttu-id="b8455-132">Beschreibung der Klasse</span><span class="sxs-lookup"><span data-stu-id="b8455-132">Description of the class.</span></span>|
|<span data-ttu-id="b8455-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b8455-133">displayName</span></span>|<span data-ttu-id="b8455-134">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8455-134">String</span></span>| <span data-ttu-id="b8455-135">Der Name der Klasse</span><span class="sxs-lookup"><span data-stu-id="b8455-135">Name of the class.</span></span>|
|<span data-ttu-id="b8455-136">mailNickname</span><span class="sxs-lookup"><span data-stu-id="b8455-136">mailNickname</span></span>|<span data-ttu-id="b8455-137">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="b8455-137">String</span></span>| <span data-ttu-id="b8455-138">E-Mail-Alias zum Senden von E-Mails an alle Benutzer, wenn diese Funktion aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="b8455-138">Email alias for sending email to all users if that feature is enabled.</span></span> |
<span data-ttu-id="b8455-139"><!-- Please verify the revised description here. --> |classCode|String| Von der Schule verwendeter Klassencode. | |externalId|String| Die ID der Klasse aus dem Synchronisierungssystem.</span><span class="sxs-lookup"><span data-stu-id="b8455-139"><!-- Please verify the revised description here. -->|classCode|String| Class code used by the school.| |externalId|String| ID of the class from the syncing system.</span></span> <span data-ttu-id="b8455-140">| |externalName|String| Name der Klasse im Synchronisierungssystem.| |externalSource|String| Wie diese Klasse erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="b8455-140">| |externalName|String|Name of the class in the syncing system.| |externalSource|string| How this class was created.</span></span> <span data-ttu-id="b8455-141">Die möglichen Werte sind: `sis`, `manual`, `enum_sentinel`.</span><span class="sxs-lookup"><span data-stu-id="b8455-141">The possible values are , , , , , , , , , , , or .</span></span>

## <a name="response"></a><span data-ttu-id="b8455-142">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8455-142">Response</span></span>
<span data-ttu-id="b8455-143">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und ein aktualisiertes [educationClass](../resources/educationclass.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="b8455-143">If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b8455-144">Beispiel</span><span class="sxs-lookup"><span data-stu-id="b8455-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b8455-145">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b8455-145">Request</span></span>
<span data-ttu-id="b8455-146">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="b8455-146">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/classes/{class-id}
Content-type: application/json
Content-length: 224

{
  "description": "History - World History 1",
  "displayName": "World History Level 1",
}
```
##### <a name="response"></a><span data-ttu-id="b8455-147">Antwort</span><span class="sxs-lookup"><span data-stu-id="b8455-147">Response</span></span>
<span data-ttu-id="b8455-148">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="b8455-148">The following is an example of the response.</span></span> 

><span data-ttu-id="b8455-p105">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="b8455-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 224

{
  "id": "11014",
  "description": "World History Level 1",
  "classCode": "301",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
  "displayName": "History - World History 1",
  "externalId": "301",
  "externalName": "World History Level 1",
  "externalSource": "Fabrikam High School",
  "mailNickname": "Fabrikam"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationclass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->