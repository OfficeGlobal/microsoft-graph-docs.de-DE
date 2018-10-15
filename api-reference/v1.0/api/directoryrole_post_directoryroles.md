# <a name="activate-directoryrole"></a><span data-ttu-id="0e469-101">directoryRole aktivieren</span><span class="sxs-lookup"><span data-stu-id="0e469-101">Activate directoryRole</span></span>

<span data-ttu-id="0e469-p101">Dient zum Aktivieren einer Verzeichnisrolle. Um eine Verzeichnisrolle zu lesen oder ihre Mitglieder zu aktualisieren, muss diese zuerst im Mandanten aktiviert werden. Nur die Unternehmensadministratoren und die impliziten Benutzerverzeichnisrollen sind standardmäßig aktiviert. Um auf Mitglieder zuzugreifen und diese einer anderen Verzeichnisrolle zuzuweisen, müssen Sie diese zuerst mit der entsprechenden Verzeichnisrollenvorlage aktivieren ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span><span class="sxs-lookup"><span data-stu-id="0e469-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e469-106">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0e469-106">Permissions</span></span>
<span data-ttu-id="0e469-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0e469-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0e469-109">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0e469-109">Permission type</span></span>      | <span data-ttu-id="0e469-110">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0e469-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e469-111">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0e469-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0e469-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0e469-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0e469-113">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0e469-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e469-114">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0e469-114">Not supported.</span></span>    |
|<span data-ttu-id="0e469-115">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0e469-115">Application</span></span> | <span data-ttu-id="0e469-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e469-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e469-117">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e469-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="0e469-118">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0e469-118">Request headers</span></span>
| <span data-ttu-id="0e469-119">Name</span><span class="sxs-lookup"><span data-stu-id="0e469-119">Name</span></span>       | <span data-ttu-id="0e469-120">Typ</span><span class="sxs-lookup"><span data-stu-id="0e469-120">Type</span></span> | <span data-ttu-id="0e469-121">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e469-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0e469-122">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="0e469-122">Authorization</span></span>  | <span data-ttu-id="0e469-123">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e469-123">string</span></span>  | <span data-ttu-id="0e469-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e469-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e469-126">Inhaltstyp</span><span class="sxs-lookup"><span data-stu-id="0e469-126">Content-Type</span></span>  | <span data-ttu-id="0e469-127">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e469-127">string</span></span>  | <span data-ttu-id="0e469-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0e469-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e469-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0e469-129">Request body</span></span>
<span data-ttu-id="0e469-130">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0e469-130">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="0e469-131">In der folgenden Tabelle sind die Eigenschaften dargestellt, die zum Aktivieren einer Verzeichnisrolle erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="0e469-131">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="0e469-132">Parameter</span><span class="sxs-lookup"><span data-stu-id="0e469-132">Parameter</span></span> | <span data-ttu-id="0e469-133">Typ</span><span class="sxs-lookup"><span data-stu-id="0e469-133">Type</span></span> | <span data-ttu-id="0e469-134">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0e469-134">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="0e469-135">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="0e469-135">roleTemplateId</span></span> | <span data-ttu-id="0e469-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0e469-136">string</span></span> | <span data-ttu-id="0e469-137">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0e469-137">Required.</span></span> <span data-ttu-id="0e469-138">Die ID des [DirectoryRoleTemplate](../resources/directoryroletemplate.md), auf dem die Rolle basiert.</span><span class="sxs-lookup"><span data-stu-id="0e469-138">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span> <span data-ttu-id="0e469-139">Dies ist die einzige Eigenschaft, die in der Anforderung angegeben werden kann.</span><span class="sxs-lookup"><span data-stu-id="0e469-139">The ID of the directoryRoleTemplate that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="0e469-140">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e469-140">Response</span></span>

<span data-ttu-id="0e469-141">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [directoryRole](../resources/directoryrole.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e469-141">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e469-142">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0e469-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0e469-143">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0e469-143">Request</span></span>

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
<span data-ttu-id="0e469-144">Geben Sie im Anforderungstext eine JSON-Darstellung des [directoryRole](../resources/directoryrole.md)-Objekts an.</span><span class="sxs-lookup"><span data-stu-id="0e469-144">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0e469-145">Antwort</span><span class="sxs-lookup"><span data-stu-id="0e469-145">Response</span></span>
<span data-ttu-id="0e469-p105">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0e469-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
