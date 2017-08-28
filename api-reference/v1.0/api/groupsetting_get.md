# <a name="get-a-group-setting"></a><span data-ttu-id="55e12-101">Abrufen einer Gruppeneinstellung</span><span class="sxs-lookup"><span data-stu-id="55e12-101">Get a group setting</span></span>

<span data-ttu-id="55e12-102">Mit dieser API können Sie die Eigenschaften eines bestimmten Gruppeneinstellungsobjekts abrufen.</span><span class="sxs-lookup"><span data-stu-id="55e12-102">Retrieve the properties of a specific of group setting object.</span></span>

## <a name="permissions"></a><span data-ttu-id="55e12-103">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="55e12-103">Permissions</span></span>

<span data-ttu-id="55e12-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="55e12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="55e12-106">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="55e12-106">Permission type</span></span>      | <span data-ttu-id="55e12-107">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="55e12-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55e12-108">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="55e12-108">Delegated (work or school account)</span></span> | <span data-ttu-id="55e12-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="55e12-109">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="55e12-110">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="55e12-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55e12-111">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="55e12-111">Not supported.</span></span>    |
|<span data-ttu-id="55e12-112">Anwendung</span><span class="sxs-lookup"><span data-stu-id="55e12-112">Application</span></span> | <span data-ttu-id="55e12-113">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55e12-113">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="55e12-114">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="55e12-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

<span data-ttu-id="55e12-115">Rufen Sie eine bestimmte Mandanten-übergreifende oder Gruppeneinstellung ab.</span><span class="sxs-lookup"><span data-stu-id="55e12-115">Get a specific tenant-wide or group setting.</span></span>

```http
GET /groupSettings/{id}
GET /groups/{id}/settings/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="55e12-116">Optionale Abfrageparameter</span><span class="sxs-lookup"><span data-stu-id="55e12-116">Optional query parameters</span></span>
<span data-ttu-id="55e12-117">Diese Methode unterstützt die [OData-Abfrageparameter](http://graph.microsoft.io/docs/overview/query_parameters) zur Anpassung der Antwort.</span><span class="sxs-lookup"><span data-stu-id="55e12-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

> <span data-ttu-id="55e12-118">Hinweis: $filter wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="55e12-118">Note: $filter is not supported.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55e12-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="55e12-119">Request headers</span></span>
| <span data-ttu-id="55e12-120">Name</span><span class="sxs-lookup"><span data-stu-id="55e12-120">Name</span></span> | <span data-ttu-id="55e12-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="55e12-121">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="55e12-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="55e12-122">Authorization</span></span> | <span data-ttu-id="55e12-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="55e12-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55e12-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="55e12-125">Request body</span></span>

<span data-ttu-id="55e12-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="55e12-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55e12-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="55e12-127">Response</span></span>

<span data-ttu-id="55e12-128">Wenn erfolgreich ausgeführt, gibt diese Methode den Antwortcode `200 OK` und das [groupSetting](../resources/groupsetting.md)-Objekt im Antworttext zurück.</span><span class="sxs-lookup"><span data-stu-id="55e12-128">If successful, this method returns a `200 OK` response code and [groupSetting](../resources/groupsetting.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55e12-129">Beispiel</span><span class="sxs-lookup"><span data-stu-id="55e12-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55e12-130">Anforderung</span><span class="sxs-lookup"><span data-stu-id="55e12-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_groupsetting"
}-->

```http
GET https://graph.microsoft.com/v1.0/groupSettings/{id}
```
##### <a name="response"></a><span data-ttu-id="55e12-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="55e12-131">Response</span></span>

<span data-ttu-id="55e12-p103">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="55e12-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupSetting"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 194

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get groupSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->