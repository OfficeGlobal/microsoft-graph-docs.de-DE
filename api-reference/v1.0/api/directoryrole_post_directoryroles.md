# <a name="activate-directoryrole"></a><span data-ttu-id="fc38a-101">directoryRole aktivieren</span><span class="sxs-lookup"><span data-stu-id="fc38a-101">Activate directoryRole</span></span>

<span data-ttu-id="fc38a-p101">Dient zum Aktivieren einer Verzeichnisrolle. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren und die impliziten Benutzerverzeichnisrollen sind standardmäßig aktiviert. Um auf Mitglieder zuzugreifen und diese einer anderen Verzeichnisrolle zuzuweisen, müssen Sie diese zuerst mit der entsprechenden Verzeichnisrollenvorlage aktivieren ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="fc38a-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc38a-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="fc38a-106">Permissions</span></span>
<span data-ttu-id="fc38a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="fc38a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fc38a-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="fc38a-109">Permission type</span></span>      | <span data-ttu-id="fc38a-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="fc38a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc38a-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="fc38a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc38a-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc38a-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc38a-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="fc38a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc38a-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="fc38a-114">Not supported.</span></span>    |
|<span data-ttu-id="fc38a-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="fc38a-115">Application</span></span> | <span data-ttu-id="fc38a-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc38a-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc38a-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc38a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="fc38a-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="fc38a-118">Request headers</span></span>
| <span data-ttu-id="fc38a-119">Name</span><span class="sxs-lookup"><span data-stu-id="fc38a-119">Name</span></span>       | <span data-ttu-id="fc38a-120">Typ</span><span class="sxs-lookup"><span data-stu-id="fc38a-120">Type</span></span> | <span data-ttu-id="fc38a-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc38a-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fc38a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc38a-122">Authorization</span></span>  | <span data-ttu-id="fc38a-123">string</span><span class="sxs-lookup"><span data-stu-id="fc38a-123">string</span></span>  | <span data-ttu-id="fc38a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="fc38a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fc38a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fc38a-126">Content-Type</span></span>  | <span data-ttu-id="fc38a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fc38a-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fc38a-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="fc38a-128">Request body</span></span>
<span data-ttu-id="fc38a-129">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="fc38a-129">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="fc38a-130">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Aktivieren einer Verzeichnisrolle erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="fc38a-130">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="fc38a-131">Erforderliche Parameter</span><span class="sxs-lookup"><span data-stu-id="fc38a-131">Required parameter</span></span> | <span data-ttu-id="fc38a-132">Typ</span><span class="sxs-lookup"><span data-stu-id="fc38a-132">Type</span></span> | <span data-ttu-id="fc38a-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="fc38a-133">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="fc38a-134">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="fc38a-134">roleTemplateId</span></span> | <span data-ttu-id="fc38a-135">string</span><span class="sxs-lookup"><span data-stu-id="fc38a-135">string</span></span> | <span data-ttu-id="fc38a-p104">Die ID der [directoryRoleTemplate](../resources/directoryroletemplate.md), auf der die Rolle basiert. Dies ist die einzige Eigenschaft, die in der Anforderung angegeben werden kann.</span><span class="sxs-lookup"><span data-stu-id="fc38a-p104">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="fc38a-138">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc38a-138">Response</span></span>

<span data-ttu-id="fc38a-139">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201, Created` und das [directoryRole](../resources/directoryrole.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc38a-139">If successful, this method returns `201, Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc38a-140">Beispiel</span><span class="sxs-lookup"><span data-stu-id="fc38a-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc38a-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="fc38a-141">Request</span></span>

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
<span data-ttu-id="fc38a-142">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="fc38a-142">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fc38a-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="fc38a-143">Response</span></span>
<span data-ttu-id="fc38a-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="fc38a-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
