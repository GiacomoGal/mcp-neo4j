# Ingresso di lettura del fork

Questo file è l'ingresso comune, per persone e agenti, del fork `GiacomoGal/mcp-neo4j`. Si legge per primo solo come indice di questo fork. I contratti upstream restano nei loro file, con lo stesso rango, gli stessi destinatari, le stesse condizioni e gli stessi rimandi. Qui non si abbassa e non si alza alcun contratto, e non si sostituisce `README.md` né `gemini-extension/GEMINI.md`.

Mandato di questo ingresso: t127u, lotto 6, sola sezione 5, più i vincoli comuni dello stesso allegato. Scope documentale. Nessun PASS. La review è indipendente.

## Unknown espliciti

Uso attuale, installazione e database sono unknown. L'inventario locale della sezione 5 registra `identity_proven=False`, `unknowncurrentuse=True`, `nextdocscope=unresolved`, e liste vuote per `identity_evidence`, `proposalOct`, `decisionlater`, `executionreceipt`. Quei valori sono la fonte dell'inventario, non un esito misurato su un host.

UNMAPPED: il nome `neo4j`, i nomi dei quattro server e la parola memory non associano database, istanze, account o grafi di memoria esistenti. `activeguide` non compare in questo albero e non significherebbe attivo. Non risulta una classe legacy da riattivare. Unresolved resta una guida esplorativa sobria.

Il branch di default osservato su GitHub e il branch locale `main` si chiamano `main`. Questa omonimia non prova allineamento con un host, con il parent o con un database.

## Identità osservata, senza sync

