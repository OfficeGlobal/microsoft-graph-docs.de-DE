# <a name="unarchive-team"></a><span data-ttu-id="7d53b-101">Entpackt team</span><span class="sxs-lookup"><span data-stu-id="7d53b-101">Unarchive team</span></span>



<span data-ttu-id="7d53b-102">Wiederherstellen eines archivierten [Team](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7d53b-102">Restore an archived [team](../resources/team.md).</span></span> <span data-ttu-id="7d53b-103">Dadurch wird die Möglichkeit zum Senden von Nachrichten und das Team Verhältnismäßigkeitsprinzips Mandanten und Team-Einstellungen Bearbeiten des Benutzers wiederhergestellt.</span><span class="sxs-lookup"><span data-stu-id="7d53b-103">This restores users' ability to send messages and edit the team, abiding by tenant and team settings.</span></span> <span data-ttu-id="7d53b-104">Teams sind mit dem [Archiv](team_archive.md) API archiviert.</span><span class="sxs-lookup"><span data-stu-id="7d53b-104">Teams are archived using the [archive](team_archive.md) API.</span></span>

<span data-ttu-id="7d53b-105">Unarchiving ist ein asynchroner Vorgang.</span><span class="sxs-lookup"><span data-stu-id="7d53b-105">Unarchiving is an async operation.</span></span> <span data-ttu-id="7d53b-106">Ein Team ist nicht archivierte, sobald der asynchrone Vorgang erfolgreich abgeschlossen wurde die nach einer Antwort vom diese API auftreten können.</span><span class="sxs-lookup"><span data-stu-id="7d53b-106">A team is unarchived once the async operation completes successfully, which may occur subsequent to a response from this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d53b-107">Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="7d53b-107">Permissions</span></span>
<span data-ttu-id="7d53b-p103">Eine der nachfolgenden Berechtigungen ist erforderlich, um diese API aufrufen zu können. Weitere Informationen, unter anderem zur Auswahl von Berechtigungen, finden Sie im Artikel zum Thema [Berechtigungen](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="7d53b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7d53b-110">Berechtigungstyp</span><span class="sxs-lookup"><span data-stu-id="7d53b-110">Permission type</span></span>      | <span data-ttu-id="7d53b-111">Berechtigungen (von der Berechtigung mit den wenigsten Rechten zu der mit den meisten Rechten)</span><span class="sxs-lookup"><span data-stu-id="7d53b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d53b-112">Delegiert (Geschäfts-, Schul- oder Unikonto)</span><span class="sxs-lookup"><span data-stu-id="7d53b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7d53b-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d53b-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7d53b-114">Delegiert (persönliches Microsoft-Konto)</span><span class="sxs-lookup"><span data-stu-id="7d53b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d53b-115">Nicht unterstützt</span><span class="sxs-lookup"><span data-stu-id="7d53b-115">Not supported.</span></span>    |
|<span data-ttu-id="7d53b-116">Anwendung</span><span class="sxs-lookup"><span data-stu-id="7d53b-116">Application</span></span> | <span data-ttu-id="7d53b-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d53b-117">Group.ReadWrite.All</span></span>    |

## <a name="http-request"></a><span data-ttu-id="7d53b-118">HTTP-Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d53b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/unarchive
```

## <a name="request-headers"></a><span data-ttu-id="7d53b-119">Anforderungsheader</span><span class="sxs-lookup"><span data-stu-id="7d53b-119">Request headers</span></span>
| <span data-ttu-id="7d53b-120">Kopfzeile</span><span class="sxs-lookup"><span data-stu-id="7d53b-120">Header</span></span>       | <span data-ttu-id="7d53b-121">Wert</span><span class="sxs-lookup"><span data-stu-id="7d53b-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7d53b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d53b-122">Authorization</span></span>  | <span data-ttu-id="7d53b-p104">Bearer {token}. Erforderlich.</span><span class="sxs-lookup"><span data-stu-id="7d53b-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7d53b-125">Anforderungstext</span><span class="sxs-lookup"><span data-stu-id="7d53b-125">Request body</span></span>
<span data-ttu-id="7d53b-126">Geben Sie für diese Methode keinen Anforderungstext an.</span><span class="sxs-lookup"><span data-stu-id="7d53b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d53b-127">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d53b-127">Response</span></span>

<span data-ttu-id="7d53b-128">Wenn unarchiving erfolgreich gestartet wurde, gibt diese Methode einen `202 Accepted` Antwortcode.</span><span class="sxs-lookup"><span data-stu-id="7d53b-128">If unarchiving is started successfully, this method returns a `202 Accepted` response code.</span></span> <span data-ttu-id="7d53b-129">Die Antwort enthält außerdem eine `Location` Kopf, der den Speicherort der die [TeamsAsyncOperation](../resources/teamsasyncoperation.md) enthält, die zur Verarbeitung von unarchiving des Teams erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="7d53b-129">The response will also contain a `Location` header, which contains the location of the [teamsAsyncOperation](../resources/teamsasyncoperation.md) that was created to handle unarchiving of the team.</span></span> <span data-ttu-id="7d53b-130">Überprüfen Sie den Status des Vorgangs unarchiving, indem er eine GET-Anforderung an diesen Speicherort.</span><span class="sxs-lookup"><span data-stu-id="7d53b-130">Check the status of the unarchiving operation by making a GET request to this location.</span></span>

## <a name="example"></a><span data-ttu-id="7d53b-131">Beispiel</span><span class="sxs-lookup"><span data-stu-id="7d53b-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7d53b-132">Anforderung</span><span class="sxs-lookup"><span data-stu-id="7d53b-132">Request</span></span>
<span data-ttu-id="7d53b-133">Es folgt ein Beispiel für eine Anforderung.</span><span class="sxs-lookup"><span data-stu-id="7d53b-133">The following is an example of a request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "unarchive_team"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/unarchive
```

#### <a name="response"></a><span data-ttu-id="7d53b-134">Antwort</span><span class="sxs-lookup"><span data-stu-id="7d53b-134">Response</span></span>
<span data-ttu-id="7d53b-135">Es folgt ein Beispiel für eine Antwort.</span><span class="sxs-lookup"><span data-stu-id="7d53b-135">The following is an example of a response.</span></span>
```http
HTTP/1.1 202 Accepted
Location: /teams{id}/operations({opId})
Content-Type: text/plain
Content-Length: 0
```

<!-- uuid: 9a9bb83f-6f35-4426-bb04-73ca43ad6cc8
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Unarchive team",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
