# FridgeAI – Privacy Policy (English draft)


> **DRAFT – not published, not legal advice.** Prepared 09/11/2026 from the
> app and server code (version 1.0.0). Before publishing:
> - fill in every `[TO FILL]`, make every `[DECISION]` and check every
>   `[VERIFY]` (see `docs/AGE_13_PLUS_REVIEW.md` for the full list);
> - have a lawyer review it (`[LEGAL REVIEW]`);
> - publish it at a permanent public https:// address, enter that address in
>   Play Console, and link it from the app.
>
> The Hebrew version (`docs/PRIVACY_POLICY.md`) says the same; keep them in
> sync. Any change in what the app does (accounts, payments, analytics, a new
> AI provider) requires updating both first.

Last updated: [TO FILL: publication date]

## Who we are

FridgeAI ("the app", "we") is developed and operated by Elroi Cohen, an
independent developer (an individual, not a company), Israel.
Privacy contact: thecooker232@gmail.com
[TO FILL / LEGAL REVIEW: postal address, if required.]

## Who the app is for

FridgeAI is intended for people **aged 13 and older**. It is not intended for
children under 13. Users aged 13–17 get additional safety measures (see
"Teens" below).

## What stays on your device

Your ingredients, favorites, shopping list, AI recipes you saved, and your
settings (language, units, food preferences, age group, and whether you
agreed to photo recognition) are stored **on your device only**. The app has
no user accounts, and we do not have a copy of this data. Android's automatic
cloud backup is turned off for the app.

## What is sent to our server, and when

Only when you choose to use an AI feature:

| Feature | What is sent | Where it goes |
|---|---|---|
| Recognizing ingredients from a photo | The photo you picked, the app language, and your age group ("13–17" or "18+") | FridgeAI server → AI provider |
| Creating a recipe | Your ingredient list; the options you chose (meal type, kosher, cooking time, servings, style, food preferences such as vegetarian or gluten-free, ingredients to avoid); titles of up to 10 recent suggestions (so the next idea is different); app language; measurement units; your age group | FridgeAI server → AI provider |
| "Report a problem" with an AI recipe | See "Reports" below | FridgeAI server (stored) |

 - The app does not add a name, email address, phone number, advertising ID or device ID to AI requests. However, the photo or text you choose to send may itself contain personal information. Avoid photographing people, documents or identifying details, and avoid entering personal information that is not needed for the request. IP addresses are processed for communication and usage limits, as explained below.
 - **For ordinary AI requests, our server does not store** photos, ingredient lists, preferences or generated recipes. It passes the data to the AI provider to process the request, and the response returns to your device. If you choose to report a recipe, a copy of that recipe is stored as part of the report, as described under "Reports".
- **Photo metadata is removed.** Before a photo leaves your device, the app
  removes its metadata – including the location where it was taken (GPS),
  camera details, dates and comments – and keeps only what is needed to show
  the picture (the image itself, colour information and its rotation). Our
  server removes it again before passing the photo on. A photo that can't be
  cleaned is not sent.
- **You agree first.** Before the first AI request, the app explains what is
  sent and to whom, and asks for your agreement. You can withdraw it in
  Settings; AI features then stop sending anything until you agree again.
- **Food preferences may be sensitive.** Choices such as "kosher", "gluten-free" or ingredients you avoid (for example because of an allergy) could reveal information about your religious practice or health. They are optional and used to create the recipe you requested. Our server does not store these preferences during ordinary AI requests. A recipe you choose to include in a report may reflect these preferences and be stored as part of that report. [LEGAL REVIEW]

### The AI provider
Photo recognition and recipe-generation requests are processed using Anthropic (Claude API). The information described above is sent to Anthropic to provide the response.

Further information:
https://privacy.claude.com/
- Under Anthropic's commercial-product policy, inputs and outputs sent through its API are not used to train its models by default. Content deliberately submitted as feedback or explicitly permitted for training may be subject to different terms.
- Under Anthropic's standard API retention policy, inputs and outputs are deleted within 30 days, subject to exceptions such as legal requirements and enforcement of its Usage Policy. Content flagged as a policy violation may be retained for up to two years, and related safety classification scores may be retained for up to seven years.
### Hosting

Our server is hosted by Render in Oregon, United States. Requests to it pass through Cloudflare, the
network provider Render uses, and are encrypted (HTTPS). Like any internet
service, Render and Cloudflare see your IP address when the app connects.
Our server's own logs, which Render keeps for 7 days, contain no IP
addresses. Render and Cloudflare may record IP addresses in their own network
systems, under their own privacy policies:
https://render.com/privacy and https://www.cloudflare.com/privacypolicy/

Spending counters, the per-user limits (as keyed one-way codes, no IP
addresses), the usage log and reports are stored in a database run by
Supabase in Stockholm, Sweden (EU), as our service provider. Supabase processes this data only on our behalf,
under its Data Processing Addendum, which is part of Supabase's Terms of
Service. [LEGAL REVIEW: confirm that this also covers the Free plan.]

### Preventing abuse and limiting costs

Each AI request costs us money, so the server limits how many requests one
user can make per hour and per day:

-- Usage limits are counted by IP address (for IPv6, by network). Our usage counters do not store the IP address in its original form. They are stored under a keyed one-way code (HMAC), calculated from the IP address and date using a secret key kept on our server. The code changes each day and is intended to reduce identification and linking across days of use, but it does not guarantee complete anonymity. The counters are deleted automatically after 2–3 days. Processing of IP addresses by our hosting and network providers is described under "Hosting".
  deleted automatically after 2–3 days.
