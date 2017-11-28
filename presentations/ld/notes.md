# Husk:
Browser 1:
* https://nilsgs.github.io/presentations/ld/index.html#/
Browser 2:
* https://app.launchdarkly.com/settings/projects
* https://app.launchdarkly.com/default/development/features

# Intro
* Navn: Nils Georg Skutle
* Seniorkonsulent i Novanet, og sitter hos RiksTV

LaunchDarkly
* Hørt om det? 
* Erfaring?

# Agenda
* Bare kom med spørsmål underveis

# Hva er LaunchDarkly?
Rolls Royce, har alt du trenger av funksjonalitet. Pris deretter.
Vil være kostbart å bygge noe tilsvarende selv

Quote/Salgspitch. Kort fortalt: feature flags as a service.

# Admin UI
Projects og Environments:
* Projects måte å gruppere feature flags
* Enviroments, samme flagg i alle miljø. Ulikt resultat
* Flagg er knyttet til miljø ikke kode. Dermed kan det samme flagget gjenbrukes fler steder. Myttig i microservices arkitektur.

Users:
* Brukere som spør om flagg. Kommer tilbake med detaljer i SDK og når vi skal se nærmere på flagg.

Dev console:
* Live stream av aktivitet
* Vis med link
* Vis at caching fungerer

Audit log:
* Full audit av hva som har hendt

Web Hooks / Integrations:
* Web hooks: Kan abbonnere på endringer (Kun enterprise tier)
* Integrations: Slack/HipChat (Team tier)

# SDKs
* Støtter stort sett det du måtte trenge
* har i tillegg et REST API man kan integrere mot
* Offline mode / client side caching
* Real time updates

Kodeeksempel:
* Opprett klient med key
* Opprett user (evt. anonym)
* Spør om flagg

# Feature flags
* Opprett nytt flagg. 
* Vis forskjell mellom bool og multivariat
* Nevn permanent og Javascript SDK
* Targeting:
	- Prerequisite gir oss avhengighter mellom flagg
	- Target individual user: Marvin
	- Target matching rule. Email starts with "marvin"
	- Default rule / precentage rollout
	- If off serve ?
	- Lagre og slå på targeting
* Vis flagg status indikatorer
* Kill switch

# Prising
30 dager gratis

##How do you calculate monthly active users (MAU)?
We calculate the number of unique users across all environments over your billing cycle. Anonymous users can be tracked by session, so a single user who visits multiple times will only be counted once.

##Do you have free plans for non-profit, academic, or open-source projects?
Yes

# Takk for meg
* Konklusjon: Hvis du har behov for et robust, fleksibelt feature toggle system. Og du ikke vil bruke ressurser på å vedlikeholde det selv: så bør du vurdere LaunchDarkly

* Alternativer? Dårlig med tid, kom og snakk med meg etter på.

* Office Olympics