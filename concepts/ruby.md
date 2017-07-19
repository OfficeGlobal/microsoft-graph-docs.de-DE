<span data-ttu-id="9e539-p119">Um die E-Mail zu erstellen, zieht der Code den Benutzernamen aus dem Sitzungstoken und die E-Mail-Adresse des Empfängers aus den Parametern des Formulars heraus. Der Code liest dann den Textkörper der E-Mail aus einer Vorlage, die im Projekt enthalten ist, interpoliert den Benutzernamen und die E-Mail-Adresse und fügt den Text der E-Mail-Nachricht als Textkörper der HTTP-Anforderung an.</span><span class="sxs-lookup"><span data-stu-id="9e539-p119">To create the email, the code pulls the user name from the session token and the recipient email address from the parameters passed from the form. The code then reads the email body from a template included in the project, interpolates the user name and email address, and attaches the email text as the HTTP request body.</span></span>

Um die E-Mail zu erstellen, zieht der Code den Benutzernamen aus dem Sitzungstoken und die E-Mail-Adresse des Empfängers aus den Parametern des Formulars heraus. Der Code liest dann den Textkörper der E-Mail aus einer Vorlage, die im Projekt enthalten ist, interpoliert den Benutzernamen und die E-Mail-Adresse und fügt den Text der E-Mail-Nachricht als Textkörper der HTTP-Anforderung an.

<span data-ttu-id="9e539-194">Zum Senden der E-Mail erstellt der Code die HTTP-Anforderung, fügt das Zugriffstoken als Autorisierungsheader hinzu und sendet dann die Anfrage an den Sendmail-Endpunkt.</span><span class="sxs-lookup"><span data-stu-id="9e539-194">To send the email, the code constructs the HTTP request, attaches the access token as an authorization header, and then posts the request to the send email endpoint.</span></span>

<span data-ttu-id="9e539-195">Schließlich verwendet der Code, den zurückgegebenen HTTP-Antwortcode, um den Benutzer zu informieren, ob die E-Mail erfolgreich war oder nicht.</span><span class="sxs-lookup"><span data-stu-id="9e539-195">Finally, the code uses the HTTP response code returned to notify the user whether or not the email was successful.</span></span>

## <a name="run-the-app"></a><span data-ttu-id="9e539-196">Ausführen der App</span><span class="sxs-lookup"><span data-stu-id="9e539-196">Run the app</span></span>

1. <span data-ttu-id="9e539-197">Installieren Sie die Rails-Anwendung und -Abhängigkeiten mit dem folgenden Befehl.</span><span class="sxs-lookup"><span data-stu-id="9e539-197">Install the Rails application and dependencies with the following command.</span></span>

    ```
    bundle install
    ```
2. <span data-ttu-id="9e539-198">Geben Sie zum Starten der Rails-Anwendung den folgenden Befehl ein.</span><span class="sxs-lookup"><span data-stu-id="9e539-198">To start the Rails application, type the following command.</span></span>

    ```
    rackup -p 3000
    ```
3. <span data-ttu-id="9e539-199">Navigieren Sie im Webbrowser zu `http://localhost:3000`.</span><span class="sxs-lookup"><span data-stu-id="9e539-199">Go to `http://localhost:3000` in your web browser.</span></span>

## <a name="see-also"></a><span data-ttu-id="9e539-200">Siehe auch</span><span class="sxs-lookup"><span data-stu-id="9e539-200">See also</span></span>
- <span data-ttu-id="9e539-201">Testen Sie die REST-API mithilfe des [Graph-Explorers](https://graph.microsoft.io/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="9e539-201">Try out the REST API using the [Graph explorer](https://graph.microsoft.io/graph-explorer).</span></span>
- <span data-ttu-id="9e539-202">Schauen Sie sich weitere [Microsoft Graph-Beispiele](https://github.com/microsoftgraph) auf GitHub an.</span><span class="sxs-lookup"><span data-stu-id="9e539-202">Explore our other [Microsoft Graph samples](https://github.com/microsoftgraph) on GitHub.</span></span>
- [<span data-ttu-id="9e539-203">Abrufen von Zugriffstoken zum Aufrufen von Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9e539-203">Get access tokens to call Microsoft Graph</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [<span data-ttu-id="9e539-204">Im Namen eines Benutzers zugreifen</span><span class="sxs-lookup"><span data-stu-id="9e539-204">Get access on behalf of a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [<span data-ttu-id="9e539-205">Ohne Benutzer zugreifen</span><span class="sxs-lookup"><span data-stu-id="9e539-205">Get access without a user</span></span>](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)