- Our server logs record the time, the type of request, the result, the AI
  model used, the number of tokens and the estimated cost. They contain **no
  IP addresses and no content** (no photos, ingredients, recipes or
  comments). Detailed log lines are kept for 90 days; after that only daily totals are kept (number of requests,
  errors, blocked requests, cost).

## Reports ("Report a problem")

If you report an AI recipe, the app sends: the type of problem, your comment
(optional), the recipe as it was shown to you, the app language, your age
group ("13–17" or "18+", so that safety reports from teens are handled
first) and the app version.

- - The app does not add a name, email address, device identifier or location to reports. The comment and recipe you submit may themselves contain personal information, so please avoid including unnecessary identifying details. Your IP address is used to limit report submissions and is not stored with the report.
- Email addresses, phone numbers and links typed into the comment are
  removed before the report is stored.
- Reports are used only to check AI recipes and improve safety.
- **How long we keep reports:** a report is deleted automatically once we
  have reviewed it and 180 days have passed since it was received. Deletion
  happens at the server's next automatic cleanup after both are true.
  Reports not yet reviewed are kept until we review them. We keep a record of deletions that contains
  only the date, the number of reports and their problem types – no report
  content.

 - Reports are not linked to a user account or device identifier. For a request about a specific report, including deletion, contact thecooker232@gmail.com with the report date and recipe title and, if known, the report ID. We will try to locate the report using those details, but may not be able to identify it with certainty. Do not send passwords or identity documents.

## What we do not collect

No ads, no analytics or tracking tools, no selling or sharing of data for
marketing. The app does not ask for access to contacts, location or files,
except a photo you choose to send.

## Camera and photos

The camera or gallery is opened only when you tap "Take photo" or "Choose
photo", and only the photo you pick is used. Before your first photo is
sent, the app explains what happens to it and asks for your agreement; you
can withdraw it in Settings. Location and other metadata are removed before
sending (see above).

The app shows a summary of this policy under Settings → Privacy, with a link
to this full policy.

## Teens (13–17)

- The first time you use an AI feature, the app asks for your age group
  (18+, 13–17, under 13). Only the age group is saved – on your device, not
  a date of birth. With AI requests and reports the server receives only
  "13–17" or "18+", to apply the right safety rules; requests without it are
  refused.
- **Safety measures for users under 18.** Our AI provider, Anthropic, has
  extra requirements for apps used by people under 18. FridgeAI currently
  has these safeguards, for all users:
  - Before using an AI feature, users choose their age group. This is
    self-declared; it is not checked against any document.
  - AI features work only after the user has agreed to an explanation of
    what is sent and to whom. The agreement can be withdrawn in Settings.
  - Every recipe request includes safety instructions for families. Our
    server then checks each recipe: a recipe that contains alcohol, items
    that are not food, or diet or health claims is not shown. Steps that
    need an adult (for example hot oil or sharp knives) are marked.
  - Ingredients recognised in a photo are filtered: alcohol and items that
    are not food are removed.
  - Recipes created by AI are labelled as AI, so it is clear they come from
    an AI system and not from a person.
  - Anyone can report a problem with an AI recipe from inside the app, and
    reports are kept for review.
- These safeguards reduce risk, but they cannot guarantee that every AI
  answer is suitable. Please use your own judgement in the kitchen.
- [LEGAL REVIEW: which child-safety and privacy laws apply (for example
  Israel's Privacy Protection Law, and the US Children's Online Privacy
  Protection Act (COPPA) if the app is offered in the US), whether FridgeAI
  meets them, and what public compliance statement Anthropic's guidelines for
  organisations serving minors call for. Do not add any compliance claim
  before this review.]
- We recommend that teens go over this policy and the photo explanation with
  a parent.
- **Under 13:** the app is not intended for children under 13. If "Under 13"
  is chosen, **nothing is sent to our server** – no AI requests, photos,
  reports or even availability checks – and the features that work only on
  the device (fridge, built-in recipes, favorites, shopping list) stay
  available. Any agreements given earlier are cleared, and must be given
  again if the age group is later changed. Our server also refuses any
  request marked as under 13.
- [LEGAL REVIEW: requirements for users aged 13–17 in each country where the
  app is offered, including whether parental consent is needed for some ages
  (e.g. EU member states set 13–16 for some services).]

## Your choices and rights
- You are not legally required to provide information to use our AI features. Providing it is voluntary and based on your agreement. Without the information needed for a request, we cannot provide the requested AI feature, but local features remain available.
- Subject to applicable legal conditions, you may request access to personal information about you held in our database and request correction of information that is inaccurate, incomplete, unclear or outdated. Contact thecooker232@gmail.com. We will request only the details reasonably necessary to locate the information and verify the request.
- Delete your data on the device: Settings → "My data" (each part, or
  everything). Uninstalling the app also deletes it.
- Our server keeps no account or profile about you. For questions or
  requests about your personal information, contact
  thecooker232@gmail.com.
- [LEGAL REVIEW: your rights under the Israeli Privacy Protection Law
  (including Amendment 13) and, if the app is offered in the EU/UK, the GDPR
  (access, correction, deletion, objection, complaint to a supervisory
  authority) – and how requests are verified without accounts.]

## International transfers

Your requests are processed outside Israel. Our server (Render) is hosted
in the United States, and data sent for AI processing is handled by
Anthropic, a US company. Our database (Supabase) is hosted in Sweden, in the
European Union. Cloudflare may carry requests through servers in other
countries on the way. [LEGAL REVIEW: legal basis for these transfers under
Israeli law and, if relevant, the GDPR.]

## Security

Communication with the server is encrypted (HTTPS). The AI provider's key is
kept only on the server, never in the app. The server keeps as little data
as possible, as described above.

## Changes to this policy

If we add accounts, payments, analytics or a new kind of data collection, we
will update this policy before the change and tell you in the app.
