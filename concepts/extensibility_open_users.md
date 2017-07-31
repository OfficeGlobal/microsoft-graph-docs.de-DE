<span data-ttu-id="b64f5-p107">Der Benutzer entscheidet, dass er kein Roamingprofil mehr benötigt, und löscht es. Dies kann über eine ```DELETE```-Anforderung im Wert der offenen Erweiterung erfolgen.</span><span class="sxs-lookup"><span data-stu-id="b64f5-p107">The user decides that they don't want a roaming profile anymore, so they delete it. This can be done with a ```DELETE``` request on the open extension value.</span></span>
Der Benutzer entscheidet, dass er kein Roamingprofil mehr benötigt, und löscht es. Dies kann über eine ```DELETE```-Anforderung im Wert der offenen Erweiterung erfolgen.

##### <a name="request"></a><span data-ttu-id="b64f5-135">Anforderung</span><span class="sxs-lookup"><span data-stu-id="b64f5-135">Request</span></span>
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

##### <a name="response"></a><span data-ttu-id="b64f5-136">Antwort</span><span class="sxs-lookup"><span data-stu-id="b64f5-136">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a><span data-ttu-id="b64f5-137">Weitere Artikel</span><span class="sxs-lookup"><span data-stu-id="b64f5-137">See also</span></span>

- [<span data-ttu-id="b64f5-138">Hinzufügen von benutzerdefinierten Daten zu Ressourcen mithilfe von Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="b64f5-138">Add custom data to resources using extensions</span></span>](extensibility_overview.md)
- [<span data-ttu-id="b64f5-139">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="b64f5-139">Add custom data to groups using schema extensions</span></span>](extensibility_schema_groups.md)
- [<span data-ttu-id="b64f5-140">openTypeExtension-Ressourcentyp</span><span class="sxs-lookup"><span data-stu-id="b64f5-140">openTypeExtension resource type</span></span>](../api-reference/v1.0/resources/opentypeextension.md)
- [<span data-ttu-id="b64f5-141">Offene Erweiterung erstellen</span><span class="sxs-lookup"><span data-stu-id="b64f5-141">Create open extension</span></span>](../api-reference/v1.0/api/opentypeextension_post_opentypeextension.md)
- [<span data-ttu-id="b64f5-142">Offene Erweiterung abrufen</span><span class="sxs-lookup"><span data-stu-id="b64f5-142">Get open extension</span></span>](../api-reference/v1.0/api/opentypeextension_get.md)
- [<span data-ttu-id="b64f5-143">Offene Erweiterung aktualisieren</span><span class="sxs-lookup"><span data-stu-id="b64f5-143">Update open extension</span></span>](../api-reference/v1.0/api/opentypeextension_update.md)
- [<span data-ttu-id="b64f5-144">Offene Erweiterung löschen</span><span class="sxs-lookup"><span data-stu-id="b64f5-144">Delete open extension</span></span>](../api-reference/v1.0/api/opentypeextension_delete.md)