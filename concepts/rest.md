<span data-ttu-id="545b7-p119">Da Sie nun gelernt haben, wie Aufrufe für Microsoft Graph getätigt werden, können Sie anhand der API-Referenz beliebige Arten von Aufrufen erstellen, die für Ihre App erforderlich sind. Denken Sie daran, dass entsprechende Berechtigungen für die App bei der App-Registrierung für die Aufrufe konfiguriert sein müssen.</span><span class="sxs-lookup"><span data-stu-id="545b7-p119">Now that you've seen how to make calls to Microsoft Graph, you can use the API reference to construct any other kinds of calls your app needs to make. However, bear in mind that your app needs to have the appropriate permissions configured on the app registration for the calls it makes.</span></span>

```
GET https://graph.microsoft.com/v1.0/me/messages?$select=subject,from,receivedDateTime&$top=25&$orderby=receivedDateTime%20DESC
Accept: application/json
Authorization: Bearer eyJ0eXAi...b66LoPVA
```

Da Sie nun gelernt haben, wie Aufrufe für Microsoft Graph getätigt werden, können Sie anhand der API-Referenz beliebige Arten von Aufrufen erstellen, die für Ihre App erforderlich sind. Denken Sie daran, dass entsprechende Berechtigungen für die App bei der App-Registrierung für die Aufrufe konfiguriert sein müssen.

## <a name="next-steps"></a><span data-ttu-id="545b7-189">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="545b7-189">Next steps</span></span>
- <span data-ttu-id="545b7-190">Testen Sie die Möglichkeiten der REST-API mithilfe des [Graph-Explorers](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="545b7-190">Try out more of the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>

## <a name="see-also"></a><span data-ttu-id="545b7-191">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="545b7-191">See also</span></span>
- [<span data-ttu-id="545b7-192">Azure AD v2.0-Protokolle</span><span class="sxs-lookup"><span data-stu-id="545b7-192">Azure AD v2.0 protocols</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols/)
- [<span data-ttu-id="545b7-193">Azure AD v2.0-Tokens</span><span class="sxs-lookup"><span data-stu-id="545b7-193">Azure AD v2.0 tokens</span></span>](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-tokens/)
