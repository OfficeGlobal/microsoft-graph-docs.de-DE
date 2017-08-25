# <a name="send-a-sharing-invitation"></a><span data-ttu-id="960d8-101">Freigabeeinladung senden</span><span class="sxs-lookup"><span data-stu-id="960d8-101">Send a sharing invitation</span></span>

<span data-ttu-id="960d8-p101">Sendet eine Freigabeeinladung für ein **DriveItem**-Element. Eine Freigabeeinladung stellt Berechtigungen für Empfänger bereit und sendet optional eine E-Mail-Nachricht an den Empfänger, um diesen über die Freigabe in Kenntnis zu setzen.</span><span class="sxs-lookup"><span data-stu-id="960d8-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="960d8-104">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="960d8-104">Permissions</span></span>
<span data-ttu-id="960d8-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="960d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="960d8-107">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="960d8-107">Permission type</span></span>      | <span data-ttu-id="960d8-108">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="960d8-108">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="960d8-109">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="960d8-109">Delegated (work or school account)</span></span> | <span data-ttu-id="960d8-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="960d8-110">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    | 
|<span data-ttu-id="960d8-111">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="960d8-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="960d8-112">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="960d8-112">Files.ReadWrite, Files.ReadWrite.All</span></span>    | 
|<span data-ttu-id="960d8-113">Anwendung</span><span class="sxs-lookup"><span data-stu-id="960d8-113">Application</span></span> | <span data-ttu-id="960d8-114">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="960d8-114">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="960d8-115">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="960d8-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/items/{item-id}/invite
POST /drive/items/{item-id}/invite
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
```

## <a name="request-body"></a><span data-ttu-id="960d8-116">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="960d8-116">Request body</span></span>
<span data-ttu-id="960d8-117">Geben Sie im Anforderungstext ein JSON-Objekt mit den folgenden Parametern an.</span><span class="sxs-lookup"><span data-stu-id="960d8-117">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="960d8-118">Parameter</span><span class="sxs-lookup"><span data-stu-id="960d8-118">Parameter</span></span>        | <span data-ttu-id="960d8-119">Typ</span><span class="sxs-lookup"><span data-stu-id="960d8-119">Type</span></span>                                            | <span data-ttu-id="960d8-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="960d8-120">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="960d8-121">recipients</span><span class="sxs-lookup"><span data-stu-id="960d8-121">recipients</span></span>       | <span data-ttu-id="960d8-122">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="960d8-122">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="960d8-123">Eine Sammlung der Empfänger, die Zugriff und die Freigabeeinladung erhalten.</span><span class="sxs-lookup"><span data-stu-id="960d8-123">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="960d8-124">message</span><span class="sxs-lookup"><span data-stu-id="960d8-124">message</span></span>          | <span data-ttu-id="960d8-125">String</span><span class="sxs-lookup"><span data-stu-id="960d8-125">String</span></span>                                          | <span data-ttu-id="960d8-p103">Eine formatierte Nur-Text-Nachricht, die in der Freigabeeinladung enthalten ist. Die maximale Länge beträgt 2000 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="960d8-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="960d8-128">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="960d8-128">requireSignIn</span></span>    | <span data-ttu-id="960d8-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="960d8-129">Boolean</span></span>                                         | <span data-ttu-id="960d8-130">Gibt an, ob der Empfänger der Einladung sich anmelden muss, um auf das freigegebene Element zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="960d8-130">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="960d8-131">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="960d8-131">sendInvitation</span></span>   | <span data-ttu-id="960d8-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="960d8-132">Boolean</span></span>                                         | <span data-ttu-id="960d8-133">Gibt an, ob eine E-Mail oder ein Beitrag generiert (falsch) oder ob nur die Berechtigung erstellt (true) wurde.</span><span class="sxs-lookup"><span data-stu-id="960d8-133">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="960d8-134">roles</span><span class="sxs-lookup"><span data-stu-id="960d8-134">roles</span></span>            | <span data-ttu-id="960d8-135">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="960d8-135">Collection(String)</span></span>                              | <span data-ttu-id="960d8-136">Gibt die Rollen an, die den Empfängern der Freigabeeinladung erteilt werden.</span><span class="sxs-lookup"><span data-stu-id="960d8-136">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="response"></a><span data-ttu-id="960d8-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="960d8-137">Response</span></span>

<span data-ttu-id="960d8-138">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [permission](../resources/permission.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="960d8-138">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="960d8-139">Beispiel</span><span class="sxs-lookup"><span data-stu-id="960d8-139">Example</span></span>
<span data-ttu-id="960d8-140">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="960d8-140">Here is an example of how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="960d8-141">Anforderung</span><span class="sxs-lookup"><span data-stu-id="960d8-141">Request</span></span>
<span data-ttu-id="960d8-142">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="960d8-142">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "item_invite"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

##### <a name="response"></a><span data-ttu-id="960d8-143">Antwort</span><span class="sxs-lookup"><span data-stu-id="960d8-143">Response</span></span>
<span data-ttu-id="960d8-144">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="960d8-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="960d8-145">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="960d8-145">Remarks</span></span>

* <span data-ttu-id="960d8-146">[Laufwerke](../resources/drive.md) mit dem**driveType** `personal` (OneDrive Personal) können keine Berechtigungen am Stamm-DriveItem erstellen oder ändern.</span><span class="sxs-lookup"><span data-stu-id="960d8-146">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 
* <span data-ttu-id="960d8-147">Eine Liste der verfügbaren Rollen finden Sie unter [Rollenaufzählung](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="960d8-147">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "item: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
