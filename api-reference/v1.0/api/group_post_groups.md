# <a name="create-group"></a><span data-ttu-id="10f73-101">Gruppe erstellen</span><span class="sxs-lookup"><span data-stu-id="10f73-101">Create group</span></span>
<span data-ttu-id="10f73-p101">Verwenden Sie diese API zum Erstellen einer neuen Gruppe gemäß der Angabe im Anforderungstext. Sie können drei Typen von Gruppen erstellen:</span><span class="sxs-lookup"><span data-stu-id="10f73-p101">Use this API to create a new group as specified in the request body. You can create one of three types of groups:</span></span>

* <span data-ttu-id="10f73-104">Office 365-Gruppe (einheitliche Gruppe)</span><span class="sxs-lookup"><span data-stu-id="10f73-104">Office 365 Group (unified group)</span></span>
* <span data-ttu-id="10f73-105">Dynamische Gruppe</span><span class="sxs-lookup"><span data-stu-id="10f73-105">Dynamic group</span></span>
* <span data-ttu-id="10f73-106">Sicherheitsgruppe</span><span class="sxs-lookup"><span data-stu-id="10f73-106">Security group</span></span>

> <span data-ttu-id="10f73-p102">**Hinweis**: Microsoft Teams basiert zwar auf Office 365-Gruppen, über diese API kann derzeit aber kein Team erstellt werden. Sie können die anderen Gruppen-APIs verwenden, um ein Team zu verwalten, das in der Microsoft Teams-Benutzeroberfläche erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="10f73-p102">**Note**: Although Microsoft Teams is built on Office 365 Groups, you can't currently create a team via this API. You can use the other group APIs to manage a team that has been created in the Microsoft Teams UI.</span></span>

