<span data-ttu-id="d0fe3-p119">Senden Sie in Ihrer Antwort an Microsoft Graph einen `202 - Accepted` -Statuscode. Wenn Microsoft Graph keinen Code der Klasse 2xx erhält, wird versucht, die Benachrichtigung mehrmals erneut zu senden.</span><span class="sxs-lookup"><span data-stu-id="d0fe3-p119">Send a `202 - Accepted` status code in your response to Microsoft Graph. If Microsoft Graph doesn't receive a 2xx class code, it will retry resending the notification a number of times.</span></span>
3. Senden Sie in Ihrer Antwort an Microsoft Graph einen `202 - Accepted` -Statuscode. Wenn Microsoft Graph keinen Code der Klasse 2xx erhält, wird versucht, die Benachrichtigung mehrmals erneut zu senden.
  > <span data-ttu-id="d0fe3-198">Senden Sie auch dann einen `202 - Accepted`-Statuscode, wenn die Eigenschaft „clientState“ nicht mit derjenigen übereinstimmt, die in der Abonnementanfrage übermittelt wurde.</span><span class="sxs-lookup"><span data-stu-id="d0fe3-198">You should send a `202 - Accepted` status code even if the clientState property doesn't match the one submitted with the subscription request.</span></span>

<span data-ttu-id="d0fe3-199">Wiederholen Sie den Vorgang für weitere Benachrichtigungen in der Anfrage.</span><span class="sxs-lookup"><span data-stu-id="d0fe3-199">Repeat for other notifications in the request.</span></span>

# <span data-ttu-id="d0fe3-200">Zusätzliche Ressourcen</span><span class="sxs-lookup"><span data-stu-id="d0fe3-200">Additional resources</span></span>
<a id="additional-resources" class="xliff"></a>

* [<span data-ttu-id="d0fe3-201">Abonnementressourcentyp</span><span class="sxs-lookup"><span data-stu-id="d0fe3-201">Subscription resource type</span></span>](subscription.md)
* [<span data-ttu-id="d0fe3-202">Abonnement abrufen</span><span class="sxs-lookup"><span data-stu-id="d0fe3-202">Get subscription</span></span>](../api/subscription_get.md)
* [<span data-ttu-id="d0fe3-203">Abonnement erstellen</span><span class="sxs-lookup"><span data-stu-id="d0fe3-203">Create subscription</span></span>](../api/subscription_post_subscriptions.md)
* [<span data-ttu-id="d0fe3-204">Microsoft Graph Webhooks-Beispiel für Node.js</span><span class="sxs-lookup"><span data-stu-id="d0fe3-204">Microsoft Graph Webhooks Sample for Node.js</span></span>](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
* [<span data-ttu-id="d0fe3-205">Microsoft Graph Webhooks-Beispiel für ASP.NET</span><span class="sxs-lookup"><span data-stu-id="d0fe3-205">Microsoft Graph Webhooks Sample for ASP.NET</span></span>](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
