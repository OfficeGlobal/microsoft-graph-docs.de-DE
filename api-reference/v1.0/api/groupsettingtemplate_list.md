# <a name="list-groupsettingtemplates"></a><span data-ttu-id="21e6c-101">List groupSettingTemplates</span><span class="sxs-lookup"><span data-stu-id="21e6c-101">List groupSettingTemplates</span></span>

<span data-ttu-id="21e6c-p101">Gruppeneinstellungsvorlagen stellen einen Satz von Vorlagen dar, aus dem Gruppeneinstellungen erstellt und in einem Mandanten verwendet werden können.  Dieser Vorgang ruft die Liste der verfügbaren groupSettingTemplates-Objekte ab.</span><span class="sxs-lookup"><span data-stu-id="21e6c-p101">Group setting templates represents a set of templates  from which group settings may be created and used within a tenant.  This operation retrieves the list of available groupSettingTemplates objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="21e6c-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="21e6c-104">Permissions</span></span>

<span data-ttu-id="21e6c-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="21e6c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="21e6c-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="21e6c-107">Permission type</span></span>      | <span data-ttu-id="21e6c-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="21e6c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21e6c-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="21e6c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="21e6c-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="21e6c-110">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="21e6c-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="21e6c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21e6c-112">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="21e6c-112">Not supported.</span></span>    |
|<span data-ttu-id="21e6c-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="21e6c-113">Application</span></span> | <span data-ttu-id="21e6c-114">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21e6c-114">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="21e6c-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="21e6c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groupSettingTemplates
```
## <a name="optional-query-parameters"></a><span data-ttu-id="21e6c-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="21e6c-116">Optional query parameters</span></span>
<span data-ttu-id="21e6c-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="21e6c-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="21e6c-118">**Hinweis:** $filter wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="21e6c-118">**Note:** $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21e6c-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="21e6c-119">Request headers</span></span>
| <span data-ttu-id="21e6c-120">Name</span><span class="sxs-lookup"><span data-stu-id="21e6c-120">Name</span></span> | <span data-ttu-id="21e6c-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="21e6c-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="21e6c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="21e6c-122">Authorization</span></span>  | <span data-ttu-id="21e6c-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="21e6c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="21e6c-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="21e6c-125">Request body</span></span>
<span data-ttu-id="21e6c-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="21e6c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21e6c-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="21e6c-127">Response</span></span>

<span data-ttu-id="21e6c-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [groupSettingTemplate](../resources/groupsettingtemplate.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21e6c-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/groupsettingtemplate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21e6c-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="21e6c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="21e6c-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="21e6c-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsettingtemplates"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettingTemplates
```
##### <a name="response"></a><span data-ttu-id="21e6c-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="21e6c-131">Response</span></span>

<span data-ttu-id="21e6c-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="21e6c-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1770

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groupSettingTemplates",
    "value": [
                {
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
            ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettingTemplates",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->