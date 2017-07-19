<span data-ttu-id="57798-p116">Um Erweiterungsdaten aus einer Ressource auslesen oder in eine Ressource schreiben zu können, benötigen Sie dieselben [Berechtigungen](./permissions_reference.md) wie zum Lesen der Ressource und zum Schreiben in die Ressource.  Damit eine App beispielsweise das Profil des angemeldeten Benutzers mit benutzerdefinierten App-Daten aktualisieren kann, muss sie die Berechtigung *User.ReadWrite.All* besitzen.</span><span class="sxs-lookup"><span data-stu-id="57798-p116">The same [permissions](./permissions_reference.md) that are required to read from or write to a specific resource are also required to read from or write to any extensions data on that resource.  For example, for an app to be able to update the signed-in user's profile with custom app data, the app must have been granted the *User.ReadWrite.All* permission.</span></span>

Um Erweiterungsdaten aus einer Ressource auslesen oder in eine Ressource schreiben zu können, benötigen Sie dieselben [Berechtigungen](./permissions_reference.md) wie zum Lesen der Ressource und zum Schreiben in die Ressource.  Damit eine App beispielsweise das Profil des angemeldeten Benutzers mit benutzerdefinierten App-Daten aktualisieren kann, muss sie die Berechtigung *User.ReadWrite.All* besitzen.

<span data-ttu-id="57798-229">Zusätzlich muss einer App die Berechtigung *Directory.AccessAsUser.All* gewährt werden, um Schemaerweiterungsdefinitionen zu erstellen und zu verwalten.</span><span class="sxs-lookup"><span data-stu-id="57798-229">Additionally, to create and manage schema extension definitions, an application must be granted the *Directory.AccessAsUser.All* permission.</span></span>

## <a name="data-limits"></a><span data-ttu-id="57798-230">Beschränkungen für Daten</span><span class="sxs-lookup"><span data-stu-id="57798-230">Data limits</span></span>

### <a name="open-extension-limits"></a><span data-ttu-id="57798-231">Beschränkungen für offene Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="57798-231">Open extension limits</span></span>
<span data-ttu-id="57798-232">Die folgenden Beschränkungen gelten für Verzeichnisressourcen (z. B. **user**, **group**, **device**):</span><span class="sxs-lookup"><span data-stu-id="57798-232">The following limits apply to directory resources (such as **user**, **group**, **device**):</span></span>

- <span data-ttu-id="57798-233">Jede offene Erweiterung kann bis zu 2 KB Daten enthalten (einschließlich der Erweiterungsdefinition selbst).</span><span class="sxs-lookup"><span data-stu-id="57798-233">Each open extension can have up to 2KB of data (including the extension definition itself).</span></span>
- <span data-ttu-id="57798-234">Eine Anwendung kann bis zu zwei offene Erweiterungen pro Ressourceninstanz hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="57798-234">An application can add up to two open extensions per resource instance.</span></span>

### <a name="schema-extension-limits"></a><span data-ttu-id="57798-235">Beschränkungen für Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="57798-235">Schema extension limits</span></span>
<span data-ttu-id="57798-236">Eine Anwendung kann nicht mehr als fünf **Schemaerweiterungs**definitionen erstellen.</span><span class="sxs-lookup"><span data-stu-id="57798-236">An application may create no more than five **schema extension** definitions.</span></span>

## <a name="known-limitations"></a><span data-ttu-id="57798-237">Bekannte Einschränkungen</span><span class="sxs-lookup"><span data-stu-id="57798-237">Known limitations</span></span>

<span data-ttu-id="57798-238">Bekannte Einschränkungen bei der Verwendung von Erweiterungen finden Sie im [Abschnitt zu Erweiterungen](known_issues.md#extensions) im Artikel über bekannte Probleme.</span><span class="sxs-lookup"><span data-stu-id="57798-238">For known limitations using extensions, see the [extensions section](known_issues.md#extensions) in the known issues article.</span></span>

## <a name="see-also"></a><span data-ttu-id="57798-239">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="57798-239">See also</span></span>

[<span data-ttu-id="57798-240">Office 365-Domänen</span><span class="sxs-lookup"><span data-stu-id="57798-240">Office 365 domains</span></span>](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)

[<span data-ttu-id="57798-241">Hinzufügen und Überprüfen einer Domäne für einen Office 365-Mandanten</span><span class="sxs-lookup"><span data-stu-id="57798-241">Adding and verifying a domain for an Office 365 tenant</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)


## <a name="next-steps"></a><span data-ttu-id="57798-242">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="57798-242">Next steps</span></span>

<span data-ttu-id="57798-243">Sehen Sie sich ein Beispiel an, in dem die **user**-Ressource mithilfe einer offenen Erweiterung um benutzerdefinierte Roamingprofildaten erweitert wird:</span><span class="sxs-lookup"><span data-stu-id="57798-243">See an example that uses an open extension to extend the **user** resource with custom roaming profile data:</span></span>

[<span data-ttu-id="57798-244">Hinzufügen von benutzerdefinierten Daten zu Benutzern mithilfe offener Erweiterungen</span><span class="sxs-lookup"><span data-stu-id="57798-244">Add custom data to users using open extensions</span></span>](extensibility_open_users.md)

<span data-ttu-id="57798-245">Sehen Sie sich ein Beispiel an, in dem die **group**-Ressource mithilfe einer Schemaerweiterung um Schulungskursdaten erweitert wird:</span><span class="sxs-lookup"><span data-stu-id="57798-245">See an example that uses a schema extension to extend the **group** resource with training course data:</span></span>

[<span data-ttu-id="57798-246">Hinzufügen von benutzerdefinierten Daten zu Gruppen mithilfe von Schemaerweiterungen</span><span class="sxs-lookup"><span data-stu-id="57798-246">Add custom data to groups using schema extensions</span></span>](extensibility_schema_groups.md)

