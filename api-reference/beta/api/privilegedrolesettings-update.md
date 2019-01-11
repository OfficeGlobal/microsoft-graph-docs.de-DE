---
title: PrivilegedRoleSettings aktualisieren
description: Aktualisieren Sie die rolleneinstellungen für die bestimmten Rolle-Einstellung. Ein PrivilegedRoleSettings-Objekt wird zurückgegeben.
localization_priority: Normal
ms.openlocfilehash: 7c117abfe774eae60e42dcbc5f748c10cacf5cd6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819317"
---
# <a name="update-privilegedrolesettings"></a><span data-ttu-id="6a6ad-104">PrivilegedRoleSettings aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6a6ad-104">Update privilegedRoleSettings</span></span>

> <span data-ttu-id="6a6ad-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a6ad-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a6ad-107">Aktualisieren Sie die rolleneinstellungen für die bestimmten Rolle-Einstellung.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-107">Update the role settings for the given role setting.</span></span> <span data-ttu-id="6a6ad-108">Ein [PrivilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekt wird zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-108">A [privilegedRoleSettings](../resources/privilegedrolesettings.md) object will be returned.</span></span>
## <a name="permissions"></a><span data-ttu-id="6a6ad-109">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="6a6ad-109">Permissions</span></span>

<span data-ttu-id="6a6ad-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a6ad-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="6a6ad-112">**Hinweis:** Die anfordernde Person muss eines der folgenden Rollen haben: berechtigten Rolle Administrators, globaler Administrator, Sicherheitsadministrator oder Sicherheit Leser.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-112">**Note:** The requester must have one of the following roles: Privileged Role Administrator, Global Administrator, Security Administrator, or Security Reader.</span></span> 

