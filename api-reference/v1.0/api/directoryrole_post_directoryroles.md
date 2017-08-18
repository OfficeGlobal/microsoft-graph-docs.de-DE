# <a name="activate-directoryrole"></a><span data-ttu-id="041b1-101">directoryRole aktivieren</span><span class="sxs-lookup"><span data-stu-id="041b1-101">Activate directoryRole</span></span>

<span data-ttu-id="041b1-p101">Dient zum Aktivieren einer Verzeichnisrolle. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren und die impliziten Benutzerverzeichnisrollen sind standardmäßig aktiviert. Um auf Mitglieder zuzugreifen und diese einer anderen Verzeichnisrolle zuzuweisen, müssen Sie diese zuerst mit der entsprechenden Verzeichnisrollenvorlage aktivieren ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="041b1-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="041b1-106">Anforderungen</span><span class="sxs-lookup"><span data-stu-id="041b1-106">Prerequisites</span></span>
<span data-ttu-id="041b1-107">Einer der folgenden **Bereiche** ist erforderlich, um diese API auszuführen: *Directory.ReadWrite.All* oder *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="041b1-107">One of the following **scopes** is required to execute this API: *Directory.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>
## <a name="http-request"></a><span data-ttu-id="041b1-108">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="041b1-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="041b1-109">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="041b1-109">Request headers</span></span>
| <span data-ttu-id="041b1-110">Name</span><span class="sxs-lookup"><span data-stu-id="041b1-110">Name</span></span>       | <span data-ttu-id="041b1-111">Typ</span><span class="sxs-lookup"><span data-stu-id="041b1-111">Type</span></span> | <span data-ttu-id="041b1-112">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="041b1-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="041b1-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="041b1-113">Authorization</span></span>  | <span data-ttu-id="041b1-114">string</span><span class="sxs-lookup"><span data-stu-id="041b1-114">string</span></span>  | <span data-ttu-id="041b1-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="041b1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="041b1-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="041b1-117">Content-Type</span></span>  | <span data-ttu-id="041b1-118">application/json</span><span class="sxs-lookup"><span data-stu-id="041b1-118">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="041b1-119">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="041b1-119">Request body</span></span>
<span data-ttu-id="041b1-120">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="041b1-120">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="041b1-121">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Aktivieren einer Verzeichnisrolle erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="041b1-121">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="041b1-122">Erforderliche Parameter</span><span class="sxs-lookup"><span data-stu-id="041b1-122">Required parameter</span></span> | <span data-ttu-id="041b1-123">Typ</span><span class="sxs-lookup"><span data-stu-id="041b1-123">Type</span></span> | <span data-ttu-id="041b1-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="041b1-124">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="041b1-125">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="041b1-125">roleTemplateId</span></span> | <span data-ttu-id="041b1-126">string</span><span class="sxs-lookup"><span data-stu-id="041b1-126">string</span></span> | <span data-ttu-id="041b1-p103">Die ID der [directoryRoleTemplate](../resources/directoryroletemplate.md), auf der die Rolle basiert. Dies ist die einzige Eigenschaft, die in der Anforderung angegeben werden kann.</span><span class="sxs-lookup"><span data-stu-id="041b1-p103">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="041b1-129">Antwort</span><span class="sxs-lookup"><span data-stu-id="041b1-129">Response</span></span>

<span data-ttu-id="041b1-130">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [directoryRole](../resources/directoryrole.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="041b1-130">If successful, this method returns `201, Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="041b1-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="041b1-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="041b1-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="041b1-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "roleTemplateId-value"
}
```
<span data-ttu-id="041b1-133">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="041b1-133">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="041b1-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="041b1-134">Response</span></span>
<span data-ttu-id="041b1-p104">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="041b1-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
