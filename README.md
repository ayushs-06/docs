# RPI Docs

The Revenue Programming Interface (RPI) is Profound's internal intelligence layer that connects every signal across the revenue cycle — Salesforce account data, Gong call transcripts, HubSpot firmographics, and live web intelligence — into a single, AI-powered workspace for Sales and CS. Rather than stitching together exports across tools, RPI runs Claude AI agents continuously in the background: summarizing every customer call, extracting action items, profiling target companies, diagnosing lost deals, and assembling tailored meeting briefs before every conversation. Built on a FastAPI backend, PostgreSQL, and an SQS-driven worker pipeline, RPI syncs hourly from Snowflake and surfaces exactly the right context — at the account, call, and contact level — so your team spends less time researching and more time closing.

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mint) to preview your documentation changes locally. To install, use the following command:

```
npm i -g mint
```

Run the following command at the root of your documentation, where your `docs.json` is located:

```
mint dev
```

View your local preview at `http://localhost:3000`.

### Troubleshooting

- If your dev environment isn't running: Run `mint update` to ensure you have the most recent version of the CLI.
- If a page loads as a 404: Make sure you are running in a folder with a valid `docs.json`.

### Resources
- [Mintlify documentation](https://mintlify.com/docs)
