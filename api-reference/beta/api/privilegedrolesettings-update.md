---
title: PrivilegedRoleSettings aktualisieren
description: Aktualisieren Sie die rolleneinstellungen für die bestimmten Rolle-Einstellung. Ein PrivilegedRoleSettings-Objekt wird zurückgegeben.
localization_priority: Normal
ms.openlocfilehash: 09464c878c76ed557f30d0eac21e0572fae05062
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641120"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="2c015-104">PrivilegedRoleSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="2c015-104">Update privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c015-105">Aktualisieren Sie die rolleneinstellungen für die bestimmten Rolle-Einstellung.</span><span class="sxs-lookup"><span data-stu-id="2c015-105">Update the role settings for the given role setting.</span></span> <span data-ttu-id="2c015-106">Ein [PrivilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekt wird zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2c015-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c015-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="2c015-107">Permissions</span></span>

<span data-ttu-id="2c015-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c015-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="2c015-110">**Hinweis:** Die anfordernde Person muss eines der folgenden Rollen haben: berechtigten Rolle Administrators, globaler Administrator, Sicherheitsadministrator oder Sicherheit Leser.</span><span class="sxs-lookup"><span data-stu-id="2c015-110">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="2c015-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="2c015-111">Permission type</span></span>      | <span data-ttu-id="2c015-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="2c015-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c015-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="2c015-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2c015-114">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2c015-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2c015-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="2c015-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c015-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2c015-116">Not supported.</span></span>    |
|<span data-ttu-id="2c015-117">Application</span><span class="sxs-lookup"><span data-stu-id="2c015-117">Application</span></span> | <span data-ttu-id="2c015-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="2c015-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c015-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c015-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="2c015-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="2c015-120">Request headers</span></span>
| <span data-ttu-id="2c015-121">Name</span><span class="sxs-lookup"><span data-stu-id="2c015-121">Name</span></span>      |<span data-ttu-id="2c015-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c015-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2c015-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c015-123">Authorization</span></span>  | <span data-ttu-id="2c015-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="2c015-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c015-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="2c015-126">Request body</span></span>
<span data-ttu-id="2c015-127">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [PrivilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="2c015-127">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="2c015-128">Die folgende Tabelle enthält die Eigenschaften, die Sie angeben können, wenn Sie eine Einstellung für die Rolle aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="2c015-128">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="2c015-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="2c015-129">Property</span></span>|<span data-ttu-id="2c015-130">Typ</span><span class="sxs-lookup"><span data-stu-id="2c015-130">Type</span></span>|<span data-ttu-id="2c015-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="2c015-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c015-132">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="2c015-132">elevationDuration</span></span>|<span data-ttu-id="2c015-133">duration</span><span class="sxs-lookup"><span data-stu-id="2c015-133">duration</span></span>|<span data-ttu-id="2c015-134">Die Dauer, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="2c015-134">The duration when the role is activated.</span></span> <span data-ttu-id="2c015-135">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2c015-135">Required.</span></span>|
|<span data-ttu-id="2c015-136">id</span><span class="sxs-lookup"><span data-stu-id="2c015-136">id</span></span>|<span data-ttu-id="2c015-137">string</span><span class="sxs-lookup"><span data-stu-id="2c015-137">string</span></span>|<span data-ttu-id="2c015-138">Der eindeutige Bezeichner für die rolleneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="2c015-138">The unique identifier for the role settings.</span></span> <span data-ttu-id="2c015-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="2c015-139">Read-only.</span></span> <span data-ttu-id="2c015-140">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2c015-140">Required.</span></span>|
|<span data-ttu-id="2c015-141">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="2c015-141">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="2c015-142">Boolescher Wert</span><span class="sxs-lookup"><span data-stu-id="2c015-142">boolean</span></span>|<span data-ttu-id="2c015-143">**true,** Wenn MfaOnElevation konfigurierbar ist.</span><span class="sxs-lookup"><span data-stu-id="2c015-143">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="2c015-144">**false,** Wenn MfaOnElevation nicht konfigurierbar ist.</span><span class="sxs-lookup"><span data-stu-id="2c015-144">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="2c015-145">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2c015-145">Required.</span></span>|
|<span data-ttu-id="2c015-146">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="2c015-146">lastGlobalAdmin</span></span>|<span data-ttu-id="2c015-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c015-147">Boolean</span></span>|<span data-ttu-id="2c015-148">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="2c015-148">For internal use only.</span></span>|
|<span data-ttu-id="2c015-149">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="2c015-149">maxElavationDuration</span></span>|<span data-ttu-id="2c015-150">duration</span><span class="sxs-lookup"><span data-stu-id="2c015-150">duration</span></span>|<span data-ttu-id="2c015-151">Maximale Speicherdauer für die aktivierte Rolle.</span><span class="sxs-lookup"><span data-stu-id="2c015-151">Maximum duration for the activated role.</span></span> <span data-ttu-id="2c015-152">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2c015-152">Required.</span></span>|
|<span data-ttu-id="2c015-153">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="2c015-153">mfaOnElevation</span></span>|<span data-ttu-id="2c015-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c015-154">Boolean</span></span>|<span data-ttu-id="2c015-155">**true,** Wenn mehrstufiger Authentifizierung das erforderlich ist, um die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="2c015-155">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="2c015-156">**false,** Wenn mehrstufiger Authentifizierung das nicht erforderlich ist, um die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="2c015-156">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="2c015-157">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2c015-157">Required.</span></span>|
|<span data-ttu-id="2c015-158">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="2c015-158">minElevationDuration</span></span>|<span data-ttu-id="2c015-159">duration</span><span class="sxs-lookup"><span data-stu-id="2c015-159">duration</span></span>|<span data-ttu-id="2c015-160">Minimale Dauer für die aktivierte Rolle.</span><span class="sxs-lookup"><span data-stu-id="2c015-160">Minimum duration for the activated role.</span></span> <span data-ttu-id="2c015-161">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2c015-161">Required.</span></span>|
|<span data-ttu-id="2c015-162">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="2c015-162">notificationToUserOnElevation</span></span>|<span data-ttu-id="2c015-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c015-163">Boolean</span></span>|<span data-ttu-id="2c015-164">**true,** Wenn für den Endbenutzer Benachrichtigung senden, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="2c015-164">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="2c015-165">**false,** Wenn keine Benachrichtigung senden, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="2c015-165">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="2c015-166">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2c015-166">Required.</span></span>|
|<span data-ttu-id="2c015-167">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="2c015-167">ticketingInfoOnElevation</span></span>|<span data-ttu-id="2c015-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c015-168">Boolean</span></span>|<span data-ttu-id="2c015-169">**true,** Wenn die Informationen zur erforderlichen wann ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="2c015-169">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="2c015-170">**false,** Wenn die Informationen zur nicht erforderlich bei ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="2c015-170">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="2c015-171">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2c015-171">Required.</span></span>|
|<span data-ttu-id="2c015-172">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="2c015-172">approvalOnElevation</span></span>|<span data-ttu-id="2c015-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="2c015-173">Boolean</span></span>|<span data-ttu-id="2c015-174">**true,** Wenn die Genehmigung erforderlich wann ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="2c015-174">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="2c015-175">**false,** Wenn die Genehmigung ist nicht erforderlich bei die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="2c015-175">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="2c015-176">Erforderlich. </span><span class="sxs-lookup"><span data-stu-id="2c015-176">Required.</span></span>|
|<span data-ttu-id="2c015-177">approverIds</span><span class="sxs-lookup"><span data-stu-id="2c015-177">approverIds</span></span>|<span data-ttu-id="2c015-178">Array</span><span class="sxs-lookup"><span data-stu-id="2c015-178">array</span></span>|<span data-ttu-id="2c015-179">Liste der Genehmigung-IDs, wenn die Genehmigung für die Aktivierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="2c015-179">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="2c015-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c015-180">Response</span></span>

<span data-ttu-id="2c015-181">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="2c015-181">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="2c015-182">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="2c015-182">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="2c015-183">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="2c015-183">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="2c015-184">Beispiel</span><span class="sxs-lookup"><span data-stu-id="2c015-184">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2c015-185">Anforderung</span><span class="sxs-lookup"><span data-stu-id="2c015-185">Request</span></span>
<span data-ttu-id="2c015-186">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="2c015-186">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "put_privilegedrolesettings"
}-->
```http
PUT https://graph.microsoft.com/beta/privilegedRoles/{id}/settings
Content-type: application/json

{
    "id": "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3",
    "elevationDuration": "PT8H",
    "notificationToUserOnElevation": false,
    "ticketingInfoOnElevation": true,
    "mfaOnElevation": false,
    "maxElavationDuration": "PT0S",
    "minElevationDuration": "PT0S",
    "lastGlobalAdmin": false,
    "isMfaOnElevationConfigurable": true,
    "approvalOnElevation": false,
    "approverIds": ["e2b2a2fb-13d7-495c-adc9-941fe966793f", "22770e3f-b9b4-418e-9dea-d0e3d2f275dd"]
}
```
##### <a name="response"></a><span data-ttu-id="2c015-187">Antwort</span><span class="sxs-lookup"><span data-stu-id="2c015-187">Response</span></span>
<span data-ttu-id="2c015-188">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="2c015-188">Here is an example of the response.</span></span>

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrolesettings-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
