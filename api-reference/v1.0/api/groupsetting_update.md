# <a name="update-a-group-setting"></a><span data-ttu-id="ed71f-101">Aktualisieren einer Gruppeneinstellung</span><span class="sxs-lookup"><span data-stu-id="ed71f-101">Update a group setting</span></span>

<span data-ttu-id="ed71f-102">Mit dieser API können Sie die Eigenschaften des jeweils angegebenen Gruppeneinstellungsobjekts aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="ed71f-102">Update the properties of a specific group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed71f-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ed71f-103">Permissions</span></span>

<span data-ttu-id="ed71f-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ed71f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="ed71f-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed71f-106">Permission type</span></span>      | <span data-ttu-id="ed71f-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed71f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed71f-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed71f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ed71f-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed71f-109">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ed71f-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed71f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed71f-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed71f-111">Not supported.</span></span>    |
|<span data-ttu-id="ed71f-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed71f-112">Application</span></span> | <span data-ttu-id="ed71f-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed71f-113">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed71f-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed71f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="ed71f-115">Aktualisiert eine mandantenweite oder gruppenspezifische Einstellung.</span><span class="sxs-lookup"><span data-stu-id="ed71f-115">Update a tenant-wide or group specific setting.</span></span>

```http
PATCH /groupSettings/{id}
PATCH /groups/{id}/settings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ed71f-116">Optionale Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed71f-116">Optional request headers</span></span>
| <span data-ttu-id="ed71f-117">Name</span><span class="sxs-lookup"><span data-stu-id="ed71f-117">Name</span></span> | <span data-ttu-id="ed71f-118">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed71f-118">Description</span></span> |
|:-----------|:-----------|
| <span data-ttu-id="ed71f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed71f-119">Authorization</span></span>  | <span data-ttu-id="ed71f-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ed71f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed71f-122">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ed71f-122">Content-Type</span></span>  | <span data-ttu-id="ed71f-123">application/json</span><span class="sxs-lookup"><span data-stu-id="ed71f-123">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ed71f-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed71f-124">Request body</span></span>
<span data-ttu-id="ed71f-125">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen.</span><span class="sxs-lookup"><span data-stu-id="ed71f-125">In the request body, supply the values for relevant fields that should be updated.</span></span> 

| <span data-ttu-id="ed71f-126">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="ed71f-126">Property</span></span> | <span data-ttu-id="ed71f-127">Typ</span><span class="sxs-lookup"><span data-stu-id="ed71f-127">Type</span></span> | <span data-ttu-id="ed71f-128">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed71f-128">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="ed71f-129">values</span><span class="sxs-lookup"><span data-stu-id="ed71f-129">values</span></span> | <span data-ttu-id="ed71f-130">settingValue</span><span class="sxs-lookup"><span data-stu-id="ed71f-130">settingValue</span></span> | <span data-ttu-id="ed71f-p103">Der aktualisierten Satz von Werten.  HINWEIS: Sie müssen den gesamten Sammlungssatz angeben. Sie können keinen einzelnen Wertesatz aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="ed71f-p103">The updated set of values.  NOTE: You must supply the entire collection set. You cannot update a single set of values.</span></span> |

## <a name="response"></a><span data-ttu-id="ed71f-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed71f-134">Response</span></span>

<span data-ttu-id="ed71f-135">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `204 OK` und ein aktualisiertes [groupSetting](../resources/groupsetting.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="ed71f-135">If successful, this method returns a `204 OK` response code and updated [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed71f-136">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed71f-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed71f-137">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed71f-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_groupsetting"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/groupSettings/{id}
Content-type: application/json
Content-length: 173

{
  "displayName": "displayName-value",
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
##### <a name="response"></a><span data-ttu-id="ed71f-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed71f-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 204 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->