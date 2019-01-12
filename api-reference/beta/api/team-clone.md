---
title: Klonen Sie ein team
description: Erstellen Sie eine Kopie eines Teams. Dieser Vorgang wird außerdem eine Kopie der entsprechenden Gruppe erstellt.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4fb3769db0df6d2fc30d995098daee19b49e83b7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958341"
---
# <a name="clone-a-team"></a><span data-ttu-id="0a915-104">Klonen Sie ein team</span><span class="sxs-lookup"><span data-stu-id="0a915-104">Clone a team</span></span>

> <span data-ttu-id="0a915-105">**Wichtig:** Die APIs der /Beta-Version in Microsoft Graph befinden sich in der Vorschau und können Änderungen unterliegen.</span><span class="sxs-lookup"><span data-stu-id="0a915-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a915-106">Die Verwendung dieser APIs in Produktionsanwendungen wird nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="0a915-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a915-107">Erstellen Sie eine Kopie eines [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="0a915-107">Create a copy of a [team](../resources/team.md).</span></span> <span data-ttu-id="0a915-108">Dieser Vorgang wird außerdem eine Kopie der entsprechenden [Gruppe](../resources/group.md)erstellt.</span><span class="sxs-lookup"><span data-stu-id="0a915-108">This operation also creates a copy of the corresponding [group](../resources/group.md).</span></span>
<span data-ttu-id="0a915-109">Sie können die Teile des Teams Klonen angeben:</span><span class="sxs-lookup"><span data-stu-id="0a915-109">You can specify which parts of the team to clone:</span></span>

- <span data-ttu-id="0a915-110">**apps** – Microsoft-Teams, Kopien apps, die im Team installiert sind.</span><span class="sxs-lookup"><span data-stu-id="0a915-110">**apps** - Copies Microsoft Teams apps that are installed in the team.</span></span> 
- <span data-ttu-id="0a915-111">**Kanäle** – kopiert die Struktur DDE-Kanal (jedoch nicht die Nachrichten im Kanal).</span><span class="sxs-lookup"><span data-stu-id="0a915-111">**channels** – Copies the channel structure (but not the messages in the channel).</span></span>
- <span data-ttu-id="0a915-112">**Elemente des Objekts** – kopiert die Mitglieder und Besitzer der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="0a915-112">**members** – Copies the members and owners of the group.</span></span>
- <span data-ttu-id="0a915-113">**Einstellungen** – kopiert alle Einstellungen im Team, zusammen mit den wichtigsten gruppeneinstellungen.</span><span class="sxs-lookup"><span data-stu-id="0a915-113">**settings** – Copies all settings within the team, along with key group settings.</span></span>
- <span data-ttu-id="0a915-114">**Registerkarten** – kopiert die Registerkarten in den Kanälen.</span><span class="sxs-lookup"><span data-stu-id="0a915-114">**tabs** – Copies the tabs within channels.</span></span>

<span data-ttu-id="0a915-115">Wenn Registerkarten geklont werden, in einen nicht konfigurierten Status zugeführt werden – auf der Registerleiste in Microsoft-Teams angezeigt werden, und beim ersten Öffnen, werden über den Konfigurationsbildschirm wechseln.</span><span class="sxs-lookup"><span data-stu-id="0a915-115">When tabs are cloned, they are put into an unconfigured state -- they are displayed on the tab bar in Microsoft Teams, and the first time you open them, you'll go through the configuration screen.</span></span> <span data-ttu-id="0a915-116">(Wenn die Person, die beim Öffnen der Registerkarte keinen Berechtigung zum Konfigurieren von apps, sehen sie eine Meldung angezeigt, dass die Registerkarte nicht konfiguriert wurde.)</span><span class="sxs-lookup"><span data-stu-id="0a915-116">(If the person opening the tab does not have permission to configure apps, they will see a message explaining that the tab hasn't been configured.)</span></span>

