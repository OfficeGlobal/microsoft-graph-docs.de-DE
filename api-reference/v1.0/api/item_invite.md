<span data-ttu-id="e061f-p102">Eine formatierte Nur-Text-Nachricht, die in der Freigabeeinladung enthalten ist. Die maximale Länge beträgt 2000 Zeichen.</span><span class="sxs-lookup"><span data-stu-id="e061f-p102">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span>                                          | Eine formatierte Nur-Text-Nachricht, die in der Freigabeeinladung enthalten ist. Die maximale Länge beträgt 2000 Zeichen. |
| <span data-ttu-id="e061f-122">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="e061f-122">requireSignIn</span></span>    | <span data-ttu-id="e061f-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="e061f-123">Boolean</span></span>                                         | <span data-ttu-id="e061f-124">Gibt an, ob der Empfänger der Einladung sich anmelden muss, um auf das freigegebene Element zuzugreifen.</span><span class="sxs-lookup"><span data-stu-id="e061f-124">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="e061f-125">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="e061f-125">sendInvitation</span></span>   | <span data-ttu-id="e061f-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="e061f-126">Boolean</span></span>                                         | <span data-ttu-id="e061f-127">Gibt an, ob eine E-Mail oder ein Beitrag generiert (falsch) oder ob nur die Berechtigung erstellt (true) wurde.</span><span class="sxs-lookup"><span data-stu-id="e061f-127">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="e061f-128">roles</span><span class="sxs-lookup"><span data-stu-id="e061f-128">roles</span></span>            | <span data-ttu-id="e061f-129">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="e061f-129">Collection(String)</span></span>                              | <span data-ttu-id="e061f-130">Gibt die Rollen an, die den Empfängern der Freigabeeinladung erteilt werden.</span><span class="sxs-lookup"><span data-stu-id="e061f-130">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <span data-ttu-id="e061f-131">Antwort</span><span class="sxs-lookup"><span data-stu-id="e061f-131">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="e061f-132">Wenn die Methode erfolgreich verläuft, werden der Antwortcode `200 OK` und das [permission](../resources/permission.md)-Sammlungsobjekt im Antworttext zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="e061f-132">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

## <span data-ttu-id="e061f-133">Beispiel</span><span class="sxs-lookup"><span data-stu-id="e061f-133">Example</span></span>
<a id="example" class="xliff"></a>
<span data-ttu-id="e061f-134">Nachfolgend sehen Sie ein Beispiel dafür, wie diese API aufgerufen wird.</span><span class="sxs-lookup"><span data-stu-id="e061f-134">Here is an example of how to call this API.</span></span>

##### <span data-ttu-id="e061f-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="e061f-135">Request</span></span>
<a id="request" class="xliff"></a>
<span data-ttu-id="e061f-136">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="e061f-136">Here is an example of the request.</span></span>

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

##### <span data-ttu-id="e061f-137">Antwort</span><span class="sxs-lookup"><span data-stu-id="e061f-137">Response</span></span>
<a id="response" class="xliff"></a>
<span data-ttu-id="e061f-138">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="e061f-138">Here is an example of the response.</span></span>
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

## <span data-ttu-id="e061f-139">Bemerkungen</span><span class="sxs-lookup"><span data-stu-id="e061f-139">Remarks</span></span>
<a id="remarks" class="xliff"></a>

* <span data-ttu-id="e061f-140">[Laufwerke](../resources/drive.md) mit dem**driveType** `personal` (OneDrive Personal) können keine Berechtigungen am Stamm-DriveItem erstellen oder ändern.</span><span class="sxs-lookup"><span data-stu-id="e061f-140">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 
* <span data-ttu-id="e061f-141">Eine Liste der verfügbaren Rollen finden Sie unter [Rollenaufzählung](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="e061f-141">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "item: invite",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