## <a name="permissions"></a><span data-ttu-id="10f73-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="10f73-109">Permissions</span></span>
<span data-ttu-id="10f73-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="10f73-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="10f73-112">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="10f73-112">Permission type</span></span>      | <span data-ttu-id="10f73-113">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="10f73-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10f73-114">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="10f73-114">Delegated (work or school account)</span></span> | <span data-ttu-id="10f73-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10f73-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="10f73-116">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="10f73-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10f73-117">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="10f73-117">Not supported.</span></span>    |
|<span data-ttu-id="10f73-118">Anwendung</span><span class="sxs-lookup"><span data-stu-id="10f73-118">Application</span></span> | <span data-ttu-id="10f73-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10f73-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="10f73-120">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="10f73-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups
```

## <a name="request-headers"></a><span data-ttu-id="10f73-121">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="10f73-121">Request headers</span></span>
| <span data-ttu-id="10f73-122">Name</span><span class="sxs-lookup"><span data-stu-id="10f73-122">Name</span></span>       | <span data-ttu-id="10f73-123">Typ</span><span class="sxs-lookup"><span data-stu-id="10f73-123">Type</span></span> | <span data-ttu-id="10f73-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10f73-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="10f73-125">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="10f73-125">Authorization</span></span>  | <span data-ttu-id="10f73-126">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10f73-126">string</span></span>  | <span data-ttu-id="10f73-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10f73-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10f73-129">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="10f73-129">Request body</span></span>
<span data-ttu-id="10f73-130">Die folgende Tabelle zeigt die Eigenschaften der [Gruppen](../resources/group.md)-Ressource, die Sie angeben müssen, wenn Sie eine Gruppe erstellen.</span><span class="sxs-lookup"><span data-stu-id="10f73-130">The following table shows the properties of the [group](../resources/group.md) resource that you must specify at a minimum when you create a group.</span></span> 

| <span data-ttu-id="10f73-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10f73-131">Property</span></span> | <span data-ttu-id="10f73-132">Typ</span><span class="sxs-lookup"><span data-stu-id="10f73-132">Type</span></span> | <span data-ttu-id="10f73-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="10f73-133">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="10f73-134">displayName</span><span class="sxs-lookup"><span data-stu-id="10f73-134">displayName</span></span> | <span data-ttu-id="10f73-135">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10f73-135">string</span></span> | <span data-ttu-id="10f73-136">Der Name der Gruppe, der im Adressbuch angezeigt wird.</span><span class="sxs-lookup"><span data-stu-id="10f73-136">The name to display in the address book for the group.</span></span> <span data-ttu-id="10f73-137">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10f73-137">Required.</span></span> |
| <span data-ttu-id="10f73-138">mailEnabled</span><span class="sxs-lookup"><span data-stu-id="10f73-138">mailEnabled</span></span> | <span data-ttu-id="10f73-139">boolesch</span><span class="sxs-lookup"><span data-stu-id="10f73-139">boolean</span></span> | <span data-ttu-id="10f73-140">**true** für E-Mail-aktivierte Gruppen.</span><span class="sxs-lookup"><span data-stu-id="10f73-140">Set to **true** for mail-enabled groups.</span></span> <span data-ttu-id="10f73-141">Legen Sie dies auf **true** fest, wenn Sie eine Office 365-Gruppe erstellen.</span><span class="sxs-lookup"><span data-stu-id="10f73-141">Set this to **true** if creating an Office 365 Group.</span></span> <span data-ttu-id="10f73-142">Legen Sie dies auf **false** fest, wenn Sie eine dynamische oder eine Sicherheitsgruppe erstellen.</span><span class="sxs-lookup"><span data-stu-id="10f73-142">Set this to **false** if creating dynamic or security group.</span></span> <span data-ttu-id="10f73-143">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10f73-143">Required.</span></span> |
| <span data-ttu-id="10f73-144">mailNickname</span><span class="sxs-lookup"><span data-stu-id="10f73-144">mailNickname</span></span> | <span data-ttu-id="10f73-145">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="10f73-145">string</span></span> | <span data-ttu-id="10f73-146">Der E-Mail-Alias für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="10f73-146">The mail alias for the group.</span></span> <span data-ttu-id="10f73-147">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10f73-147">Required.</span></span> |
| <span data-ttu-id="10f73-148">securityEnabled</span><span class="sxs-lookup"><span data-stu-id="10f73-148">securityEnabled</span></span> | <span data-ttu-id="10f73-149">boolesch</span><span class="sxs-lookup"><span data-stu-id="10f73-149">boolean</span></span> | <span data-ttu-id="10f73-150">Legen Sie dies für Sicherheits-aktivierte Gruppen auf **true** fest.</span><span class="sxs-lookup"><span data-stu-id="10f73-150">Set to **true** for security-enabled groups.</span></span> <span data-ttu-id="10f73-151">Legen Sie dies auf **true** fest, wenn Sie eine dynamische oder eine Sicherheitsgruppe erstellen.</span><span class="sxs-lookup"><span data-stu-id="10f73-151">Set this to **true** if creating a dynamic or security group.</span></span> <span data-ttu-id="10f73-152">Legen Sie dies auf **false** fest, wenn Sie eine Office 365-Gruppe erstellen.</span><span class="sxs-lookup"><span data-stu-id="10f73-152">Set this to **false** if creating an Office 365 group.</span></span> <span data-ttu-id="10f73-153">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="10f73-153">Required.</span></span> |
| <span data-ttu-id="10f73-154">Besitzer</span><span class="sxs-lookup"><span data-stu-id="10f73-154">owners</span></span> | <span data-ttu-id="10f73-155">Zeichenfolgen-Sammlung</span><span class="sxs-lookup"><span data-stu-id="10f73-155">string collection</span></span> | <span data-ttu-id="10f73-156">Diese Eigenschaft stellt die Besitzer für die Gruppe zum Zeitpunkt der Erstellung dar.</span><span class="sxs-lookup"><span data-stu-id="10f73-156">This property represents the owners for the group at creation time.</span></span> <span data-ttu-id="10f73-157">Optional.</span><span class="sxs-lookup"><span data-stu-id="10f73-157">Optional.</span></span> |
| <span data-ttu-id="10f73-158">Elemente</span><span class="sxs-lookup"><span data-stu-id="10f73-158">members</span></span> | <span data-ttu-id="10f73-159">Zeichenfolgen-Sammlung</span><span class="sxs-lookup"><span data-stu-id="10f73-159">string collection</span></span> | <span data-ttu-id="10f73-160">Diese Eigenschaft stellt die Mitglieder der Gruppe zum Zeitpunkt der Erstellung.</span><span class="sxs-lookup"><span data-stu-id="10f73-160">This property represents the members for the group at creation time.</span></span> <span data-ttu-id="10f73-161">Optional.</span><span class="sxs-lookup"><span data-stu-id="10f73-161">Optional.</span></span> |


<span data-ttu-id="10f73-162">Geben Sie die **groupTypes** Eigenschaft an, wenn Sie eine Office 365 oder eine dynamische Gruppe erstellen, wie unten beschrieben.</span><span class="sxs-lookup"><span data-stu-id="10f73-162">Specify the **groupTypes** property if you're creating an Office 365 or dynamic group, as stated below.</span></span>

### <a name="grouptypes-options"></a><span data-ttu-id="10f73-163">GroupTypes-Optionen</span><span class="sxs-lookup"><span data-stu-id="10f73-163">groupTypes options</span></span>

| <span data-ttu-id="10f73-164">Art der Gruppe</span><span class="sxs-lookup"><span data-stu-id="10f73-164">Type of group</span></span> | <span data-ttu-id="10f73-165">**groupTypes**-Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="10f73-165">**groupTypes** property</span></span> |
|:--------------|:------------------------|
| <span data-ttu-id="10f73-166">Office 365 (auch einheitliche Gruppe genannt)</span><span class="sxs-lookup"><span data-stu-id="10f73-166">Office 365 (aka unified group)</span></span>| <span data-ttu-id="10f73-167">„Unified“</span><span class="sxs-lookup"><span data-stu-id="10f73-167">"Unified"</span></span> |
| <span data-ttu-id="10f73-168">Dynamisch</span><span class="sxs-lookup"><span data-stu-id="10f73-168">Dynamic</span></span> | <span data-ttu-id="10f73-169">"DynamicMembership"</span><span class="sxs-lookup"><span data-stu-id="10f73-169">"DynamicMembership"</span></span> |
| <span data-ttu-id="10f73-170">Sicherheit</span><span class="sxs-lookup"><span data-stu-id="10f73-170">Security</span></span> | <span data-ttu-id="10f73-171">Nicht festlegen.</span><span class="sxs-lookup"><span data-stu-id="10f73-171">Do not set.</span></span> |


><span data-ttu-id="10f73-172">**Hinweis:** Das programmgesteuerte Erstellen einer Office 365-Gruppe ohne einen Benutzerkontext und ohne Angabe von Besitzer erstellt die Gruppe anonym.</span><span class="sxs-lookup"><span data-stu-id="10f73-172">**Note:** Creating an Office 365 Group programmatically without a user context and  without specifying owners will create the group anonymously.</span></span>  <span data-ttu-id="10f73-173">Dies kann dazu führen, dass die zugehörige SharePoint Online-Website nicht automatisch erstellt wird, bis eine zusätzliche manuelle Aktion ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="10f73-173">Doing so can result in the associated SharePoint Online site not being created automatically until further manual action is taken.</span></span>  

<span data-ttu-id="10f73-p112">Geben Sie bei Bedarf andere beschreibbare Eigenschaften für Ihre Gruppe an. Weitere Informationen finden Sie in Themen zu Eigenschaften der [group](../resources/group.md)-Ressource.</span><span class="sxs-lookup"><span data-stu-id="10f73-p112">Specify other writable properties as necessary for your group. For more information, see the properties of the [group](../resources/group.md) resource.</span></span>

## <a name="response"></a><span data-ttu-id="10f73-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="10f73-176">Response</span></span>
<span data-ttu-id="10f73-177">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `201 Created` und das [group](../resources/group.md)-Objekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="10f73-177">If successful, this method returns `201 Created` response code and [group](../resources/group.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10f73-178">Beispiel</span><span class="sxs-lookup"><span data-stu-id="10f73-178">Example</span></span>
#### <a name="request-1"></a><span data-ttu-id="10f73-179">Anforderung 1</span><span class="sxs-lookup"><span data-stu-id="10f73-179">Request 1</span></span>
<span data-ttu-id="10f73-180">Die erste Beispielanforderung erstellt eine Office 365-Gruppe.</span><span class="sxs-lookup"><span data-stu-id="10f73-180">The following is an example of a request that creates an Office 365 Group.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_group"
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

#### <a name="response-1"></a><span data-ttu-id="10f73-181">Antwort 1</span><span class="sxs-lookup"><span data-stu-id="10f73-181">Response 1</span></span>
<span data-ttu-id="10f73-182">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="10f73-182">The following is an example of the response.</span></span>
><span data-ttu-id="10f73-p113">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="10f73-p113">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

#### <a name="request-2"></a><span data-ttu-id="10f73-185">Anforderung 2</span><span class="sxs-lookup"><span data-stu-id="10f73-185">Request 2</span></span>
<span data-ttu-id="10f73-186">Die zweite Beispielanforderung erstellt eine Office 365-Gruppe mit angegebenem Besitzer.</span><span class="sxs-lookup"><span data-stu-id="10f73-186">The second example request creates an Office 365 Group with owners specified.</span></span>
<!-- {
  "blockType": "request"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
  "description": "Group with owners",
  "displayName": "Group1",
  "groupTypes": [
    "Unified"
  ],
  "mailEnabled": true,
  "mailNickname": "group1",
  "securityEnabled": false,
  "owners@odata.bind": [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ]
}
```

#### <a name="response-2"></a><span data-ttu-id="10f73-187">Antwort 2</span><span class="sxs-lookup"><span data-stu-id="10f73-187">Response 2</span></span>
<span data-ttu-id="10f73-188">Es folgt ein Beispiel für die erfolgreiche Antwort.</span><span class="sxs-lookup"><span data-stu-id="10f73-188">The following is an example of the response.</span></span>
><span data-ttu-id="10f73-p114">**Hinweis:** Das hier gezeigte Antwortobjekt kann zur besseren Lesbarkeit gekürzt werden. Ein tatsächlicher Aufruf gibt alle Eigenschaften zurück.</span><span class="sxs-lookup"><span data-stu-id="10f73-p114">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "description": "Group with owners",
    "displayName": "Group1",
    "groupTypes": [
        "Unified"
    ],
    "mail": "group1@contoso.onmicrosoft.com",
    "mailEnabled": true,
    "mailNickname": "group1",
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
