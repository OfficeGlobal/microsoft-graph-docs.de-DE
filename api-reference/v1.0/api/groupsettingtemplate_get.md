# <a name="get-a-group-setting-template"></a><span data-ttu-id="ed249-101">Vorlage für Gruppeneinstellung abrufen</span><span class="sxs-lookup"><span data-stu-id="ed249-101">Get a group setting template</span></span>

<span data-ttu-id="ed249-p101">Eine Vorlage für Gruppeneinstellungen ist eine Vorlage mit Einstellungen, aus denen Einstellungen innerhalb eines Mandanten erstellt werden können. Dieser Vorgang ermöglicht das Abrufen der Eigenschaften des [groupSettingTemplate](../resources/groupsettingtemplate.md)-Objekts, einschließlich der verfügbaren Einstellungen und ihrer Standardwerte.</span><span class="sxs-lookup"><span data-stu-id="ed249-p101">A group setting template represents a template of settings from which settings may be created within a tenant. This operation allows retrieval of the properties of the [groupSettingTemplate](../resources/groupsettingtemplate.md) object, including the available settings and their defaults.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed249-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="ed249-104">Permissions</span></span>

<span data-ttu-id="ed249-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="ed249-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="ed249-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="ed249-107">Permission type</span></span>      | <span data-ttu-id="ed249-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="ed249-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="ed249-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="ed249-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ed249-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed249-110">One of the following scopes is required to execute this API: Directory.Read.All; Directory.ReadWrite.All; Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="ed249-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="ed249-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed249-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="ed249-112">Not supported.</span></span>    | 
|<span data-ttu-id="ed249-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="ed249-113">Application</span></span> | <span data-ttu-id="ed249-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed249-114">Directory.Read.All, Directory.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="ed249-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed249-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ed249-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="ed249-116">Optional query parameters</span></span>
<span data-ttu-id="ed249-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="ed249-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed249-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="ed249-118">Request headers</span></span>
| <span data-ttu-id="ed249-119">Name</span><span class="sxs-lookup"><span data-stu-id="ed249-119">Name</span></span> | <span data-ttu-id="ed249-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="ed249-120">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="ed249-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed249-121">Authorization</span></span> | <span data-ttu-id="ed249-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="ed249-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed249-124">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="ed249-124">Request body</span></span>
<span data-ttu-id="ed249-125">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="ed249-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed249-126">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed249-126">Response</span></span>

<span data-ttu-id="ed249-127">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [groupSettingTemplate](../resources/groupsettingtemplate.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed249-127">If successful, this method returns a `200 OK` response code and [groupSettingTemplate](../resources/groupsettingtemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed249-128">Beispiel</span><span class="sxs-lookup"><span data-stu-id="ed249-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed249-129">Anforderung</span><span class="sxs-lookup"><span data-stu-id="ed249-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplate"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates/{id}
```
##### <a name="response"></a><span data-ttu-id="ed249-130">Antwort</span><span class="sxs-lookup"><span data-stu-id="ed249-130">Response</span></span>

<span data-ttu-id="ed249-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="ed249-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1341

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates/$entity",
    "id": "62375ab9-6b52-47ed-826b-58e47e0e304b",
    "deletedDateTime": null,
    "displayName": "Group.Unified",
    "description": "Setting templates define the different settings that can be used for the associated ObjectSettings. This template defines settings that can be used for Unified Groups.",
    "values": [
        {
            "name": "CustomBlockedWordsList",
            "type": "System.String",
            "defaultValue": "",
            "description": "A comma-delimited list of blocked words for Unified Group displayName and mailNickName."
        },
        {
            "name": "EnableMSStandardBlockedWords",
            "type": "System.Boolean",
            "defaultValue": "false",
            "description": "A flag indicating whether or not to enable the Microsoft Standard list of blocked words for Unified Group displayName and mailNickName."
        },
        {
            "name": "ClassificationDescriptions",
            "type": "System.String",
            "defaultValue": "",
            "description": "A comma-delimited list of structured strings describing the classification values in the ClassificationList. The structure of the string is: Value: Description"
        }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSettingTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->