|<span data-ttu-id="6a6ad-113">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="6a6ad-113">Permission type</span></span>      | <span data-ttu-id="6a6ad-114">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="6a6ad-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a6ad-115">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="6a6ad-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6a6ad-116">PrivilegedAccess.ReadWrite.AzureAD Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a6ad-116">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a6ad-117">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="6a6ad-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a6ad-118">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a6ad-118">Not supported.</span></span>    |
|<span data-ttu-id="6a6ad-119">Anwendung</span><span class="sxs-lookup"><span data-stu-id="6a6ad-119">Application</span></span> | <span data-ttu-id="6a6ad-120">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="6a6ad-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a6ad-121">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a6ad-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /privilegedRoles/{id}/settings
```

## <a name="request-headers"></a><span data-ttu-id="6a6ad-122">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="6a6ad-122">Request headers</span></span>
| <span data-ttu-id="6a6ad-123">Name</span><span class="sxs-lookup"><span data-stu-id="6a6ad-123">Name</span></span>      |<span data-ttu-id="6a6ad-124">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a6ad-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a6ad-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a6ad-125">Authorization</span></span>  | <span data-ttu-id="6a6ad-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a6ad-128">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="6a6ad-128">Request body</span></span>
<span data-ttu-id="6a6ad-129">Geben Sie im Textkörper Anforderung eine JSON-Darstellung eines [PrivilegedRoleSettings](../resources/privilegedrolesettings.md) -Objekts.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-129">In the request body, supply a JSON representation of a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.</span></span>

<span data-ttu-id="6a6ad-130">Die folgende Tabelle enthält die Eigenschaften, die Sie angeben können, wenn Sie eine Einstellung für die Rolle aktualisieren.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-130">The following table lists the properties that you can supply when you update a role setting.</span></span>

|<span data-ttu-id="6a6ad-131">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="6a6ad-131">Property</span></span>|<span data-ttu-id="6a6ad-132">Typ</span><span class="sxs-lookup"><span data-stu-id="6a6ad-132">Type</span></span>|<span data-ttu-id="6a6ad-133">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="6a6ad-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a6ad-134">elevationDuration</span><span class="sxs-lookup"><span data-stu-id="6a6ad-134">elevationDuration</span></span>|<span data-ttu-id="6a6ad-135">duration</span><span class="sxs-lookup"><span data-stu-id="6a6ad-135">duration</span></span>|<span data-ttu-id="6a6ad-136">Die Dauer, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-136">The duration when the role is activated.</span></span> <span data-ttu-id="6a6ad-137">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-137">Required.</span></span>|
|<span data-ttu-id="6a6ad-138">id</span><span class="sxs-lookup"><span data-stu-id="6a6ad-138">id</span></span>|<span data-ttu-id="6a6ad-139">string</span><span class="sxs-lookup"><span data-stu-id="6a6ad-139">string</span></span>|<span data-ttu-id="6a6ad-140">Der eindeutige Bezeichner für die rolleneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-140">The unique identifier for the role settings.</span></span> <span data-ttu-id="6a6ad-141">Schreibgeschützt.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-141">Read-only.</span></span> <span data-ttu-id="6a6ad-142">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-142">Required.</span></span>|
|<span data-ttu-id="6a6ad-143">isMfaOnElevationConfigurable</span><span class="sxs-lookup"><span data-stu-id="6a6ad-143">isMfaOnElevationConfigurable</span></span>|<span data-ttu-id="6a6ad-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a6ad-144">boolean</span></span>|<span data-ttu-id="6a6ad-145">**true,** Wenn MfaOnElevation konfigurierbar ist.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-145">**true** if mfaOnElevation is configurable.</span></span> <span data-ttu-id="6a6ad-146">**false,** Wenn MfaOnElevation nicht konfigurierbar ist.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-146">**false** if mfaOnElevation is not configurable.</span></span> <span data-ttu-id="6a6ad-147">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-147">Required.</span></span>|
|<span data-ttu-id="6a6ad-148">lastGlobalAdmin</span><span class="sxs-lookup"><span data-stu-id="6a6ad-148">lastGlobalAdmin</span></span>|<span data-ttu-id="6a6ad-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a6ad-149">Boolean</span></span>|<span data-ttu-id="6a6ad-150">Nur für internen Gebrauch.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-150">For internal use only.</span></span>|
|<span data-ttu-id="6a6ad-151">maxElavationDuration</span><span class="sxs-lookup"><span data-stu-id="6a6ad-151">maxElavationDuration</span></span>|<span data-ttu-id="6a6ad-152">duration</span><span class="sxs-lookup"><span data-stu-id="6a6ad-152">duration</span></span>|<span data-ttu-id="6a6ad-153">Maximale Speicherdauer für die aktivierte Rolle.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-153">Maximum duration for the activated role.</span></span> <span data-ttu-id="6a6ad-154">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-154">Required.</span></span>|
|<span data-ttu-id="6a6ad-155">mfaOnElevation</span><span class="sxs-lookup"><span data-stu-id="6a6ad-155">mfaOnElevation</span></span>|<span data-ttu-id="6a6ad-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a6ad-156">Boolean</span></span>|<span data-ttu-id="6a6ad-157">**true,** Wenn mehrstufiger Authentifizierung das erforderlich ist, um die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-157">**true** if MFA is required to activate the role.</span></span> <span data-ttu-id="6a6ad-158">**false,** Wenn mehrstufiger Authentifizierung das nicht erforderlich ist, um die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-158">**false** if MFA is not required to activate the role.</span></span> <span data-ttu-id="6a6ad-159">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-159">Required.</span></span>|
|<span data-ttu-id="6a6ad-160">minElevationDuration</span><span class="sxs-lookup"><span data-stu-id="6a6ad-160">minElevationDuration</span></span>|<span data-ttu-id="6a6ad-161">duration</span><span class="sxs-lookup"><span data-stu-id="6a6ad-161">duration</span></span>|<span data-ttu-id="6a6ad-162">Minimale Dauer für die aktivierte Rolle.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-162">Minimum duration for the activated role.</span></span> <span data-ttu-id="6a6ad-163">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-163">Required.</span></span>|
|<span data-ttu-id="6a6ad-164">notificationToUserOnElevation</span><span class="sxs-lookup"><span data-stu-id="6a6ad-164">notificationToUserOnElevation</span></span>|<span data-ttu-id="6a6ad-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a6ad-165">Boolean</span></span>|<span data-ttu-id="6a6ad-166">**true,** Wenn für den Endbenutzer Benachrichtigung senden, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-166">**true** if send notification to the end user when the role is activated.</span></span> <span data-ttu-id="6a6ad-167">**false,** Wenn keine Benachrichtigung senden, wenn die Rolle aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-167">**false** if do not send notification when the role is activated.</span></span> <span data-ttu-id="6a6ad-168">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-168">Required.</span></span>|
|<span data-ttu-id="6a6ad-169">ticketingInfoOnElevation</span><span class="sxs-lookup"><span data-stu-id="6a6ad-169">ticketingInfoOnElevation</span></span>|<span data-ttu-id="6a6ad-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a6ad-170">Boolean</span></span>|<span data-ttu-id="6a6ad-171">**true,** Wenn die Informationen zur erforderlichen wann ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-171">**true** if the ticketing information is required when activate the role.</span></span> <span data-ttu-id="6a6ad-172">**false,** Wenn die Informationen zur nicht erforderlich bei ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-172">**false** if the ticketing information is not required when activate the role.</span></span> <span data-ttu-id="6a6ad-173">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-173">Required.</span></span>|
|<span data-ttu-id="6a6ad-174">approvalOnElevation</span><span class="sxs-lookup"><span data-stu-id="6a6ad-174">approvalOnElevation</span></span>|<span data-ttu-id="6a6ad-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a6ad-175">Boolean</span></span>|<span data-ttu-id="6a6ad-176">**true,** Wenn die Genehmigung erforderlich wann ist die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-176">**true** if the approval is required when activate the role.</span></span> <span data-ttu-id="6a6ad-177">**false,** Wenn die Genehmigung ist nicht erforderlich bei die Rolle zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-177">**false** if the approval is not required when activate the role.</span></span> <span data-ttu-id="6a6ad-178">Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-178">Required.</span></span>|
|<span data-ttu-id="6a6ad-179">approverIds</span><span class="sxs-lookup"><span data-stu-id="6a6ad-179">approverIds</span></span>|<span data-ttu-id="6a6ad-180">Array</span><span class="sxs-lookup"><span data-stu-id="6a6ad-180">array</span></span>|<span data-ttu-id="6a6ad-181">Liste der Genehmigung-IDs, wenn die Genehmigung für die Aktivierung erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-181">List of Approval IDs, if approval is required for activation.</span></span>|

## <a name="response"></a><span data-ttu-id="6a6ad-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a6ad-182">Response</span></span>

<span data-ttu-id="6a6ad-183">Wenn die Methode erfolgreich verläuft, wird der Antwortcode `204 No Content` zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-183">If successful, this method returns a `204 No Content` response code.</span></span>

<span data-ttu-id="6a6ad-184">Beachten Sie, dass der Mandant muss auf den PIM registriert werden.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-184">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6a6ad-185">Andernfalls wird der Statuscode HTTP 403 Verboten zurückgegeben werden soll.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-185">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="6a6ad-186">Beispiel</span><span class="sxs-lookup"><span data-stu-id="6a6ad-186">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a6ad-187">Anforderung</span><span class="sxs-lookup"><span data-stu-id="6a6ad-187">Request</span></span>
<span data-ttu-id="6a6ad-188">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-188">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6a6ad-189">Antwort</span><span class="sxs-lookup"><span data-stu-id="6a6ad-189">Response</span></span>
<span data-ttu-id="6a6ad-190">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="6a6ad-190">Here is an example of the response.</span></span>

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update privilegedRoleSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
