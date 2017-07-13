<span data-ttu-id="09b0d-p109">Im folgenden Beispiel wird nach der Gruppe mit der Erweiterung `graphlearn_courses` gesucht, deren `courseId`-Eigenschaft den Wert `123` hat, und es werden die Gruppeneigenschaften **displayName**, **id** und **description** sowie die benutzerdefinierten Daten in der Erweiterung `graphlearn_courses` abgerufen. (Denken Sie daran, in der tatsächlichen Abfrage URL-Codierung nach Bedarf anzuwenden.)</span><span class="sxs-lookup"><span data-stu-id="09b0d-p109">The following example looks for the group that has the `graphlearn_courses` extension with a `courseId` property value matching `123`, and gets the group properties **displayName**, **id**, and **description**, and the custom data in the `graphlearn_courses` extension. (In the actual query, make sure you apply URL encoding as necessary.)</span></span>

Im folgenden Beispiel wird nach der Gruppe mit der Erweiterung `graphlearn_courses` gesucht, deren `courseId`-Eigenschaft den Wert `123` hat, und es werden die Gruppeneigenschaften **displayName**, **id** und **description** sowie die benutzerdefinierten Daten in der Erweiterung `graphlearn_courses` abgerufen. (Denken Sie daran, in der tatsächlichen Abfrage URL-Codierung nach Bedarf anzuwenden.)

#### <span data-ttu-id="09b0d-157">Anforderung</span><span class="sxs-lookup"><span data-stu-id="09b0d-157">Request</span></span>
<a id="request" class="xliff"></a>

```http
GET https://graph.microsoft.com/v1.0/groups?$filter=graphlearn_courses/courseId eq ‘123’&$select=displayName,id,description,graphlearn_courses
```


##### <span data-ttu-id="09b0d-158">Antwort</span><span class="sxs-lookup"><span data-stu-id="09b0d-158">Response</span></span>
<a id="response" class="xliff"></a>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 326
{
  "value": [
    {
      "displayName": "New Managers March 2017",
      "id": "14429ae5-3e74-41a2-9fa8-028fbb984637",
      "description": "New Managers training course for March 2017",
      "graphlearn_courses": {
        "@odata.type": "#microsoft.graph.ComplexExtensionValue",
        "courseId":"123",
        "courseName":"New Managers",
        "courseType":"Online"
      }
    }
  ]
}
```

## <span data-ttu-id="09b0d-159">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="09b0d-159">See also</span></span>
<a id="see-also" class="xliff"></a>

- [<span data-ttu-id="09b0d-160">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="09b0d-160">Add custom data to resources using extensions</span></span>](extensibility_overview.md)
- [<span data-ttu-id="09b0d-161">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen (Preview)</span><span class="sxs-lookup"><span data-stu-id="09b0d-161">Add custom data to users using open extensions (preview)</span></span>](extensibility_open_users.md)
- <span data-ttu-id="09b0d-162">
  [Office 365-Domänen](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span><span class="sxs-lookup"><span data-stu-id="09b0d-162">[Office 365 domains](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span></span>
- [<span data-ttu-id="09b0d-163">Hinzufügen und Überprüfen einer Domäne für das NEUE Office 365</span><span class="sxs-lookup"><span data-stu-id="09b0d-163">Adding and Verifying a Domain for the NEW Office 365</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
- [<span data-ttu-id="09b0d-164">schemaExtension-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="09b0d-164">schemaExtension resource type</span></span>](../api-reference/v1.0/resources/schemaextension.md)
- [<span data-ttu-id="09b0d-165">schemaExtensions aufführen</span><span class="sxs-lookup"><span data-stu-id="09b0d-165">List schemaExtensions</span></span>](../api-reference/v1.0/api/schemaextension_list.md)
- [<span data-ttu-id="09b0d-166">schemaExtension erstellen</span><span class="sxs-lookup"><span data-stu-id="09b0d-166">Create schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_post_schemaextensions.md)
- [<span data-ttu-id="09b0d-167">schemaExtension abrufen</span><span class="sxs-lookup"><span data-stu-id="09b0d-167">Get schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_get.md)
- [<span data-ttu-id="09b0d-168">schemaExtension aktualisieren</span><span class="sxs-lookup"><span data-stu-id="09b0d-168">Update schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_update.md)
- [<span data-ttu-id="09b0d-169">schemaExtension löschen</span><span class="sxs-lookup"><span data-stu-id="09b0d-169">Delete schemaExtension</span></span>](../api-reference/v1.0/api/schemaextension_delete.md)
