# <a name="clone-a-team"></a><span data-ttu-id="d61c9-101">Klonen Sie ein team</span><span class="sxs-lookup"><span data-stu-id="d61c9-101">Clone a team</span></span>



<span data-ttu-id="d61c9-102">Erstellen Sie eine Kopie eines [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="d61c9-102">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="d61c9-103">Dieser Vorgang wird außerdem eine Kopie der entsprechenden [Gruppe](../resources/group.md)erstellt.</span><span class="sxs-lookup"><span data-stu-id="d61c9-103">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="d61c9-104">Sie können die Teile des Teams Klonen angeben:</span><span class="sxs-lookup"><span data-stu-id="d61c9-104">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="d61c9-105">**apps** – Microsoft-Teams, Kopien apps, die im Team installiert sind.</span><span class="sxs-lookup"><span data-stu-id="d61c9-105">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="d61c9-106">**Kanäle** – kopiert die Struktur DDE-Kanal (jedoch nicht die Nachrichten im Kanal).</span><span class="sxs-lookup"><span data-stu-id="d61c9-106">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="d61c9-107">**Elemente des Objekts** – kopiert die Mitglieder und Besitzer der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="d61c9-107">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="d61c9-108">**Einstellungen** – kopiert alle Einstellungen im Team, zusammen mit den wichtigsten gruppeneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="d61c9-108">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="d61c9-109">**Registerkarten** – kopiert die Registerkarten in den Kanälen.</span><span class="sxs-lookup"><span data-stu-id="d61c9-109">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="d61c9-110">Wenn Registerkarten geklont werden, in einen nicht konfigurierten Status zugeführt werden – auf der Registerleiste in Microsoft-Teams angezeigt werden, und beim ersten Öffnen, werden über den Konfigurationsbildschirm wechseln.</span><span class="sxs-lookup"><span data-stu-id="d61c9-110">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="d61c9-111">(Wenn die Person, die beim Öffnen der Registerkarte keinen Berechtigung zum Konfigurieren von apps, sehen sie eine Meldung angezeigt, dass die Registerkarte nicht konfiguriert wurde.)</span><span class="sxs-lookup"><span data-stu-id="d61c9-111">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="d61c9-112">Klonen ist ein zeitintensiver Vorgang.</span><span class="sxs-lookup"><span data-stu-id="d61c9-112">Cloning is a long-running operation.</span></span>
<span data-ttu-id="d61c9-113">Nachdem der POST-Klon zurückgegeben wird, müssen Sie den [Vorgang](../resources/teamsasyncoperation.md) abrufen, um festzustellen, ob es sich um "ausführen" oder "erfolgreich" oder "Fehler" ist.</span><span class="sxs-lookup"><span data-stu-id="d61c9-113">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="d61c9-114">Sie sollten zu berechnen fortfahren, bis der Status nicht "aktiv" ist.</span><span class="sxs-lookup"><span data-stu-id="d61c9-114">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="d61c9-115">Die empfohlene Verzögerung zwischen ruft beträgt 5 Sekunden.</span><span class="sxs-lookup"><span data-stu-id="d61c9-115">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="d61c9-116">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="d61c9-116">Permissions</span></span>

<span data-ttu-id="d61c9-p104">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d61c9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d61c9-119">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="d61c9-119">Permission type</span></span>      | <span data-ttu-id="d61c9-120">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="d61c9-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d61c9-121">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="d61c9-121">Delegated (work or school account)</span></span>     | <span data-ttu-id="d61c9-122">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d61c9-122">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d61c9-123">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="d61c9-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d61c9-124">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="d61c9-124">Not supported.</span></span>    |
|<span data-ttu-id="d61c9-125">Anwendung</span><span class="sxs-lookup"><span data-stu-id="d61c9-125">Application</span></span>                            | <span data-ttu-id="d61c9-126">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d61c9-126">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d61c9-127">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="d61c9-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="d61c9-128">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="d61c9-128">Request headers</span></span>
| <span data-ttu-id="d61c9-129">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="d61c9-129">Header</span></span>       | <span data-ttu-id="d61c9-130">Wert</span><span class="sxs-lookup"><span data-stu-id="d61c9-130">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d61c9-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="d61c9-131">Authorization</span></span>  | <span data-ttu-id="d61c9-p105">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="d61c9-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d61c9-134">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d61c9-134">Content-Type</span></span>  | <span data-ttu-id="d61c9-135">application/json</span><span class="sxs-lookup"><span data-stu-id="d61c9-135">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d61c9-136">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="d61c9-136">Request body</span></span>

| <span data-ttu-id="d61c9-137">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="d61c9-137">Property</span></span>     | <span data-ttu-id="d61c9-138">Typ</span><span class="sxs-lookup"><span data-stu-id="d61c9-138">Type</span></span>   |<span data-ttu-id="d61c9-139">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="d61c9-139">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d61c9-140">Klassifikation</span><span class="sxs-lookup"><span data-stu-id="d61c9-140">classification</span></span>|<span data-ttu-id="d61c9-141">Zeichenfolge (optional)</span><span class="sxs-lookup"><span data-stu-id="d61c9-141">String (optional)</span></span>|<span data-ttu-id="d61c9-142">Beschreibt eine Klassifizierung für die Gruppe (z. B. niedrig, Mittel oder hoch geschäftliche Relevanz).</span><span class="sxs-lookup"><span data-stu-id="d61c9-142">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="d61c9-143">Wenn Klassifizierung nicht angegeben ist, wird die Klassifizierung aus der ursprünglichen Team-Gruppe kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="d61c9-143">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="d61c9-144">description</span><span class="sxs-lookup"><span data-stu-id="d61c9-144">description</span></span>|<span data-ttu-id="d61c9-145">Zeichenfolge (optional)</span><span class="sxs-lookup"><span data-stu-id="d61c9-145">String (optional)</span></span>|<span data-ttu-id="d61c9-146">Eine optionale Beschreibung für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="d61c9-146">An optional description for the group.</span></span> <span data-ttu-id="d61c9-147">Wenn diese Eigenschaft nicht angegeben ist, wird es leer sein.</span><span class="sxs-lookup"><span data-stu-id="d61c9-147">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="d61c9-148">displayName</span><span class="sxs-lookup"><span data-stu-id="d61c9-148">displayName</span></span>|<span data-ttu-id="d61c9-149">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d61c9-149">String</span></span>|<span data-ttu-id="d61c9-p108">Der Anzeigename der Gruppe. Diese Eigenschaft ist beim Erstellen einer Gruppe erforderlich und kann bei Updates nicht deaktiviert werden. Unterstützt $Filter und $orderby.</span><span class="sxs-lookup"><span data-stu-id="d61c9-p108">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="d61c9-153">mailNickname</span><span class="sxs-lookup"><span data-stu-id="d61c9-153">mailNickname</span></span>|<span data-ttu-id="d61c9-154">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="d61c9-154">String</span></span>|<span data-ttu-id="d61c9-155">Der e-Mail-Alias für die Gruppe, die in der Organisation eindeutig.</span><span class="sxs-lookup"><span data-stu-id="d61c9-155">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="d61c9-156">Diese Eigenschaft muss angegeben werden, wenn eine Gruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="d61c9-156">This property must be specified when a group is created.</span></span> <span data-ttu-id="d61c9-157">Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="d61c9-157">Supports $filter.</span></span> <span data-ttu-id="d61c9-158">Wenn diese Eigenschaft nicht angegeben ist, wird er von der DisplayName berechnet.</span><span class="sxs-lookup"><span data-stu-id="d61c9-158">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="d61c9-159">Bekanntes Problem: Diese Eigenschaft wird zurzeit ignoriert.</span><span class="sxs-lookup"><span data-stu-id="d61c9-159">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="d61c9-160">partsToClone</span><span class="sxs-lookup"><span data-stu-id="d61c9-160">partsToClone</span></span>| [<span data-ttu-id="d61c9-161">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="d61c9-161">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="d61c9-162">Eine durch Trennzeichen getrennte Liste der Teile zum Klonen.</span><span class="sxs-lookup"><span data-stu-id="d61c9-162">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="d61c9-163">Rechtliche Webparts sind "apps, Registerkarten, Einstellungen, Kanäle, Mitglieder".</span><span class="sxs-lookup"><span data-stu-id="d61c9-163">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="d61c9-164">visibility</span><span class="sxs-lookup"><span data-stu-id="d61c9-164">visibility</span></span>|<span data-ttu-id="d61c9-165">[teamVisibilityType](../resources/teamVisibilityType.md) (optional)</span><span class="sxs-lookup"><span data-stu-id="d61c9-165">[teamVisibilityType](../resources/teamVisibilityType.md) (optional)</span></span>| <span data-ttu-id="d61c9-166">Gibt die Sichtbarkeit der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="d61c9-166">Specifies the visibility of the group.</span></span> <span data-ttu-id="d61c9-167">Mögliche Werte sind: **Private**, **Public**.</span><span class="sxs-lookup"><span data-stu-id="d61c9-167">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="d61c9-168">Wenn die Sichtbarkeit nicht angegeben wird, werden die Sichtbarkeit aus der ursprünglichen Team-Gruppe kopiert.</span><span class="sxs-lookup"><span data-stu-id="d61c9-168">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="d61c9-169">Wenn das Team geklont wird ist ein **EducationClass** Team der Sichtbarkeit-Parameter wird ignoriert und Sichtbarkeit für die neue Gruppe wird auf HiddenMembership festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="d61c9-169">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="d61c9-170">Antwort</span><span class="sxs-lookup"><span data-stu-id="d61c9-170">Response</span></span>

<span data-ttu-id="d61c9-171">Wenn erfolgreich, mit dieser Methode zurückgegeben wird eine `202 Accepted` Antwortcode mit einem Standortprofil: Verweisen auf die Ressource [Vorgang](../resources/teamsasyncoperation.md) Kopfzeile.</span><span class="sxs-lookup"><span data-stu-id="d61c9-171">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="d61c9-172">Wenn der Vorgang abgeschlossen ist, wird die Vorgang Ressource die Id des erstellten Teams informieren.</span><span class="sxs-lookup"><span data-stu-id="d61c9-172">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="d61c9-173">Beispiel</span><span class="sxs-lookup"><span data-stu-id="d61c9-173">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d61c9-174">Anforderung</span><span class="sxs-lookup"><span data-stu-id="d61c9-174">Request</span></span>
<span data-ttu-id="d61c9-175">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="d61c9-175">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="d61c9-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="d61c9-176">Response</span></span>
<span data-ttu-id="d61c9-177">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="d61c9-177">The following is an example of the response.</span></span> <span data-ttu-id="d61c9-178">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="d61c9-178">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d61c9-179">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="d61c9-179">All of the properties will be returned from an actual call.</span></span>
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