<span data-ttu-id="0a915-117">Klonen ist ein zeitintensiver Vorgang.</span><span class="sxs-lookup"><span data-stu-id="0a915-117">Cloning is a long-running operation.</span></span>
<span data-ttu-id="0a915-118">Nachdem der POST-Klon zurückgegeben wird, müssen Sie den [Vorgang](../resources/teamsasyncoperation.md) abrufen, um festzustellen, ob es sich um "ausführen" oder "erfolgreich" oder "Fehler" ist.</span><span class="sxs-lookup"><span data-stu-id="0a915-118">After the POST clone returns, you need to GET the [operation](../resources/teamsasyncoperation.md) to see if it's "running" or "succeeded" or "failed".</span></span> <span data-ttu-id="0a915-119">Sie sollten zu berechnen fortfahren, bis der Status nicht "aktiv" ist.</span><span class="sxs-lookup"><span data-stu-id="0a915-119">You should continue to GET until the status is not "running".</span></span> <span data-ttu-id="0a915-120">Die empfohlene Verzögerung zwischen ruft beträgt 5 Sekunden.</span><span class="sxs-lookup"><span data-stu-id="0a915-120">The recommended delay between GETs is 5 seconds.</span></span>

## <a name="permissions"></a><span data-ttu-id="0a915-121">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="0a915-121">Permissions</span></span>

