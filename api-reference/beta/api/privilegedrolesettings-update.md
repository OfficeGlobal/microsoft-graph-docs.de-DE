---
title: PrivilegedRoleSettings aktualisieren
description: Aktualisieren Sie die Rolleneinstellungen für die angegebene Rollen Einstellung. Ein privilegedRoleSettings-Objekt wird zurückgegeben.
localization_priority: Normal
ms.openlocfilehash: f416656362c5be0ccdaa2b3aaa7812511e357875
ms.sourcegitcommit: 3615f9475d57bfbb3a8c4402af863897f592dfbd
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2019
ms.locfileid: "30789606"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="236f3-104">PrivilegedRoleSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="236f3-104">Update privilegedRoleSettings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="236f3-105">Aktualisieren Sie die Rolleneinstellungen für die angegebene Rollen Einstellung.</span><span class="sxs-lookup"><span data-stu-id="236f3-105">Update the role settings for the given role setting.</span></span> <span data-ttu-id="236f3-106">Ein [privilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekt wird zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="236f3-106">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="236f3-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="236f3-107">Permissions</span></span>

<span data-ttu-id="236f3-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="236f3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="236f3-110">**Hinweis:** Der anfordernde muss eine der folgenden Rollen besitzen: Administrator für privilegierte Rollen, globaler Administrator, Sicherheitsadministrator oder Sicherheits Leser.</span><span class="sxs-lookup"><span data-stu-id="236f3-110">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="236f3-111">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="236f3-111">Permission type</span></span>      | <span data-ttu-id="236f3-112">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="236f3-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="236f3-113">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="236f3-113">Delegated (work or school account)</span></span> | <span data-ttu-id="236f3-114">PrivilegedAccess. ReadWrite. AzureAD, Directory. AccessAsUser. all</span><span class="sxs-lookup"><span data-stu-id="236f3-114">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="236f3-115">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="236f3-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="236f3-116">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="236f3-116">Not supported.</span></span>    |
|<span data-ttu-id="236f3-117">Anwendung</span><span class="sxs-lookup"><span data-stu-id="236f3-117">Application</span></span> | <span data-ttu-id="236f3-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="236f3-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="236f3-119">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="236f3-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="236f3-120">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="236f3-120">Request headers</span></span>
| <span data-ttu-id="236f3-121">Name</span><span class="sxs-lookup"><span data-stu-id="236f3-121">Name</span></span>      |<span data-ttu-id="236f3-122">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="236f3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="236f3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="236f3-123">Authorization</span></span>  | <span data-ttu-id="236f3-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="236f3-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="236f3-126">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="236f3-126">Request body</span></span>
<span data-ttu-id="236f3-127">Geben Sie im Anforderungstext eine JSON-Darstellung eines [privilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekts an.</span><span class="sxs-lookup"><span data-stu-id="236f3-127">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="236f3-128">In der folgenden Tabelle sind die Eigenschaften aufgeführt, die Sie beim Aktualisieren einer Rollen Einstellung angeben können.</span><span class="sxs-lookup"><span data-stu-id="236f3-128">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="236f3-129">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="236f3-129">Property</span></span>|<span data-ttu-id="236f3-130">Typ</span><span class="sxs-lookup"><span data-stu-id="236f3-130">Type</span></span>|<span data-ttu-id="236f3-131">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="236f3-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="236f3-132">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="236f3-132">elevationDuration</span></span>|<span data-ttu-id="236f3-133">duration</span><span class="sxs-lookup"><span data-stu-id="236f3-133">duration</span></span>|<span data-ttu-id="236f3-134">Die Dauer der Aktivierung der Rolle.</span><span class="sxs-lookup"><span data-stu-id="236f3-134">The duration when the role is activated.</span></span> <span data-ttu-id="236f3-135">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="236f3-135">Required.</span></span>|
|<span data-ttu-id="236f3-136">id</span><span class="sxs-lookup"><span data-stu-id="236f3-136">id</span></span>|<span data-ttu-id="236f3-137">string</span><span class="sxs-lookup"><span data-stu-id="236f3-137">string</span></span>|<span data-ttu-id="236f3-138">Der eindeutige Bezeichner für die Rolleneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="236f3-138">The unique identifier for the role settings.</span></span> <span data-ttu-id="236f3-139">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="236f3-139">Read-only.</span></span> <span data-ttu-id="236f3-140">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="236f3-140">Required.</span></span>|
|<span data-ttu-id="236f3-141">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="236f3-141">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="236f3-142">Boolesch</span><span class="sxs-lookup"><span data-stu-id="236f3-142">boolean</span></span>|<span data-ttu-id="236f3-143">**true** , wenn mfaOnElevation ist konfigurierbar.</span><span class="sxs-lookup"><span data-stu-id="236f3-143">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="236f3-144">**false** , wenn mfaOnElevation nicht konfigurierbar ist.</span><span class="sxs-lookup"><span data-stu-id="236f3-144">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="236f3-145">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="236f3-145">Required.</span></span>|
|<span data-ttu-id="236f3-146">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="236f3-146">lastGlobalAdmin</span></span>|<span data-ttu-id="236f3-147">Boolesch</span><span class="sxs-lookup"><span data-stu-id="236f3-147">Boolean</span></span>|<span data-ttu-id="236f3-148">Ausschließlich für interne Zwecke.</span><span class="sxs-lookup"><span data-stu-id="236f3-148">For internal use only.</span></span>|
|<span data-ttu-id="236f3-149">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="236f3-149">maxElavationDuration</span></span>|<span data-ttu-id="236f3-150">duration</span><span class="sxs-lookup"><span data-stu-id="236f3-150">duration</span></span>|<span data-ttu-id="236f3-151">Maximale Dauer der aktivierten Rolle.</span><span class="sxs-lookup"><span data-stu-id="236f3-151">Maximum duration for the activated role.</span></span> <span data-ttu-id="236f3-152">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="236f3-152">Required.</span></span>|
|<span data-ttu-id="236f3-153">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="236f3-153">mfaOnElevation</span></span>|<span data-ttu-id="236f3-154">Boolesch</span><span class="sxs-lookup"><span data-stu-id="236f3-154">Boolean</span></span>|<span data-ttu-id="236f3-155">**true** , wenn MFA erforderlich ist, um die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="236f3-155">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="236f3-156">**false** , wenn MFA nicht erforderlich ist, um die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="236f3-156">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="236f3-157">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="236f3-157">Required.</span></span>|
|<span data-ttu-id="236f3-158">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="236f3-158">minElevationDuration</span></span>|<span data-ttu-id="236f3-159">duration</span><span class="sxs-lookup"><span data-stu-id="236f3-159">duration</span></span>|<span data-ttu-id="236f3-160">Mindestdauer für die aktivierte Rolle.</span><span class="sxs-lookup"><span data-stu-id="236f3-160">Minimum duration for the activated role.</span></span> <span data-ttu-id="236f3-161">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="236f3-161">Required.</span></span>|
|<span data-ttu-id="236f3-162">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="236f3-162">notificationToUserOnElevation</span></span>|<span data-ttu-id="236f3-163">Boolesch</span><span class="sxs-lookup"><span data-stu-id="236f3-163">Boolean</span></span>|<span data-ttu-id="236f3-164">**true** , wenn eine Benachrichtigung an den Endbenutzer gesendet wird, wenn die Rolle aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="236f3-164">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="236f3-165">**false** , wenn keine Benachrichtigung gesendet wird, wenn die Rolle aktiviert wird.</span><span class="sxs-lookup"><span data-stu-id="236f3-165">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="236f3-166">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="236f3-166">Required.</span></span>|
|<span data-ttu-id="236f3-167">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="236f3-167">ticketingInfoOnElevation</span></span>|<span data-ttu-id="236f3-168">Boolesch</span><span class="sxs-lookup"><span data-stu-id="236f3-168">Boolean</span></span>|<span data-ttu-id="236f3-169">**true** , wenn die Ticketing-Informationen erforderlich sind, wenn die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="236f3-169">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="236f3-170">**false** , wenn die Ticket Informationen beim Aktivieren der Rolle nicht erforderlich sind.</span><span class="sxs-lookup"><span data-stu-id="236f3-170">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="236f3-171">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="236f3-171">Required.</span></span>|
|<span data-ttu-id="236f3-172">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="236f3-172">approvalOnElevation</span></span>|<span data-ttu-id="236f3-173">Boolesch</span><span class="sxs-lookup"><span data-stu-id="236f3-173">Boolean</span></span>|<span data-ttu-id="236f3-174">**true** , wenn die Genehmigung erforderlich ist, wenn die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="236f3-174">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="236f3-175">**false** , wenn die Genehmigung nicht erforderlich ist, wenn die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="236f3-175">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="236f3-176">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="236f3-176">Required.</span></span>|
|<span data-ttu-id="236f3-177">approverIds</span><span class="sxs-lookup"><span data-stu-id="236f3-177">approverIds</span></span>|<span data-ttu-id="236f3-178">String collection</span><span class="sxs-lookup"><span data-stu-id="236f3-178">String collection</span></span>|<span data-ttu-id="236f3-179">Liste der Genehmigungs-IDs, falls für die Aktivierung Genehmigung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="236f3-179">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="236f3-180">Antwort</span><span class="sxs-lookup"><span data-stu-id="236f3-180">Response</span></span>

<span data-ttu-id="236f3-181">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="236f3-181">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="236f3-182">Beachten Sie, dass der Mandant bei PIM registriert werden muss.</span><span class="sxs-lookup"><span data-stu-id="236f3-182">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="236f3-183">Andernfalls wird der vom HTTP 403 Forbidden-Statuscode zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="236f3-183">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="236f3-184">Beispiel</span><span class="sxs-lookup"><span data-stu-id="236f3-184">Example</span></span>
##### <a name="request"></a><span data-ttu-id="236f3-185">Anforderung</span><span class="sxs-lookup"><span data-stu-id="236f3-185">Request</span></span>
<span data-ttu-id="236f3-186">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="236f3-186">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="236f3-187">Antwort</span><span class="sxs-lookup"><span data-stu-id="236f3-187">Response</span></span>
<span data-ttu-id="236f3-188">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="236f3-188">Here is an example of the response.</span></span>

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
