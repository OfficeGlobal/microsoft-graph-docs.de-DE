---
title: Serviceprincipal aktualisieren
description: Aktualisieren Sie die Eigenschaften des Serviceprincipal-Objekts.
localization_priority: Normal
ms.openlocfilehash: a562bca03881923cfc21d32eadee2a7f7053fa9b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641176"
---
# <a name="update-serviceprincipal"></a><span data-ttu-id="73f54-103">Serviceprincipal aktualisieren</span><span class="sxs-lookup"><span data-stu-id="73f54-103">Update serviceprincipal</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73f54-104">Aktualisieren Sie die Eigenschaften des Serviceprincipal-Objekts.</span><span class="sxs-lookup"><span data-stu-id="73f54-104">Update the properties of serviceprincipal object.</span></span>
## <a name="permissions"></a><span data-ttu-id="73f54-105">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="73f54-105">Permissions</span></span>
<span data-ttu-id="73f54-p101">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73f54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73f54-108">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="73f54-108">Permission type</span></span>      | <span data-ttu-id="73f54-109">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="73f54-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73f54-110">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="73f54-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73f54-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="73f54-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="73f54-112">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="73f54-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73f54-113">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="73f54-113">Not supported.</span></span>    |
|<span data-ttu-id="73f54-114">Anwendung</span><span class="sxs-lookup"><span data-stu-id="73f54-114">Application</span></span> | <span data-ttu-id="73f54-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73f54-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73f54-116">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="73f54-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a><span data-ttu-id="73f54-117">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="73f54-117">Request headers</span></span>
| <span data-ttu-id="73f54-118">Name</span><span class="sxs-lookup"><span data-stu-id="73f54-118">Name</span></span>       | <span data-ttu-id="73f54-119">Typ</span><span class="sxs-lookup"><span data-stu-id="73f54-119">Type</span></span> | <span data-ttu-id="73f54-120">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73f54-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="73f54-121">Autorisierung</span><span class="sxs-lookup"><span data-stu-id="73f54-121">Authorization</span></span>  | <span data-ttu-id="73f54-122">string</span><span class="sxs-lookup"><span data-stu-id="73f54-122">string</span></span>  | <span data-ttu-id="73f54-p102">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="73f54-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="73f54-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="73f54-125">Request body</span></span>
<span data-ttu-id="73f54-p103">Geben Sie im Anforderungstext die Werte für die relevanten Felder an, die aktualisiert werden sollen. Vorhandene Eigenschaften, die nicht im Anforderungstext enthalten sind, behalten ihre vorherigen Werte oder werden basierend auf Änderungen an anderen Eigenschaftswerten neu berechnet. Aus Gründen der Leistung sollten Sie vorhandene Werte, die nicht geändert wurden, nicht angeben.</span><span class="sxs-lookup"><span data-stu-id="73f54-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="73f54-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="73f54-129">Property</span></span>     | <span data-ttu-id="73f54-130">Typ</span><span class="sxs-lookup"><span data-stu-id="73f54-130">Type</span></span>   |<span data-ttu-id="73f54-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="73f54-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73f54-132">accountEnabled</span><span class="sxs-lookup"><span data-stu-id="73f54-132">accountEnabled</span></span>|<span data-ttu-id="73f54-133">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="73f54-133">Boolean</span></span>|                <span data-ttu-id="73f54-134">**True**, wenn das Dienstprinzipalkonto aktiviert ist; andernfalls **false**.</span><span class="sxs-lookup"><span data-stu-id="73f54-134">**true** if the service principal account is enabled; otherwise, **false**.</span></span>            |
|<span data-ttu-id="73f54-135">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="73f54-135">appDisplayName</span></span>|<span data-ttu-id="73f54-136">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f54-136">String</span></span>|<span data-ttu-id="73f54-137">Der von der verknüpften Anwendung verfügbar gemachte Anzeigename.</span><span class="sxs-lookup"><span data-stu-id="73f54-137">The display name exposed by the associated application.</span></span>|
|<span data-ttu-id="73f54-138">appId</span><span class="sxs-lookup"><span data-stu-id="73f54-138">appId</span></span>|<span data-ttu-id="73f54-139">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f54-139">String</span></span>|<span data-ttu-id="73f54-140">Die eindeutige ID für die verknüpfte Anwendung (die **appId**-Eigenschaft).</span><span class="sxs-lookup"><span data-stu-id="73f54-140">The unique identifier for the associated application (its **appId** property).</span></span>|
|<span data-ttu-id="73f54-141">appRoleAssignmentRequired</span><span class="sxs-lookup"><span data-stu-id="73f54-141">appRoleAssignmentRequired</span></span>|<span data-ttu-id="73f54-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="73f54-142">Boolean</span></span>|<span data-ttu-id="73f54-143">Gibt an, ob eine **eppRoleAssignment** für einen Benutzer oder eine Gruppe erforderlichist, bevor Azure Active Directory ein Benutzer- oder Zugriffstoken für die Anwendung ausstellt.</span><span class="sxs-lookup"><span data-stu-id="73f54-143">Specifies whether an **appRoleAssignment** to a user or group is required before Azure AD will issue a user or access token to the application.</span></span>                            <span data-ttu-id="73f54-144">**Notes**: erfordert Version 1.5 oder neuere, nicht NULL-Werte zulässt.</span><span class="sxs-lookup"><span data-stu-id="73f54-144">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="73f54-145">appRoles</span><span class="sxs-lookup"><span data-stu-id="73f54-145">appRoles</span></span>|<span data-ttu-id="73f54-146">appRole</span><span class="sxs-lookup"><span data-stu-id="73f54-146">appRole</span></span>|<span data-ttu-id="73f54-147">Die von der verknüpften Anwendung verfügbar gemachten Anwendungsrollen.</span><span class="sxs-lookup"><span data-stu-id="73f54-147">The application roles exposed by the associated application.</span></span> <span data-ttu-id="73f54-148">Weitere Informationen finden Sie in der Definition der **AppRoles** -Eigenschaft in der Anwendung Entität **Notes**: erfordert Version 1.5 oder neuere, nicht NULL-Werte zulässt.</span><span class="sxs-lookup"><span data-stu-id="73f54-148">For more information see the **appRoles** property definition on the application entity                            **Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="73f54-149">displayName</span><span class="sxs-lookup"><span data-stu-id="73f54-149">displayName</span></span>|<span data-ttu-id="73f54-150">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f54-150">String</span></span>|<span data-ttu-id="73f54-151">Der Anzeigename für den Dienstprinzipal.</span><span class="sxs-lookup"><span data-stu-id="73f54-151">The display name for the service principal.</span></span>|
|<span data-ttu-id="73f54-152">errorUrl</span><span class="sxs-lookup"><span data-stu-id="73f54-152">errorUrl</span></span>|<span data-ttu-id="73f54-153">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f54-153">String</span></span>|            |
|<span data-ttu-id="73f54-154">homepage</span><span class="sxs-lookup"><span data-stu-id="73f54-154">homepage</span></span>|<span data-ttu-id="73f54-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f54-155">String</span></span>|<span data-ttu-id="73f54-156">Die URL zur Homepage der zugehörigen Anwendung.</span><span class="sxs-lookup"><span data-stu-id="73f54-156">The URL to the homepage of the associated application.</span></span>|
|<span data-ttu-id="73f54-157">keyCredentials</span><span class="sxs-lookup"><span data-stu-id="73f54-157">keyCredentials</span></span>|<span data-ttu-id="73f54-158">keyCredential</span><span class="sxs-lookup"><span data-stu-id="73f54-158">keyCredential</span></span>|<span data-ttu-id="73f54-159">Die Auflistung der wichtigsten Anmeldeinformationen, die mit dem Dienstprinzipal verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="73f54-159">The collection of key credentials associated with the service principal.</span></span>                            <span data-ttu-id="73f54-160">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="73f54-160">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="73f54-161">logoutUrl</span><span class="sxs-lookup"><span data-stu-id="73f54-161">logoutUrl</span></span>|<span data-ttu-id="73f54-162">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f54-162">String</span></span>| <span data-ttu-id="73f54-163">Gibt die URL an, die vom Autorisierungsdienst von Microsoft verwendet wird, um einen Benutzer mithilfe von [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html)-, [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html)- oder SAML-Abmeldeprotokollen abzumelden.</span><span class="sxs-lookup"><span data-stu-id="73f54-163">Specifies the URL that will be used by Microsoft's authorization service to logout an user using [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) or SAML logout protocols.</span></span> |
|<span data-ttu-id="73f54-164">oauth2Permissions</span><span class="sxs-lookup"><span data-stu-id="73f54-164">oauth2Permissions</span></span>|<span data-ttu-id="73f54-165">oAuth2Permission</span><span class="sxs-lookup"><span data-stu-id="73f54-165">oAuth2Permission</span></span>|<span data-ttu-id="73f54-166">Die von der verknüpften Anwendung verfügbar gemachten OAuth 2.0-Berechtigungen.</span><span class="sxs-lookup"><span data-stu-id="73f54-166">The OAuth 2.0 permissions exposed by the associated application.</span></span> <span data-ttu-id="73f54-167">Weitere Informationen finden Sie in der **oauth2Permissions**-Eigenschaftsdefinition in der application-Entität.</span><span class="sxs-lookup"><span data-stu-id="73f54-167">For more information see the **oauth2Permissions** property definition on the application entity.</span></span>                            <span data-ttu-id="73f54-168">**Notes**: erfordert Version 1.5 oder neuere, nicht NULL-Werte zulässt.</span><span class="sxs-lookup"><span data-stu-id="73f54-168">**Notes**: Requires version 1.5 or newer, not nullable.</span></span>            |
|<span data-ttu-id="73f54-169">passwordCredentials</span><span class="sxs-lookup"><span data-stu-id="73f54-169">passwordCredentials</span></span>|<span data-ttu-id="73f54-170">passwordCredential</span><span class="sxs-lookup"><span data-stu-id="73f54-170">passwordCredential</span></span>|<span data-ttu-id="73f54-171">Die Auflistung der Kennwortanmeldeinformationen, die mit dem Dienstprinzipal verknüpft sind.</span><span class="sxs-lookup"><span data-stu-id="73f54-171">The collection of password credentials associated with the service principal.</span></span>                            <span data-ttu-id="73f54-172">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="73f54-172">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="73f54-173">preferredTokenSigningKeyThumbprint</span><span class="sxs-lookup"><span data-stu-id="73f54-173">preferredTokenSigningKeyThumbprint</span></span>|<span data-ttu-id="73f54-174">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f54-174">String</span></span>|<span data-ttu-id="73f54-175">Nur für die interne Verwendung reserviert.</span><span class="sxs-lookup"><span data-stu-id="73f54-175">Reserved for internal use only.</span></span> <span data-ttu-id="73f54-176">Schreiben Sie diese Eigenschaft nicht, und verwenden Sie diese Eigenschaft nicht anderweitig.</span><span class="sxs-lookup"><span data-stu-id="73f54-176">Do not write or otherwise rely on this property.</span></span> <span data-ttu-id="73f54-177">Sie kann in zukünftigen Versionen möglicherweise entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="73f54-177">May be removed in future versions.</span></span>                            <span data-ttu-id="73f54-178">**Notes**: erfordert Version 1.5 oder höher.</span><span class="sxs-lookup"><span data-stu-id="73f54-178">**Notes**: Requires version 1.5 or newer.</span></span>            |
|<span data-ttu-id="73f54-179">publisherName</span><span class="sxs-lookup"><span data-stu-id="73f54-179">publisherName</span></span>|<span data-ttu-id="73f54-180">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f54-180">String</span></span>|<span data-ttu-id="73f54-181">Der Anzeigename des Mandanten, in dem verknüpfte Anwendung angegeben wird.</span><span class="sxs-lookup"><span data-stu-id="73f54-181">The display name of the tenant in which the associated application is specified.</span></span>|
|<span data-ttu-id="73f54-182">replyUrls</span><span class="sxs-lookup"><span data-stu-id="73f54-182">replyUrls</span></span>|<span data-ttu-id="73f54-183">String</span><span class="sxs-lookup"><span data-stu-id="73f54-183">String</span></span>|<span data-ttu-id="73f54-184">Die URLs, an die Benutzertoken zur Anmeldung bei der verknüpften Anwendung gesendet werden, oder die Umleitungs-URIs, an die die OAuth 2.0-Autorisierungscodes und Zugriffstoken für die verknüpfte Anwendung gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="73f54-184">The URLs that user tokens are sent to for sign in with the associated application, or the redirect URIs that OAuth 2.0 authorization codes and access tokens are sent to for the associated application.</span></span>                            <span data-ttu-id="73f54-185">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="73f54-185">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="73f54-186">samlMetadataUrl</span><span class="sxs-lookup"><span data-stu-id="73f54-186">samlMetadataUrl</span></span>|<span data-ttu-id="73f54-187">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="73f54-187">String</span></span>|            |
|<span data-ttu-id="73f54-188">servicePrincipalNames</span><span class="sxs-lookup"><span data-stu-id="73f54-188">servicePrincipalNames</span></span>|<span data-ttu-id="73f54-189">String</span><span class="sxs-lookup"><span data-stu-id="73f54-189">String</span></span>|<span data-ttu-id="73f54-190">Die URLs, die die verknüpfte Anwendung identifizieren.</span><span class="sxs-lookup"><span data-stu-id="73f54-190">The URIs that identify the associated application.</span></span> <span data-ttu-id="73f54-191">Weitere Informationen finden Sie unter [Anwendungsobjekte und Dienstprinzipalobjekte](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span><span class="sxs-lookup"><span data-stu-id="73f54-191">For more information see, [Application Objects and Service Principal Objects](https://msdn.microsoft.com/library/azure/dn132633.aspx).</span></span>                            <span data-ttu-id="73f54-192">**Notes**: keine Nullwerte zulassen der **any** -Operator ist erforderlich für Filterausdrücke auf mehrwertige Eigenschaften; Weitere Informationen finden Sie unter [unterstützte Abfragen, Filter, und Paging-Optionen](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span><span class="sxs-lookup"><span data-stu-id="73f54-192">**Notes**: not nullable, the **any** operator is required for filter expressions on multi-valued properties; for more information, see [Supported Queries, Filters, and Paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).</span></span>            |
|<span data-ttu-id="73f54-193">tags</span><span class="sxs-lookup"><span data-stu-id="73f54-193">tags</span></span>|<span data-ttu-id="73f54-194">String</span><span class="sxs-lookup"><span data-stu-id="73f54-194">String</span></span>|                                        <span data-ttu-id="73f54-195">**Hinweis:** Lässt keine Nullwerte zu.</span><span class="sxs-lookup"><span data-stu-id="73f54-195">**Notes**: not nullable.</span></span>            |

## <a name="response"></a><span data-ttu-id="73f54-196">Antwort</span><span class="sxs-lookup"><span data-stu-id="73f54-196">Response</span></span>

<span data-ttu-id="73f54-197">Wenn der Vorgang erfolgreich war, gibt diese Methode einen `200 OK` Antwortcode und aktualisierte [ServicePrincipal](../resources/serviceprincipal.md) -Objekts in der Antworttext.</span><span class="sxs-lookup"><span data-stu-id="73f54-197">If successful, this method returns a `200 OK` response code and updated [servicePrincipal](../resources/serviceprincipal.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="73f54-198">Beispiel</span><span class="sxs-lookup"><span data-stu-id="73f54-198">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73f54-199">Anforderung</span><span class="sxs-lookup"><span data-stu-id="73f54-199">Request</span></span>
<span data-ttu-id="73f54-200">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="73f54-200">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="73f54-201">Antwort</span><span class="sxs-lookup"><span data-stu-id="73f54-201">Response</span></span>
<span data-ttu-id="73f54-p112">Nachfolgend sehen Sie ein Beispiel der Antwort. Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten. Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="73f54-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