<span data-ttu-id="0a915-p106">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0a915-p106">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a915-124">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="0a915-124">Permission type</span></span>      | <span data-ttu-id="0a915-125">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="0a915-125">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a915-126">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="0a915-126">Delegated (work or school account)</span></span>     | <span data-ttu-id="0a915-127">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a915-127">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0a915-128">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="0a915-128">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a915-129">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="0a915-129">Not supported.</span></span>    |
|<span data-ttu-id="0a915-130">Anwendung</span><span class="sxs-lookup"><span data-stu-id="0a915-130">Application</span></span>                            | <span data-ttu-id="0a915-131">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0a915-131">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a915-132">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a915-132">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/clone
```

## <a name="request-headers"></a><span data-ttu-id="0a915-133">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="0a915-133">Request headers</span></span>
| <span data-ttu-id="0a915-134">Header</span><span class="sxs-lookup"><span data-stu-id="0a915-134">Header</span></span>       | <span data-ttu-id="0a915-135">Wert</span><span class="sxs-lookup"><span data-stu-id="0a915-135">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0a915-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a915-136">Authorization</span></span>  | <span data-ttu-id="0a915-p107">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0a915-p107">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0a915-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0a915-139">Content-Type</span></span>  | <span data-ttu-id="0a915-140">application/json</span><span class="sxs-lookup"><span data-stu-id="0a915-140">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0a915-141">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="0a915-141">Request body</span></span>

| <span data-ttu-id="0a915-142">Eigenschaft</span><span class="sxs-lookup"><span data-stu-id="0a915-142">Property</span></span>     | <span data-ttu-id="0a915-143">Typ</span><span class="sxs-lookup"><span data-stu-id="0a915-143">Type</span></span>   |<span data-ttu-id="0a915-144">Beschreibung</span><span class="sxs-lookup"><span data-stu-id="0a915-144">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a915-145">Klassifikation</span><span class="sxs-lookup"><span data-stu-id="0a915-145">classification</span></span>|<span data-ttu-id="0a915-146">Zeichenfolge (optional)</span><span class="sxs-lookup"><span data-stu-id="0a915-146">String (optional)</span></span>|<span data-ttu-id="0a915-147">Beschreibt eine Klassifizierung für die Gruppe (z. B. niedrig, Mittel oder hoch geschäftliche Relevanz).</span><span class="sxs-lookup"><span data-stu-id="0a915-147">Describes a classification for the group (such as low, medium or high business impact).</span></span> <span data-ttu-id="0a915-148">Gültige Werte für diese Eigenschaft werden durch Erstellen [eines Einstellungswerts ClassificationList, basierend auf der [Vorlagendefinition](../resources/directorysettingtemplate.md)](../resources/directorysetting.md) definiert.</span><span class="sxs-lookup"><span data-stu-id="0a915-148">Valid values for this property are defined by creating a ClassificationList [setting](../resources/directorysetting.md) value, based on the [template definition](../resources/directorysettingtemplate.md).</span></span> <span data-ttu-id="0a915-149">Wenn Klassifizierung nicht angegeben ist, wird die Klassifizierung aus der ursprünglichen Team-Gruppe kopiert werden.</span><span class="sxs-lookup"><span data-stu-id="0a915-149">If classification is not specified, the classification will be copied from the original team/group.</span></span>|
|<span data-ttu-id="0a915-150">description</span><span class="sxs-lookup"><span data-stu-id="0a915-150">description</span></span>|<span data-ttu-id="0a915-151">Zeichenfolge (optional)</span><span class="sxs-lookup"><span data-stu-id="0a915-151">String (optional)</span></span>|<span data-ttu-id="0a915-152">Eine optionale Beschreibung für die Gruppe.</span><span class="sxs-lookup"><span data-stu-id="0a915-152">An optional description for the group.</span></span> <span data-ttu-id="0a915-153">Wenn diese Eigenschaft nicht angegeben ist, wird es leer sein.</span><span class="sxs-lookup"><span data-stu-id="0a915-153">If this property is not specified, it will be left blank.</span></span>|
|<span data-ttu-id="0a915-154">displayName</span><span class="sxs-lookup"><span data-stu-id="0a915-154">displayName</span></span>|<span data-ttu-id="0a915-155">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0a915-155">String</span></span>|<span data-ttu-id="0a915-p110">Der Anzeigename der Gruppe. Diese Eigenschaft ist beim Erstellen einer Gruppe erforderlich und kann bei Updates nicht deaktiviert werden. Unterstützt $Filter und $orderby.</span><span class="sxs-lookup"><span data-stu-id="0a915-p110">The display name for the group. This property is required when a group is created and it cannot be cleared during updates. Supports $filter and $orderby.</span></span>|
|<span data-ttu-id="0a915-159">mailNickname</span><span class="sxs-lookup"><span data-stu-id="0a915-159">mailNickname</span></span>|<span data-ttu-id="0a915-160">Zeichenfolge</span><span class="sxs-lookup"><span data-stu-id="0a915-160">String</span></span>|<span data-ttu-id="0a915-161">Der e-Mail-Alias für die Gruppe, die in der Organisation eindeutig.</span><span class="sxs-lookup"><span data-stu-id="0a915-161">The mail alias for the group, unique in the organization.</span></span> <span data-ttu-id="0a915-162">Diese Eigenschaft muss angegeben werden, wenn eine Gruppe erstellt wird.</span><span class="sxs-lookup"><span data-stu-id="0a915-162">This property must be specified when a group is created.</span></span> <span data-ttu-id="0a915-163">Unterstützt $filter.</span><span class="sxs-lookup"><span data-stu-id="0a915-163">Supports $filter.</span></span> <span data-ttu-id="0a915-164">Wenn diese Eigenschaft nicht angegeben ist, wird er von der DisplayName berechnet.</span><span class="sxs-lookup"><span data-stu-id="0a915-164">If this property is not specified, it will be computed from the displayName.</span></span> <span data-ttu-id="0a915-165">Bekanntes Problem: Diese Eigenschaft wird zurzeit ignoriert.</span><span class="sxs-lookup"><span data-stu-id="0a915-165">Known issue: this property is currently ignored.</span></span>|
|<span data-ttu-id="0a915-166">partsToClone</span><span class="sxs-lookup"><span data-stu-id="0a915-166">partsToClone</span></span>| [<span data-ttu-id="0a915-167">clonableTeamParts</span><span class="sxs-lookup"><span data-stu-id="0a915-167">clonableTeamParts</span></span>](../resources/clonableteamparts.md) |<span data-ttu-id="0a915-168">Eine durch Trennzeichen getrennte Liste der Teile zum Klonen.</span><span class="sxs-lookup"><span data-stu-id="0a915-168">A comma-seperated list of the parts to clone.</span></span> <span data-ttu-id="0a915-169">Rechtliche Webparts sind "apps, Registerkarten, Einstellungen, Kanäle, Mitglieder".</span><span class="sxs-lookup"><span data-stu-id="0a915-169">Legal parts are "apps, tabs, settings, channels, members".</span></span>|
|<span data-ttu-id="0a915-170">visibility</span><span class="sxs-lookup"><span data-stu-id="0a915-170">visibility</span></span>|<span data-ttu-id="0a915-171">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span><span class="sxs-lookup"><span data-stu-id="0a915-171">[teamVisibilityType](../resources/teamvisibilitytype.md) (optional)</span></span>| <span data-ttu-id="0a915-172">Gibt die Sichtbarkeit der Gruppe.</span><span class="sxs-lookup"><span data-stu-id="0a915-172">Specifies the visibility of the group.</span></span> <span data-ttu-id="0a915-173">Mögliche Werte sind: **Private**, **Public**.</span><span class="sxs-lookup"><span data-stu-id="0a915-173">Possible values are: **Private**, **Public**.</span></span> <span data-ttu-id="0a915-174">Wenn die Sichtbarkeit nicht angegeben wird, werden die Sichtbarkeit aus der ursprünglichen Team-Gruppe kopiert.</span><span class="sxs-lookup"><span data-stu-id="0a915-174">If visibility is not specified, the visibility will be copied from the original team/group.</span></span> <span data-ttu-id="0a915-175">Wenn das Team geklont wird ist ein **EducationClass** Team der Sichtbarkeit-Parameter wird ignoriert und Sichtbarkeit für die neue Gruppe wird auf HiddenMembership festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="0a915-175">If the team being cloned is an **educationClass** team, the visibility parameter is ignored, and the new group's visibility will be set to HiddenMembership.</span></span>|

## <a name="response"></a><span data-ttu-id="0a915-176">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a915-176">Response</span></span>

<span data-ttu-id="0a915-177">Wenn erfolgreich, mit dieser Methode zurückgegeben wird eine `202 Accepted` Antwortcode mit einem Standortprofil: Verweisen auf die Ressource [Vorgang](../resources/teamsasyncoperation.md) Kopfzeile.</span><span class="sxs-lookup"><span data-stu-id="0a915-177">If successful, this method will return a `202 Accepted` response code with a Location: header pointing to the [operation](../resources/teamsasyncoperation.md) resource.</span></span>
<span data-ttu-id="0a915-178">Wenn der Vorgang abgeschlossen ist, wird die Vorgang Ressource die Id des erstellten Teams informieren.</span><span class="sxs-lookup"><span data-stu-id="0a915-178">When the operation is complete, the operation resource will tell you the id of the created team.</span></span>

## <a name="example"></a><span data-ttu-id="0a915-179">Beispiel</span><span class="sxs-lookup"><span data-stu-id="0a915-179">Example</span></span>
#### <a name="request"></a><span data-ttu-id="0a915-180">Anforderung</span><span class="sxs-lookup"><span data-stu-id="0a915-180">Request</span></span>
<span data-ttu-id="0a915-181">Nachfolgend sehen Sie ein Beispiel der Anforderung.</span><span class="sxs-lookup"><span data-stu-id="0a915-181">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="0a915-182">Antwort</span><span class="sxs-lookup"><span data-stu-id="0a915-182">Response</span></span>
<span data-ttu-id="0a915-183">Nachfolgend sehen Sie ein Beispiel der Antwort.</span><span class="sxs-lookup"><span data-stu-id="0a915-183">The following is an example of the response.</span></span> <span data-ttu-id="0a915-184">Hinweis: Das hier gezeigte Antwortobjekt ist möglicherweise aus Platzgründen abgeschnitten.</span><span class="sxs-lookup"><span data-stu-id="0a915-184">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0a915-185">Von einem tatsächlichen Aufruf werden alle Eigenschaften zurückgegeben.</span><span class="sxs-lookup"><span data-stu-id="0a915-185">All of the properties will be returned from an actual call.</span></span>
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
