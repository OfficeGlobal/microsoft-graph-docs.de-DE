# <a name="create-group"></a><span data-ttu-id="a5bb7-101">Gruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="a5bb7-101">Create group</span></span>

<span data-ttu-id="a5bb7-p101">Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:</span><span class="sxs-lookup"><span data-stu-id="a5bb7-p101">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="a5bb7-104">Office 365-Gruppe (einheitliche Gruppe)</span><span class="sxs-lookup"><span data-stu-id="a5bb7-104">Office 365 group (unified group)</span></span>
* <span data-ttu-id="a5bb7-105">Dynamische Gruppe</span><span class="sxs-lookup"><span data-stu-id="a5bb7-105">Dynamic group</span></span>
* <span data-ttu-id="a5bb7-106">Sicherheitsgruppe</span><span class="sxs-lookup"><span data-stu-id="a5bb7-106">Security group</span></span>

> <span data-ttu-id="a5bb7-p102">**Hinweis**: Microsoft Teams basiert zwar auf Office 365-Gruppen, über diese API kann derzeit aber kein Team erstellt werden. Sie können die anderen Gruppen-APIs verwenden, um ein Team zu verwalten, das in der Microsoft Teams-Benutzeroberfläche erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-p102">**Note**: Although Microsoft Teams is built on Office 365 groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5bb7-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="a5bb7-109">Permissions</span></span>
<span data-ttu-id="a5bb7-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a5bb7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a5bb7-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="a5bb7-112">Permission type</span></span>      | <span data-ttu-id="a5bb7-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="a5bb7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5bb7-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="a5bb7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a5bb7-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5bb7-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5bb7-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="a5bb7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5bb7-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="a5bb7-117">Not supported.</span></span>    |
|<span data-ttu-id="a5bb7-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="a5bb7-118">Application</span></span> | <span data-ttu-id="a5bb7-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5bb7-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5bb7-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5bb7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```
## <a name="request-headers"></a><span data-ttu-id="a5bb7-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="a5bb7-121">Request headers</span></span>
| <span data-ttu-id="a5bb7-122">Name</span><span class="sxs-lookup"><span data-stu-id="a5bb7-122">Name</span></span>       | <span data-ttu-id="a5bb7-123">Typ</span><span class="sxs-lookup"><span data-stu-id="a5bb7-123">Type</span></span> | <span data-ttu-id="a5bb7-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5bb7-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5bb7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5bb7-125">Authorization</span></span>  | <span data-ttu-id="a5bb7-126">string</span><span class="sxs-lookup"><span data-stu-id="a5bb7-126">string</span></span>  | <span data-ttu-id="a5bb7-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a5bb7-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="a5bb7-129">Request body</span></span>
<span data-ttu-id="a5bb7-130">Die folgende Tabelle zeigt die Eigenschaften der [Gruppe](../resources/group.md) Ressource, die Sie zumindest angeben müssen, wenn Sie eine Gruppe erstellen.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-130">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="a5bb7-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5bb7-131">Property</span></span> | <span data-ttu-id="a5bb7-132">Typ</span><span class="sxs-lookup"><span data-stu-id="a5bb7-132">Type</span></span> | <span data-ttu-id="a5bb7-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="a5bb7-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a5bb7-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a5bb7-134">displayName</span></span> | <span data-ttu-id="a5bb7-135">string</span><span class="sxs-lookup"><span data-stu-id="a5bb7-135">string</span></span> | <span data-ttu-id="a5bb7-136">Der Name der Gruppe, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-136">The name to display in the address book for the group.</span></span> |
| <span data-ttu-id="a5bb7-137">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="a5bb7-137">mailEnabled</span></span> | <span data-ttu-id="a5bb7-138">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a5bb7-138">boolean</span></span> | <span data-ttu-id="a5bb7-p105">**true** für E-Mail-aktivierte Gruppen. **true**, wenn eine Office 365-Gruppe erstellt wird. **false**, wenn dynamische oder Sicherheitsgruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-p105">Set to **true** for mail-enabled groups. Set this to **true** if creating an Office 365 group. Set this to **false** if creating dynamic or security group.</span></span>|
| <span data-ttu-id="a5bb7-142">mailNickname</span><span class="sxs-lookup"><span data-stu-id="a5bb7-142">mailNickname</span></span> | <span data-ttu-id="a5bb7-143">string</span><span class="sxs-lookup"><span data-stu-id="a5bb7-143">string</span></span> | <span data-ttu-id="a5bb7-144">Der E-Mail-Alias für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-144">The mail alias for the group.</span></span> |
| <span data-ttu-id="a5bb7-145">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="a5bb7-145">securityEnabled</span></span> | <span data-ttu-id="a5bb7-146">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="a5bb7-146">boolean</span></span> | <span data-ttu-id="a5bb7-p106">**true** für Gruppen mit aktivierter Sicherheit. **true**, wenn dynamische oder eine Sicherheitsgruppe erstellt wird. **false**, wenn eine Office 365-Gruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-p106">Set to **true** for security-enabled groups. Set this to **true** if creating a dynamic or security group. Set this to **false** if creating an Office 365 group.</span></span> |

<span data-ttu-id="a5bb7-150">Geben Sie die **groupTypes** Eigenschaft an, wenn Sie eine Office 365 oder eine dynamische Gruppe erstellen, wie unten beschrieben.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-150">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

| <span data-ttu-id="a5bb7-151">Art der Gruppe</span><span class="sxs-lookup"><span data-stu-id="a5bb7-151">Type of group</span></span> | <span data-ttu-id="a5bb7-152">**groupTypes**-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="a5bb7-152">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="a5bb7-153">Office 365 (auch einheitliche Gruppe genannt)</span><span class="sxs-lookup"><span data-stu-id="a5bb7-153">Office 365 (aka unified group)</span></span>| <span data-ttu-id="a5bb7-154">„Unified“</span><span class="sxs-lookup"><span data-stu-id="a5bb7-154">"Unified"</span></span> |
| <span data-ttu-id="a5bb7-155">Dynamisch</span><span class="sxs-lookup"><span data-stu-id="a5bb7-155">Dynamic</span></span> | <span data-ttu-id="a5bb7-156">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="a5bb7-156">"DynamicMembership"</span></span> |
| <span data-ttu-id="a5bb7-157">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="a5bb7-157">Security</span></span> | <span data-ttu-id="a5bb7-158">Nicht festlegen.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-158">Do not set.</span></span> |

<span data-ttu-id="a5bb7-p107">Geben Sie bei Bedarf andere beschreibbare Eigenschaften für Ihre Gruppe an. Weitere Informationen finden Sie in Themen zu Eigenschaften der [group](../resources/group.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-p107">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="a5bb7-161">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5bb7-161">Response</span></span>

<span data-ttu-id="a5bb7-162">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-162">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5bb7-163">Beispiel</span><span class="sxs-lookup"><span data-stu-id="a5bb7-163">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5bb7-164">Anforderung</span><span class="sxs-lookup"><span data-stu-id="a5bb7-164">Request</span></span>
<span data-ttu-id="a5bb7-165">Hier ist ein Beispiel für eine Anforderung, die eine Office 365-Gruppe erstellt.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-165">Here is an example of a request that creates an Office 365 group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group_from_groups"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

##### <a name="response"></a><span data-ttu-id="a5bb7-166">Antwort</span><span class="sxs-lookup"><span data-stu-id="a5bb7-166">Response</span></span>
<span data-ttu-id="a5bb7-p108">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden mehr Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="a5bb7-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. More properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
  "description": "Self help community for library",
  "displayName": "Library Assist",
  "groupTypes": [
    "Unified"
  ],
  "mail": "library@contoso.onmicrosoft.com",
  "mailEnabled": true,
  "mailNickname": "library",
  "securityEnabled": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create group",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
