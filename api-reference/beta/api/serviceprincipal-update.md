---
title: Serviceprincipal aktualisieren
description: Aktualisieren Sie die Eigenschaften des Serviceprincipal-Objekts.
ms.openlocfilehash: a24a8c949d48f577a3d7fe6208a1422819772801
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27065668"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="0132a-103">Serviceprincipal aktualisieren</span><span class="sxs-lookup"><span data-stu-id="0132a-103">Update serviceprincipal</span></span>

> <span data-ttu-id="0132a-104">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0132a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0132a-105">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0132a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0132a-106">Aktualisieren Sie die Eigenschaften des Serviceprincipal-Objekts.</span><span class="sxs-lookup"><span data-stu-id="0132a-106">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0132a-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0132a-107">Permissions</span></span>
<span data-ttu-id="0132a-p102">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0132a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0132a-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0132a-110">Permission type</span></span>      | <span data-ttu-id="0132a-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0132a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0132a-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0132a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0132a-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0132a-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0132a-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0132a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0132a-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0132a-115">Not supported.</span></span>    |
|<span data-ttu-id="0132a-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0132a-116">Application</span></span> | <span data-ttu-id="0132a-117">Application.ReadWrite.OwnedBy Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0132a-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0132a-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0132a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0132a-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0132a-119">Request headers</span></span>
| <span data-ttu-id="0132a-120">Name</span><span class="sxs-lookup"><span data-stu-id="0132a-120">Name</span></span>       | <span data-ttu-id="0132a-121">Typ</span><span class="sxs-lookup"><span data-stu-id="0132a-121">Type</span></span> | <span data-ttu-id="0132a-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0132a-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0132a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0132a-123">Authorization</span></span>  | <span data-ttu-id="0132a-124">string</span><span class="sxs-lookup"><span data-stu-id="0132a-124">string</span></span>  | <span data-ttu-id="0132a-p103">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0132a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0132a-127">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0132a-127">Request body</span></span>
<span data-ttu-id="0132a-p104">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="0132a-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0132a-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0132a-131">Property</span></span>     | <span data-ttu-id="0132a-132">Typ</span><span class="sxs-lookup"><span data-stu-id="0132a-132">Type</span></span>   |<span data-ttu-id="0132a-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0132a-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0132a-134">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="0132a-134">accountEnabled</span></span>|<span data-ttu-id="0132a-135">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="0132a-135">Boolean</span></span>|                <span data-ttu-id="0132a-136">**true,** Wenn das Dienstkonto für den Prinzipal aktiviert ist. anderenfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="0132a-136">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="0132a-137">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="0132a-137">appDisplayName</span></span>|<span data-ttu-id="0132a-138">String</span><span class="sxs-lookup"><span data-stu-id="0132a-138">String</span></span>|<span data-ttu-id="0132a-139">Der Anzeigename, der von der zugeordneten Anwendung verfügbar gemacht werden.</span><span class="sxs-lookup"><span data-stu-id="0132a-139">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="0132a-140">appId</span><span class="sxs-lookup"><span data-stu-id="0132a-140">appId</span></span>|<span data-ttu-id="0132a-141">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0132a-141">String</span></span>|<span data-ttu-id="0132a-142">Der eindeutige Bezeichner für die zugewiesene Anwendung (dessen **AppId** -Eigenschaft).</span><span class="sxs-lookup"><span data-stu-id="0132a-142">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="0132a-143">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="0132a-143">appRoleAssignmentRequired</span></span>|<span data-ttu-id="0132a-144">Boolesch</span><span class="sxs-lookup"><span data-stu-id="0132a-144">Boolean</span></span>|<span data-ttu-id="0132a-145">Gibt an, ob ein **AppRoleAssignment** für einen Benutzer oder Gruppe erforderlich ist, bevor Azure AD einen Benutzer oder eine Zugriffstoken an die Anwendung ausstellt.</span><span class="sxs-lookup"><span data-stu-id="0132a-145">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="0132a-146">**Notes**: erfordert Version 1.5 oder neuere, nicht NULL-Werte zulässt.</span><span class="sxs-lookup"><span data-stu-id="0132a-146">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="0132a-147">appRoles</span><span class="sxs-lookup"><span data-stu-id="0132a-147">appRoles</span></span>|<span data-ttu-id="0132a-148">appRole</span><span class="sxs-lookup"><span data-stu-id="0132a-148">appRole</span></span>|<span data-ttu-id="0132a-149">Die Rollen der Anwendung von der zugeordneten Anwendung verfügbar gemacht werden.</span><span class="sxs-lookup"><span data-stu-id="0132a-149">The application roles exposed by the associated application.</span></span> <span data-ttu-id="0132a-150">Weitere Informationen finden Sie in der Definition der **AppRoles** -Eigenschaft in der Anwendung Entität **Notes**: erfordert Version 1.5 oder neuere, nicht NULL-Werte zulässt.</span><span class="sxs-lookup"><span data-stu-id="0132a-150">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="0132a-151">displayName</span><span class="sxs-lookup"><span data-stu-id="0132a-151">displayName</span></span>|<span data-ttu-id="0132a-152">String</span><span class="sxs-lookup"><span data-stu-id="0132a-152">String</span></span>|<span data-ttu-id="0132a-153">Der Anzeigename für den Dienstprinzipal.</span><span class="sxs-lookup"><span data-stu-id="0132a-153">The display name for the service principal.</span></span>|
|<span data-ttu-id="0132a-154">errorUrl</span><span class="sxs-lookup"><span data-stu-id="0132a-154">errorUrl</span></span>|<span data-ttu-id="0132a-155">String</span><span class="sxs-lookup"><span data-stu-id="0132a-155">String</span></span>|            |
|<span data-ttu-id="0132a-156">Homepage</span><span class="sxs-lookup"><span data-stu-id="0132a-156">homepage</span></span>|<span data-ttu-id="0132a-157">String</span><span class="sxs-lookup"><span data-stu-id="0132a-157">String</span></span>|<span data-ttu-id="0132a-158">Die URL zur Homepage der zugehörigen Anwendung.</span><span class="sxs-lookup"><span data-stu-id="0132a-158">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="0132a-159">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="0132a-159">keyCredentials</span></span>|<span data-ttu-id="0132a-160">keyCredential</span><span class="sxs-lookup"><span data-stu-id="0132a-160">keyCredential</span></span>|<span data-ttu-id="0132a-161">Die Auflistung von wichtigen Anmeldeinformationen, die dem Prinzipal Dienst zugeordnet sind.</span><span class="sxs-lookup"><span data-stu-id="0132a-161">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="0132a-162">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0132a-162">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="0132a-163">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="0132a-163">logoutUrl</span></span>|<span data-ttu-id="0132a-164">String</span><span class="sxs-lookup"><span data-stu-id="0132a-164">String</span></span>| <span data-ttu-id="0132a-165">Gibt die URL, die von Microsoft Autorisierungsdienst Abmelden ein Benutzer mit der [Vorderseite-Kanal](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [Back-Kanal](https://openid.net/specs/openid-connect-backchannel-1_0.html) oder SAML Abmeldung Protokolle verwendet werden soll.</span><span class="sxs-lookup"><span data-stu-id="0132a-165">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="0132a-166">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="0132a-166">oauth2Permissions</span></span>|<span data-ttu-id="0132a-167">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="0132a-167">oAuth2Permission</span></span>|<span data-ttu-id="0132a-168">Die OAuth 2.0-Berechtigungen von der zugeordneten Anwendung verfügbar gemacht werden.</span><span class="sxs-lookup"><span data-stu-id="0132a-168">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="0132a-169">Weitere Informationen finden Sie in der Definition der **oauth2Permissions** -Eigenschaft in der Anwendung Entität.</span><span class="sxs-lookup"><span data-stu-id="0132a-169">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="0132a-170">**Notes**: erfordert Version 1.5 oder neuere, nicht NULL-Werte zulässt.</span><span class="sxs-lookup"><span data-stu-id="0132a-170">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="0132a-171">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="0132a-171">passwordCredentials</span></span>|<span data-ttu-id="0132a-172">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="0132a-172">passwordCredential</span></span>|<span data-ttu-id="0132a-173">Die Auflistung von Anmeldeinformationen den Dienstprinzipal zugeordnet.</span><span class="sxs-lookup"><span data-stu-id="0132a-173">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="0132a-174">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0132a-174">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="0132a-175">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="0132a-175">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="0132a-176">String</span><span class="sxs-lookup"><span data-stu-id="0132a-176">String</span></span>|<span data-ttu-id="0132a-177">Nur für interne Zwecke vorbehalten.</span><span class="sxs-lookup"><span data-stu-id="0132a-177">Reserved for internal use only.</span></span> <span data-ttu-id="0132a-178">Schreiben oder verlassen sich andernfalls auf diese Eigenschaft nicht.</span><span class="sxs-lookup"><span data-stu-id="0132a-178">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="0132a-179">Kann in zukünftigen Versionen entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="0132a-179">May be removed in future versions.</span></span>                            <span data-ttu-id="0132a-180">**Notes**: erfordert Version 1.5 oder höher.</span><span class="sxs-lookup"><span data-stu-id="0132a-180">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="0132a-181">publisherName</span><span class="sxs-lookup"><span data-stu-id="0132a-181">publisherName</span></span>|<span data-ttu-id="0132a-182">String</span><span class="sxs-lookup"><span data-stu-id="0132a-182">String</span></span>|<span data-ttu-id="0132a-183">Der Anzeigename des Mandanten in dem verbundenen Anwendung angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="0132a-183">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="0132a-184">replyUrls</span><span class="sxs-lookup"><span data-stu-id="0132a-184">replyUrls</span></span>|<span data-ttu-id="0132a-185">String</span><span class="sxs-lookup"><span data-stu-id="0132a-185">String</span></span>|<span data-ttu-id="0132a-186">Die URLs, dass Benutzertoken, um für die Anmeldung mit der zugeordneten Anwendung oder die Umleitung URIs, dass OAuth 2.0 Autorisierungscodes gesendet werden und Zugriffstoken werden für die zugewiesene Anwendung an.</span><span class="sxs-lookup"><span data-stu-id="0132a-186">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="0132a-187">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0132a-187">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="0132a-188">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="0132a-188">samlMetadataUrl</span></span>|<span data-ttu-id="0132a-189">String</span><span class="sxs-lookup"><span data-stu-id="0132a-189">String</span></span>|            |
|<span data-ttu-id="0132a-190">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="0132a-190">servicePrincipalNames</span></span>|<span data-ttu-id="0132a-191">String</span><span class="sxs-lookup"><span data-stu-id="0132a-191">String</span></span>|<span data-ttu-id="0132a-192">Die URIs, mit denen die zugewiesene Anwendung identifiziert.</span><span class="sxs-lookup"><span data-stu-id="0132a-192">The URIs that identify the associated application.</span></span> <span data-ttu-id="0132a-193">Weitere Informationen finden Sie unter [Application Objects und Service Principal-Objekte](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span><span class="sxs-lookup"><span data-stu-id="0132a-193">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="0132a-194">**Notes**: keine Nullwerte zulassen der **any** -Operator ist erforderlich für Filterausdrücke auf mehrwertige Eigenschaften; Weitere Informationen finden Sie unter [unterstützte Abfragen, Filter, und Paging-Optionen](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span><span class="sxs-lookup"><span data-stu-id="0132a-194">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="0132a-195">-Tags hinzugefügtes Markup</span><span class="sxs-lookup"><span data-stu-id="0132a-195">tags</span></span>|<span data-ttu-id="0132a-196">String</span><span class="sxs-lookup"><span data-stu-id="0132a-196">String</span></span>|                                        <span data-ttu-id="0132a-197">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="0132a-197">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="0132a-198">Antwort</span><span class="sxs-lookup"><span data-stu-id="0132a-198">Response</span></span>

<span data-ttu-id="0132a-199">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [ServicePrincipal](../resources/serviceprincipal.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="0132a-199">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0132a-200">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0132a-200">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0132a-201">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0132a-201">Request</span></span>
<span data-ttu-id="0132a-202">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0132a-202">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
##### <a name="response"></a><span data-ttu-id="0132a-203">Antwort</span><span class="sxs-lookup"><span data-stu-id="0132a-203">Response</span></span>
<span data-ttu-id="0132a-p113">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0132a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
