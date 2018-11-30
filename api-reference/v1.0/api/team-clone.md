---
title: Klonen Sie ein team
description: Erstellen Sie eine Kopie eines Teams. Dieser Vorgang wird außerdem eine Kopie der entsprechenden Gruppe erstellt.
ms.openlocfilehash: 8cd6c580db9aa77f87a31bdb9b2878ed9e580e61
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/29/2018
ms.locfileid: "27016482"
---
# <a name="clone-a-team"></a><span data-ttu-id="1afff-104">Klonen Sie ein team</span><span class="sxs-lookup"><span data-stu-id="1afff-104">Clone a team</span></span>



<span data-ttu-id="1afff-105">Erstellen Sie eine Kopie eines [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="1afff-105">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="1afff-106">Dieser Vorgang wird außerdem eine Kopie der entsprechenden [Gruppe](../resources/group.md)erstellt.</span><span class="sxs-lookup"><span data-stu-id="1afff-106">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="1afff-107">Sie können die Teile des Teams Klonen angeben:</span><span class="sxs-lookup"><span data-stu-id="1afff-107">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="1afff-108">**apps** – Microsoft-Teams, Kopien apps, die im Team installiert sind.</span><span class="sxs-lookup"><span data-stu-id="1afff-108">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="1afff-109">**Kanäle** – kopiert die Struktur DDE-Kanal (jedoch nicht die Nachrichten im Kanal).</span><span class="sxs-lookup"><span data-stu-id="1afff-109">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="1afff-110">**Elemente des Objekts** – kopiert die Mitglieder und Besitzer der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="1afff-110">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="1afff-111">**Einstellungen** – kopiert alle Einstellungen im Team, zusammen mit den wichtigsten gruppeneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="1afff-111">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="1afff-112">**Registerkarten** – kopiert die Registerkarten in den Kanälen.</span><span class="sxs-lookup"><span data-stu-id="1afff-112">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="1afff-113">Wenn Registerkarten geklont werden, in einen nicht konfigurierten Status zugeführt werden – auf der Registerleiste in Microsoft-Teams angezeigt werden, und beim ersten Öffnen, werden über den Konfigurationsbildschirm wechseln.</span><span class="sxs-lookup"><span data-stu-id="1afff-113">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="1afff-114">(Wenn die Person, die beim Öffnen der Registerkarte keinen Berechtigung zum Konfigurieren von apps, sehen sie eine Meldung angezeigt, dass die Registerkarte nicht konfiguriert wurde.)</span><span class="sxs-lookup"><span data-stu-id="1afff-114">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="1afff-115">Klonen ist ein zeitintensiver Vorgang.</span><span class="sxs-lookup"><span data-stu-id="1afff-115">Cloning is a long-running operation.</span></span>
<span data-ttu-id="1afff-116">Nachdem der POST-Klon zurückgegeben wird, müssen Sie den [Vorgang](../resources/teamsasyncoperation.md) abrufen, um festzustellen, ob es sich um "ausführen" oder "erfolgreich" oder "Fehler" ist.</span><span class="sxs-lookup"><span data-stu-id="1afff-116">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="1afff-117">Sie sollten zu berechnen fortfahren, bis der Status nicht "aktiv" ist.</span><span class="sxs-lookup"><span data-stu-id="1afff-117">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="1afff-118">Die empfohlene Verzögerung zwischen ruft beträgt 5 Sekunden.</span><span class="sxs-lookup"><span data-stu-id="1afff-118">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="1afff-119">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="1afff-119">Permissions</span></span>

<span data-ttu-id="1afff-p105">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1afff-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1afff-122">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="1afff-122">Permission type</span></span>      | <span data-ttu-id="1afff-123">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="1afff-123">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1afff-124">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="1afff-124">Delegated (work or school account)</span></span>     | <span data-ttu-id="1afff-125">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1afff-125">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="1afff-126">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="1afff-126">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1afff-127">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="1afff-127">Not supported.</span></span>    |
|<span data-ttu-id="1afff-128">Anwendung</span><span class="sxs-lookup"><span data-stu-id="1afff-128">Application</span></span>                            | <span data-ttu-id="1afff-129">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1afff-129">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1afff-130">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="1afff-130">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="1afff-131">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="1afff-131">Request headers</span></span>
| <span data-ttu-id="1afff-132">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="1afff-132">Header</span></span>       | <span data-ttu-id="1afff-133">Wert</span><span class="sxs-lookup"><span data-stu-id="1afff-133">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1afff-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="1afff-134">Authorization</span></span>  | <span data-ttu-id="1afff-p106">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="1afff-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1afff-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1afff-137">Content-Type</span></span>  | <span data-ttu-id="1afff-138">application/json</span><span class="sxs-lookup"><span data-stu-id="1afff-138">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1afff-139">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="1afff-139">Request body</span></span>

| <span data-ttu-id="1afff-140">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="1afff-140">Property</span></span>     | <span data-ttu-id="1afff-141">Typ</span><span class="sxs-lookup"><span data-stu-id="1afff-141">Type</span></span>   |<span data-ttu-id="1afff-142">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="1afff-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1afff-143">Klassifikation</span><span class="sxs-lookup"><span data-stu-id="1afff-143">classification</span></span>|<span data-ttu-id="1afff-144">Zeichenfolge (optional)</span><span class="sxs-lookup"><span data-stu-id="1afff-144">String (optional)</span></span>|<span data-ttu-id="1afff-145">Beschreibt eine Klassifizierung für die Gruppe (z. B. niedrig, Mittel oder hoch geschäftliche Relevanz).</span><span class="sxs-lookup"><span data-stu-id="1afff-145">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="1afff-146">Wenn Klassifizierung nicht angegeben ist, wird die Klassifizierung aus der ursprünglichen Team-Gruppe kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="1afff-146">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="1afff-147">description</span><span class="sxs-lookup"><span data-stu-id="1afff-147">description</span></span>|<span data-ttu-id="1afff-148">Zeichenfolge (optional)</span><span class="sxs-lookup"><span data-stu-id="1afff-148">String (optional)</span></span>|<span data-ttu-id="1afff-149">Eine optionale Beschreibung für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="1afff-149">An optional description for the group.</span></span> <span data-ttu-id="1afff-150">Wenn diese Eigenschaft nicht angegeben ist, wird es leer sein.</span><span class="sxs-lookup"><span data-stu-id="1afff-150">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="1afff-151">displayName</span><span class="sxs-lookup"><span data-stu-id="1afff-151">displayName</span></span>|<span data-ttu-id="1afff-152">String</span><span class="sxs-lookup"><span data-stu-id="1afff-152">String</span></span>|<span data-ttu-id="1afff-p109">Der Anzeigename der Gruppe. Diese Eigenschaft ist beim Erstellen einer Gruppe erforderlich und kann bei Updates nicht deaktiviert werden. Unterstützt $Filter und $orderby.</span><span class="sxs-lookup"><span data-stu-id="1afff-p109">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="1afff-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="1afff-156">mailNickname</span></span>|<span data-ttu-id="1afff-157">String</span><span class="sxs-lookup"><span data-stu-id="1afff-157">String</span></span>|<span data-ttu-id="1afff-158">Der e-Mail-Alias für die Gruppe, die in der Organisation eindeutig.</span><span class="sxs-lookup"><span data-stu-id="1afff-158">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="1afff-159">Diese Eigenschaft muss angegeben werden, wenn eine Gruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="1afff-159">This property must be specified when a group is created.</span></span> <span data-ttu-id="1afff-160">Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="1afff-160">Supports $filter.</span></span> <span data-ttu-id="1afff-161">Wenn diese Eigenschaft nicht angegeben ist, wird er von der DisplayName berechnet.</span><span class="sxs-lookup"><span data-stu-id="1afff-161">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="1afff-162">Bekanntes Problem: Diese Eigenschaft wird zurzeit ignoriert.</span><span class="sxs-lookup"><span data-stu-id="1afff-162">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="1afff-163">partsToClone</span><span class="sxs-lookup"><span data-stu-id="1afff-163">partsToClone</span></span>| [<span data-ttu-id="1afff-164">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="1afff-164">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="1afff-165">Eine durch Trennzeichen getrennte Liste der Teile zum Klonen.</span><span class="sxs-lookup"><span data-stu-id="1afff-165">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="1afff-166">Rechtliche Webparts sind "apps, Registerkarten, Einstellungen, Kanäle, Mitglieder".</span><span class="sxs-lookup"><span data-stu-id="1afff-166">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="1afff-167">visibility</span><span class="sxs-lookup"><span data-stu-id="1afff-167">visibility</span></span>|<span data-ttu-id="1afff-168">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span><span class="sxs-lookup"><span data-stu-id="1afff-168">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="1afff-169">Gibt die Sichtbarkeit der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="1afff-169">Specifies the visibility of the group.</span></span> <span data-ttu-id="1afff-170">Mögliche Werte sind: **Private**, **Public**.</span><span class="sxs-lookup"><span data-stu-id="1afff-170">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="1afff-171">Wenn die Sichtbarkeit nicht angegeben wird, werden die Sichtbarkeit aus der ursprünglichen Team-Gruppe kopiert.</span><span class="sxs-lookup"><span data-stu-id="1afff-171">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="1afff-172">Wenn das Team geklont wird ist ein **EducationClass** Team der Sichtbarkeit-Parameter wird ignoriert und Sichtbarkeit für die neue Gruppe wird auf HiddenMembership festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="1afff-172">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="1afff-173">Antwort</span><span class="sxs-lookup"><span data-stu-id="1afff-173">Response</span></span>

<span data-ttu-id="1afff-174">Wenn erfolgreich, mit dieser Methode zurückgegeben wird eine `202 Accepted` Antwortcode mit einem Standortprofil: Verweisen auf die Ressource [Vorgang](../resources/teamsasyncoperation.md) Kopfzeile.</span><span class="sxs-lookup"><span data-stu-id="1afff-174">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="1afff-175">Wenn der Vorgang abgeschlossen ist, wird die Vorgang Ressource die Id des erstellten Teams informieren.</span><span class="sxs-lookup"><span data-stu-id="1afff-175">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="1afff-176">Beispiel</span><span class="sxs-lookup"><span data-stu-id="1afff-176">Example</span></span>
#### <a name="request"></a><span data-ttu-id="1afff-177">Anforderung</span><span class="sxs-lookup"><span data-stu-id="1afff-177">Request</span></span>
<span data-ttu-id="1afff-178">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="1afff-178">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_team"
}-->
```http
POST /teams/{id}/clone
Content-Type: application/json

{  
     "displayName": "Library Assist",
     "description": "Self help community for library",
     "mailNickname": "libassist",
     "partsToClone": "apps,tabs,settings,channels,members",
     "visibility": "public"
}
```

#### <a name="response"></a><span data-ttu-id="1afff-179">Antwort</span><span class="sxs-lookup"><span data-stu-id="1afff-179">Response</span></span>
<span data-ttu-id="1afff-180">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="1afff-180">The following is an example of the response.</span></span> <span data-ttu-id="1afff-181">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="1afff-181">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="1afff-182">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="1afff-182">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
