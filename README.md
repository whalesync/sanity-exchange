# Whalesync

**Two-way sync your Sanity content with Airtable, Google Sheets, Notion, Supabase, and more.**

[Start a free trial](https://app.whalesync.com/install/sanity?source=sanity_exchange) · [Docs](https://docs.whalesync.com/connectors/sanity) · [Pricing](https://www.whalesync.com/pricing?utm_source=sanity&utm_medium=marketplace&utm_campaign=listing&utm_content=pricing)

![A Sanity Studio document list and the same documents in an Airtable table, kept in two-way sync by Whalesync](https://raw.githubusercontent.com/whalesync/sanity-exchange/main/images/1-sanity-and-airtable.png)

## Run your Sanity content from the tools your team already uses

Whalesync keeps your Sanity datasets in two-way sync with Airtable, Google Sheets, Notion, Supabase, Postgres, HubSpot, Attio, and more. Every document type in your deployed Studio schema becomes a table and each document a row. Change a record on either side and the other side updates within seconds. Setup takes a few minutes with no code, and there is nothing to install in your Studio. 7-day free trial, no credit card.

### Common setups

- **Airtable:** bulk edits and AI-generated fields across hundreds of documents, and programmatic SEO pages from a base.
- **Google Sheets:** imports, bulk edits, and a content calendar the whole team can see.
- **Supabase and Postgres:** directories, listings, and product data from your database published through Sanity, or your Sanity content in your database for search and reporting.
- **Notion:** plan in a Notion database. Titles, slugs, SEO fields, authors, and publish dates edited there land in Sanity.
- **HubSpot, Attio, or Salesforce:** CRM data published to the site.

![Sanity documents in a Supabase table that Whalesync created](https://raw.githubusercontent.com/whalesync/sanity-exchange/main/images/5-sanity-and-supabase.png)

## Built for Sanity

Whalesync reads your document types from the schema your Studio deploys, nested objects like SEO settings, references between types, dates, slugs, and select lists included.

**References.** They sync as links to the related document, not just as text.

**Nested objects.** An `seo` object shows up as fields like `seo / Meta title`, so each part can be mapped on its own.

**Drafts and publishing.** Whalesync syncs the latest content whether it is published or still a draft. A Draft field lets you keep a change unpublished or publish it from the other app.

![A Sanity draft edited from Airtable, held unpublished by the Draft field](https://raw.githubusercontent.com/whalesync/sanity-exchange/main/images/4-drafts.png)

**Portable Text and images.** They sync out of Sanity as HTML and image URLs, so your content can feed reports, search indexes, or other tools.

**Instant updates.** Changes in Sanity come through on webhooks as they happen. A background pass picks up anything a webhook missed.

**Auto-create tables.** Point a sync at an empty Airtable base or Supabase database and Whalesync creates a table for every document type, with the fields to match.

![Whalesync mapping each field of a Sanity document type to an Airtable column](https://raw.githubusercontent.com/whalesync/sanity-exchange/main/images/3-field-mapping.png)

## Sync with confidence

Whalesync wants you to feel in control of your sync and protect your data. Deletes wait for your explicit approval. Sync a filtered subset of your data instead of a whole document type. Pause your sync at any time and it won't miss any changes when you resume. SOC 2 Type II certified and GDPR compliant.

## Keep a read-only copy of your content with Live Export

If you only need a read-only copy of your Sanity content in Airtable, Notion, Google Sheets, or Supabase, Whalesync's Live Export feature can help. It creates the tables and refreshes them on a schedule, anywhere from every 10 minutes to once a day. Sanity stays the source of truth.

## Build on top of your sync

**MCP server.** [Connect Whalesync](https://docs.whalesync.com/api/mcp) to Claude, ChatGPT, Cursor, or VS Code and have an agent set up, map, and monitor your Sanity syncs. Get your agent's help solving any issues with your data.

**REST API.** Create, monitor, pause, and retry syncs and Live Exports from your own code.

**Sync webhooks.** Whalesync can send an HTTP POST to your endpoint each time it creates, updates, or deletes a document in Sanity. Use it to trigger a site rebuild, clear a cache, or post to Slack.

## Get started

Before you start, you need:

- A Sanity project with your Studio schema deployed. Run `npx sanity schema deploy` in your Studio project (Studio 3.88 or newer).
- An account in the app you want to sync with, such as Airtable, Google Sheets, or Notion.

Steps:

1. Go to [app.whalesync.com/install/sanity](https://app.whalesync.com/install/sanity?source=sanity_exchange) and sign in, or create an account (7-day free trial, no credit card).
2. In [sanity.io/manage](https://www.sanity.io/manage), open your project, go to **API → Tokens**, and add a token with the **Editor** role. Paste it into Whalesync.
3. Pick the dataset to sync.
4. Pick the other app you want to sync with and connect it.
5. Select the document types you want to sync. Match them with existing tables in the other app, or have Whalesync create new ones.
6. Check the field mapping and click Save and continue.
7. Click Activate sync. Whalesync will copy your existing documents, then keeps both sides in sync.

![Whalesync dialog to connect a Sanity project with an API token](https://raw.githubusercontent.com/whalesync/sanity-exchange/main/images/7-connect-sanity.png)

Full guide: [docs.whalesync.com/connectors/sanity](https://docs.whalesync.com/connectors/sanity)

## Good to know

- **The deployed schema is the schema.** When you change your Studio schema, deploy it again and refresh the schema in Whalesync so the new fields appear.
- Portable Text, images, files, and references to more than one document type sync one way, out of Sanity.
- Content Releases are not synced.

## Learn more

- [Whalesync for Sanity](https://www.whalesync.com/connector/sanity?utm_source=sanity&utm_medium=marketplace&utm_campaign=listing&utm_content=website)
- [Supported services](https://www.whalesync.com/connectors?utm_source=sanity&utm_medium=marketplace&utm_campaign=listing&utm_content=connectors)
- [Pricing](https://www.whalesync.com/pricing?utm_source=sanity&utm_medium=marketplace&utm_campaign=listing&utm_content=pricing)
- [Documentation](https://docs.whalesync.com/connectors/sanity)
- [Security](https://security.whalesync.com)
- Support: support@whalesync.com

Whalesync is an independent product and is not affiliated with or endorsed by Sanity, Airtable, Google, Notion, Supabase, or any other service it connects to.