| Fatto | Fonte | Limite |
| --- | --- | --- |
| Repository `GiacomoGal/mcp-neo4j`, fork, non archiviato, descrizione «Model Context Protocol with Neo4j», branch di default `main` | Metadata GitHub del fork, 2026-11-07 | Metadata pubblica. Non è uso, installazione o database |
| Parent registrato: `neo4j-contrib/mcp-neo4j` | Stessa metadata | Nessun fetch, merge, push o PR verso il parent |
| `origin` locale punta a `GiacomoGal/mcp-neo4j` | Configurazione git locale, senza trascrivere credenziali | Prova l'identità configurata. Non prova canonicità, sync o uso |
| `HEAD` = `origin/main` = `b9c2effe92c3ff7c477737b38c72ce0f76d2f9f7` | Git locale | Il messaggio storico è «Docs: Added cloud (AWS, Azure) deployment instructions. (#198)», autore Pedro Leitao. Storia del commit, non decisione di questo mandato |
| Allineamento dell'albero con il parent | Non eseguito | Non attestato |

Nessuna PR verso `neo4j-contrib`. L'invito a contribuire in `README.md` righe 84-86 resta com'è: questo passaggio non lo revoca e non lo esercita.

## Come leggere

Persone e agenti usano lo stesso ordine e le stesse condizioni.

1. Leggere questo indice.
2. Lasciare intatti i file upstream citati sotto. Il loro rango vale anche per le righe non trascritte qui.
3. Trattare comandi, configurazioni, prompt, query ed esempi Cypher come testo dei manuali. Descriverli non autorizza esecuzione, login, connessione, installazione o dati reali.
4. Non sincronizzare memorie e non aprire env, token, password, URI con credenziali, config sensibili, backup, store, database, grafi di memoria o payload di grafo.
5. Assenze, commenti, changelog, prompt e manuali ricevono policy solo se il fonte gliela assegna già. Questo indice non gliene aggiunge.

Questo file non è `AGENTS.md`. Chi carica solo istruzioni automatiche di quel nome non lo riceve da solo. L'assenza di un caricatore automatico è voluta: non si aggiunge un secondo contratto agente.

## Rango usato nella matrice

Il rango è quello del fonte. La colonna «Trattamento» dice solo come questo ingresso lo riporta.

| Rango | Significato nel fonte | Effetto su questo ingresso |
| --- | --- | --- |
| R1 | Obbligo di condotta già scritto (licenza, disclosure, checklist PR, cautele di sicurezza nei manuali) | Citato e lasciato nel file originale. Non scaricato da questo passaggio, perché le condizioni d'uso non sono state attivate |
| R2 | Descrizione upstream di protocollo, server e capacità | Catalogo. Non è prova che un server sia in esecuzione |
| R3 | Istruzione operativa, esempio, prompt o query nel manuale | Il rango di manuale resta. Condizione aggiunta solo in lettura del fork: non è mandato di esecuzione o di connessione per questo passaggio |
| R4 | Trigger o host ref | Percorso o URL conservati. Il bersaglio operativo non è stato aperto come contenuto normativo |
| R0 | Vincolo esterno t127u / lotto 6 sezione 5 | Vale per chi scrive e legge questo ingresso. Non modifica i file upstream |
| Assenza | File non presente | L'assenza resta. Non viene colmata con un contratto sostitutivo |

Conflitti e storia stanno fuori dalle decisioni. L'unica decisione di questo passaggio è aggiungere questo indice sul fork. Non decide uso, dismissione, deploy, sync o merge.

## Matrice fonti → questo ingresso

### Contratti e manuali letti in tutto o in parte

| Fonte | Righe | Rango | Destinatario nel fonte | Condizioni nel fonte | Trigger / host ref | Lettura | Trattamento | Motivo |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Allegato lotto 6, vincoli comuni e sezione 5 | Testo esterno, non è un file del repo | R0 | Esecutore del passaggio e lettori dell'ingresso | Solo `GiacomoGal/mcp-neo4j`; UNMAPPED; guide Markdown; no esecuzione; no PR upstream | Nessuno nel repo | Testo dell'allegato letto | Realizzato in questo file | Unica autorizzazione a scrivere |
| `README.md` | 1-11 | R2, con domande di esempio in R3 | Lettori del progetto | Nessuna condizione di fork | `https://modelcontextprotocol.io/introduction` riga 3 | Testo letto | Rango invariato. Le cinque domande restano esempi. Nessun risultato certificato | Ingresso umano upstream da non riscrivere |
| `README.md` | 13-40 | R2 | Lettori del progetto | Quattro server descritti come componenti del repo | Link relativi ai README annidati. Riga 30: `./servers/mcp-neo4j-cloud-aura-api//` (doppio slash nel fonte). Riga 32: `https://console.neo4j.io` | Testo letto | Directory locali presenti. Il doppio slash non è stato «corretto». La console non è stata contattata. Il nome memory non associa memorie | Preservare il catalogo, compreso il ref com'è scritto |
| `README.md` | 42-70 | R3 | Chi avvia un server | Flag e variabili di transport descritte nel manuale | Host e path di esempio nel blocco comandi | Testo letto | Comandi non eseguiti e non ricopiati come procedura | Non declassare il manuale; non eseguirlo |
| `README.md` | 72-82 | R3 | Chi pubblica i server su cloud | Rimando al manuale cloud | `README-Cloud.md` | Testo letto | Puntatore conservato | Il cloud resta manuale, non deploy effettuato |
| `README.md` | 84-86 | R1 testuale di invito | Contributori | Nessuna | Nessuno | Testo letto | Invito invariato. Questo passaggio non apre PR upstream | Distinguere il contratto dalla decisione locale |
| `README.md` | 88-92 | R3 | Lettori | Nessuna | Tre URL `https://neo4j.com/blog/developer/...` | Titoli e URL letti. Corpo dei blog non letto | Claim dei blog non certificati | I post non diventano policy del fork |
| `README.md` | 94-96 | R2 | Lettori | Rimando alla licenza | `LICENSE.txt` | Testo letto | Puntatore conservato | La licenza sta nel proprio file |
| `LICENSE.txt` | 1-21 | R1 | Chi riceve il software | Inclusione dell'avviso di copyright nelle copie | Nessuno | Testo letto | File non modificato. Copyright nel fonte: Neo4j, 2024-2025. Questo indice non è una copia dei termini | Obbligo di licenza fuori da questo overlay |
| `SECURITY.md` | 1-2 | R1 | Chi segnala una vulnerabilità | Seguire i passi della policy al URL indicato | `https://neo4j.com/trust-center/responsible-disclosure/` | Due righe lette. Passi della policy non seguiti e non copiati | Obbligo lasciato al file. Vedi esito HTTP sotto: il corpo non è stato letto | Non sostituire la policy di disclosure |
| `gemini-extension/GEMINI.md` | 1-23 | R3 annidato, ingresso agente Gemini | Chi installa l'estensione Gemini | Variabili d'ambiente richieste dal testo; esito assunto dal manuale, non osservato | Riga 9: `https://github.com/neo4j-contrib/mcp-neo4j.git` | Testo letto | Comandi di install e uninstall non eseguiti. Nessun clone | Preservare l'ingresso agente upstream |
| `gemini-extension.json` | 1-21 | R2 | Client dell'estensione Gemini | Quattro chiavi `mcpServers` con comando `uvx` e un argomento ciascuna. Nel file non ci sono variabili d'ambiente | Nessun URL | Testo letto | Comandi non eseguiti. Non prova un'installazione locale | Manifest agente coerente con `GEMINI.md`, non un secondo obbligo |
| `glama.json` | 1-6 | R2 | Registry Glama | Schema e tre stringhe maintainer | `https://glama.ai/mcp/schemas/server.json` | Testo letto. Schema remoto non adottato | I maintainer scritti non sono una prova di uso di questo fork e non diventano destinatari di un invio | Non promuovere il registry a policy locale |
| `.github/pull_request_template.md` | 1-36 | R1 | Autori di PR su questo repository | Checklist condizionata al tipo di modifica | Nessuno | Testo letto | La PR di questo ingresso usa il template. Le voci di test applicativo, server MCP e changelog restano non soddisfatte | Il template non viene adattato per far sembrare eseguiti i test |
| `README-Cloud.md` | 1-335 | R3 | Chi fa un deploy AWS o Azure | Prerequisiti di account e registry scritti nel manuale | Placeholder `yourdomain.com`, `your-deployment-url` e analoghi. Non sono host accertati | Titolo, righe 1-20 e 252-335 letti. I blocchi intermedi di comandi cloud non sono stati trascritti | Intero manuale non modificato. Nessun comando cloud eseguito. Gli endpoint di health del manuale non sono stati chiamati | Manuale operativo intero, anche dove il corpo non è stato copiato |
| `servers/mcp-neo4j-cypher/README.md` | 1-16; 18-48; 185-195. Titoli di sezione sul resto del file (560 righe) | R2 per overview e tool; R1 per le best practice lette; R3 per i comandi del resto | Utenti del server Cypher e, per le cautele, chi espone HTTP | Timeout e read-only descritti alle righe 33 e 41. Cautele 185-195: origini specifiche, no `*` in produzione con credenziali, HTTPS in produzione; host reali, localhost solo per sviluppo, no `*` senza comprenderne i rischi | Vedi tabella host. Immagine `assets/images/text2cypher-process.png` | Porzioni indicate lette. Corpo di install, Docker e sviluppo non trascritto | Tool `read_neo4j_cypher`, `write_neo4j_cypher`, `get_neo4j_schema` restano descrizione di capacità. Nessuna query eseguita. Immagine presente, byte non letti | Non trasformare gli esempi Cypher in policy né in mandato |
| `servers/mcp-neo4j-memory/README.md` | 1-30; 249-259. Titoli sul resto (385 righe) | R2 per overview e schema; R3 per l'esempio d'uso 18-26; R1 per le cautele 249-259, stesso tenore del server Cypher | Utenti del server memory | Il manuale parla di memoria persistente su Neo4j locale o remoto | Riga 9: `https://console.neo4j.io`, non contattata. Immagini in `docs/images/` | Porzioni indicate lette | Esempio e immagini restano materiale upstream. Nessuna memoria letta, scritta o sincronizzata. Lo schema `Memory` / `Relationship` è testo del manuale, non un grafo esistente | `nomemorysync`: il componente non aggancia memorie di questo fork |
| `servers/mcp-neo4j-data-modeling/README.md` | 1-20; 168-177. Titoli e righe 314-320 individuate per ricerca | R2 overview; R3 prompt `create_new_data_model` e demo; la tabella variabili è descrizione R2, senza una sezione «Security Best Practices» omonima | Utenti del server di modeling e l'agente che riceve il prompt | Il prompt è strutturato dal manuale. Non è una policy del fork | `https://arrows.app/`, repo demo, PyPI. Clone di esempio con `yourusername`, non aperto | Porzioni indicate lette. Corpo del prompt non ricopiato | Il prompt non è policy e non è un mandato di generazione | Evitare che la sezione Prompts diventi obbligo agente |
| `servers/mcp-neo4j-cloud-aura-api/README.md` | 1-17; 293-303. Titoli 426-446 | R2 overview; R3 autenticazione descritta; R1 cautele 293-303, stesso tenore; R3 esempi d'uso dai soli titoli | Chi gestisce istanze Aura tramite il manuale | Il manuale richiede Client ID e Client Secret ottenuti dalla console | Due URL di documentazione Aura, riga 15 e 17. Console non aperta. Credenziali non cercate | Righe 1-17 e 293-303 lette. Esempi 426-442 solo come titoli | Nessuna credenziale riportata. L'URL di riga 15 non è stato sostituito dopo il controllo HTTP | Il fallimento di un link non autorizza a riscrivere il manuale |

### Trigger, host e altre fonti non aperti

| Fonte | Rango | Destinatario | Condizioni / trigger | Lettura | Trattamento | Motivo |
| --- | --- | --- | --- | --- | --- | --- |
| `.github/workflows/pr-mcp-neo4j-cypher.yml` | R4 | Automazione del repo, non accertata nel contenuto | `on:` non letto. Il nome file non è una condizione | Non aperto | File lasciato. Nessun run | Preservare il trigger senza ricavarne una policy |
| `.github/workflows/pr-mcp-neo4j-memory.yml` | R4 | Come sopra | Come sopra | Non aperto | Come sopra | Come sopra |
| `.github/workflows/pr-mcp-neo4j-data-modeling.yml` | R4 | Come sopra | Come sopra | Non aperto | Come sopra | Come sopra |
| `.github/workflows/pr-mcp-neo4j-cloud-aura-api.yml` | R4 | Come sopra | Come sopra | Non aperto | Come sopra | Come sopra |
| `.github/workflows/publish-cypher.yml` | R4 | Come sopra | Come sopra | Non aperto | Come sopra | Come sopra |
| `.github/workflows/publish-memory.yml` | R4 | Come sopra | Come sopra | Non aperto | Come sopra | Come sopra |
| `.github/workflows/publish-data-modeling.yml` | R4 | Come sopra | Come sopra | Non aperto | Come sopra | Come sopra |
| `.github/workflows/publish-aura-manager.yml` | R4 | Come sopra | Come sopra | Non aperto | Come sopra | Come sopra |
| `.github/workflows/generate-upload-dxt-cypher.yml` | R4 | Come sopra | Come sopra | Non aperto | Come sopra | Come sopra |
| `https://console.neo4j.io` in `README.md:32` e `servers/mcp-neo4j-memory/README.md:9` | R4 | Lettori dei due manuali | Host di prodotto nel testo upstream | Non contattato | URL invariati | Host operativo: niente login e niente associazione a un account |
| URL `localhost`, `example.com`, `yourapp.com`, `yourdomain.com`, `your-deployment-url`, `yourusername` nei manuali | R4 | Lettori dei manuali | Placeholder o loopback scritti come esempio | Non contattati | Non promossi a endpoint reali | Non sono database né deploy di questo fork |
| `.gitignore` riga 1 `.env`, riga 50 `mcp.json` | R1 di esclusione dal tree pubblicato | Chi lavora sull'albero | I nomi sono ignorati da git | Righe lette. Nessun file `.env` o `mcp.json` nell'elenco dell'albero di lavoro. Contenuti non cercati altrove | Esclusione conservata | Non aprire la classe di file che il repo già tiene fuori |
| `.gitignore` riga 2, URL `http://help.github.com/ignore-files/` | R4 | Lettori del commento | Commento upstream | URL non richiesto | Commento non promosso a policy | Host ref lasciato chiuso |
| Quattro `CHANGELOG.md` sotto `servers/` | Storia | Lettori delle versioni | Nessuna trasformata in decisione | Solo titoli di versione individuati per ricerca, corpi non usati | File non modificati | La storia di versione non è una decisione di uso |
| `.vscode/extensions.json` | Non è un contratto Neo4j | Editor | Quattro raccomandazioni di estensioni non Neo4j | Testo letto | Non modificato e non promosso | Evitare di farne una policy del fork |
| Codice, test, Dockerfile, compose, Makefile, `pyproject.toml`, `uv.lock`, `.verdaccio/config.yml`, immagini, script `test.sh` / `inspector.sh` | Non classificati come contratti di questo ingresso | — | Non derivati | Non aperti. Eccezione: esistenza su disco delle immagini citate dai README, senza lettura dei byte | Nessuna modifica | I payload e le config possono essere sensibili o operativi. Nessuna affermazione sul loro comportamento |

### Assenze preservate

Non esistono, in questo albero, `AGENTS.md`, `CLAUDE.md`, `.cursorrules`, `.cursor/rules`, né una directory `docs/`. L'assenza non è stata riempita con regole nuove. Questo `GUIDA.md` è un indice del fork, non un rimpiazzo di quelle assenze.

## Esempi

Gli esempi Cypher, i prompt, le query e i blocchi di comandi nei README sono R3. Restano nel manuale upstream. Non sono policy del fork e non sono un mandato di esecuzione, di connessione, di installazione o di sync delle memorie. Nessun esempio è stato ricopiato in questo file.

## Controlli di link e di path

Data del controllo: 2026-11-07T20:58:46Z. Metodo: richiesta HTTP con al più cinque redirect, codice e URL finale, corpo scartato, senza login e senza cookie di sessione conservati. Il controllo di stato non adotta il contenuto della pagina. I path locali sono esistenza su disco, non lettura di media o di codice.

| URL nel fonte | Esito osservato | Limite |
| --- | --- | --- |
| `https://modelcontextprotocol.io/introduction` | 200 dopo 1 redirect verso `https://modelcontextprotocol.io/docs/2026-07-28/getting-started/intro` | Corpo non letto. La destinazione del redirect non sostituisce l'URL scritto nel README |
| `https://neo4j.com/blog/developer/model-context-protocol/` | 200, 0 redirect | Corpo non letto |
| `https://neo4j.com/blog/developer/claude-converses-neo4j-via-mcp/` | 200, 0 redirect | Corpo non letto |
| `https://neo4j.com/blog/developer/knowledge-graphs-claude-neo4j-mcp/` | 200, 0 redirect | Corpo non letto |
| `https://neo4j.com/trust-center/responsible-disclosure/` | 200 dopo 1 redirect verso `https://neo4j.com/responsible-disclosure/` | Passi non letti e non eseguiti |
| `https://pypi.org/project/mcp-neo4j-cypher/` | 200 | Pagina non letta. Presenza HTTP non prova installazione locale |
| `https://pypi.org/project/mcp-neo4j-data-modeling/` | 200 | Come sopra |
| `https://neo4j.com/docs/aura/classic/platform/api/overview/` | 404 dopo 1 redirect verso `https://neo4j.com/docs/aura/api/overview/overview/` | Documento vivo non verificato. URL del manuale non modificato e non rimpiazzato |
| `https://neo4j.com/docs/aura/platform/api/specification/` | 200 | Corpo non letto. Nessuna chiamata API |
| `https://arrows.app/` | 200 | Corpo non letto |
| `https://glama.ai/mcp/schemas/server.json` | 200 | Schema non incorporato |
| `https://github.com/neo4j-contrib/mcp-neo4j` | 200 | Pagina non usata come sync |
| `https://github.com/neo4j-contrib/mcp-neo4j.git` | 200 dopo 1 redirect verso la pagina del repo | Nessun clone |
| `https://github.com/neo4j-contrib/mcp-neo4j/releases` | 200 | Elenco release non adottato come versione in uso |
| `https://github.com/astral-sh/uv` | 200 | `uv` non installato |
| `https://github.com/neo4j-field/data-modeling-assistant-demo` | 200 | Repo demo non clonato. Non è questo fork |
| `https://github.com/GiacomoGal/mcp-neo4j` | 200 | Pagina del fork. Non è una prova di attività |

Path relativi: esistono le directory `servers/mcp-neo4j-cypher`, `servers/mcp-neo4j-memory`, `servers/mcp-neo4j-cloud-aura-api`, `servers/mcp-neo4j-data-modeling`, e i file immagine citati dai README di Cypher, data modeling, memory e Aura. I byte delle immagini non sono stati letti. Il doppio slash in `README.md` riga 30 non ha un controllo HTTP separato: la directory senza slash esiste in locale.

Non contattati, di proposito: `https://console.neo4j.io`, ogni `localhost`, i placeholder di dominio e gli URL `yourusername`.

## Decisioni e non-decisioni

Decisione di questo passaggio: aggiungere solo `GUIDA.md` sul fork, per la review.

Non decisioni: uso del software, installazione, esistenza di un database, esistenza di memorie, allineamento con `neo4j-contrib/mcp-neo4j`, esecuzione dei workflow, accettazione della PR, PASS documentale. `executionreceipt` dell'inventario non viene compilato. `executed` non viene impostato.

## Ricevuta e limiti

| Campo | Valore |
| --- | --- |
| Base | `b9c2effe92c3ff7c477737b38c72ce0f76d2f9f7` su `main` |
| Head | SHA del commit di questo file, riportato nella PR. Non è scritto qui, perché entrerebbe nell'hash |
| Diff atteso | Solo `GUIDA.md`. Nessun codice, config, script, query, dato, media o lockfile |
| Push | Ordinario verso `GiacomoGal/mcp-neo4j`, senza force e senza rebase |
| Verifiche | Lettura documentale elencata e controlli HTTP/path di questa pagina |
| Effetto dei controlli | Stato di rete o esistenza di path. Nessun effetto su server, database o memorie |
| PASS | Non assegnato. Review indipendente |

Limiti che restano aperti: corpi dei blog, della disclosure, dello schema Glama e delle pagine GitHub non letti; workflow non aperti; manuali lunghi non trascritti oltre le righe indicate; URL Aura classico non risolto con 200; parent non fetchato; nessun test del software; nessuna prova che i pacchetti PyPI visibili in HTTP siano installati qui.
