# <a name="list-group-settings"></a><span data-ttu-id="7428b-101">Gruppeneinstellungen auflisten</span><span class="sxs-lookup"><span data-stu-id="7428b-101">List group settings</span></span>

<span data-ttu-id="7428b-102">Mit dieser API können Sie eine Liste von Gruppeneinstellungsobjekten abrufen.</span><span class="sxs-lookup"><span data-stu-id="7428b-102">Retrieve a list of group setting objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7428b-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7428b-103">Permissions</span></span>

<span data-ttu-id="7428b-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7428b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="7428b-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7428b-106">Permission type</span></span>      | <span data-ttu-id="7428b-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7428b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7428b-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7428b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="7428b-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7428b-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7428b-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7428b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7428b-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7428b-111">Not supported.</span></span>    |
|<span data-ttu-id="7428b-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7428b-112">Application</span></span> | <span data-ttu-id="7428b-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7428b-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7428b-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7428b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="7428b-115">Listet mandantenweite oder Gruppeneinstellungen auf.</span><span class="sxs-lookup"><span data-stu-id="7428b-115">List tenant-wide or group settings.</span></span>

```http
GET /groupSettings
GET group/{id}/settings
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7428b-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="7428b-116">Optional query parameters</span></span>
<span data-ttu-id="7428b-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="7428b-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="7428b-118">Hinweis: $filter wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="7428b-118">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7428b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7428b-119">Request headers</span></span>
| <span data-ttu-id="7428b-120">Name</span><span class="sxs-lookup"><span data-stu-id="7428b-120">Name</span></span> | <span data-ttu-id="7428b-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="7428b-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="7428b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7428b-122">Authorization</span></span>  | <span data-ttu-id="7428b-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7428b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7428b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7428b-125">Request body</span></span>
<span data-ttu-id="7428b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7428b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7428b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7428b-127">Response</span></span>

<span data-ttu-id="7428b-128">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und eine Sammlung von [groupSetting](../resources/groupsetting.md)-Objekten im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7428b-128">If successful, this method returns a `200 OK` response code and collection of [groupSetting](../resources/groupsetting.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7428b-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7428b-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7428b-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7428b-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_groupsettings"
}-->
```http
GET https://graph.microsoft.com/v1.0/groupSettings
```
##### <a name="response"></a><span data-ttu-id="7428b-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="7428b-131">Response</span></span>

<span data-ttu-id="7428b-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="7428b-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "displayName": "displayName-value",
      "templateId": "templateId-value",
      "values": [
        {
          "name": "name-value",
          "value": "value-value"
        }
      ],
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->