<div align="center">

<img src="https://gitdoc.ai/logos-dark.svg" alt="GitDocAI" width="120">

# GitDocAI

### Docs that write themselves. And keep themselves up to date.

[![Website](https://img.shields.io/badge/Website-gitdoc.ai-0EA5E9?style=flat-square)](https://gitdoc.ai)
[![Docs](https://img.shields.io/badge/Docs-docs.gitdoc.ai-6366F1?style=flat-square)](https://docs.gitdoc.ai)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-GitDocAI-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/company/gitdocai/)
[![Contact](https://img.shields.io/badge/Contact-contact@gitdoc.ai-EC4899?style=flat-square)](mailto:contact@gitdoc.ai)

<br />

</div>

<div align="center">

Connect a GitHub repo and we generate **a complete, branded documentation site from your code — and host it for you on the internet,**<br />
at your own custom domain with auto-SSL. Every commit proposes a PR-style documentation update you can accept, reject, or edit. **No more doc rot.**

</div>

<br />

---

<br />

<div align="center"><h2>What makes GitDocAI different</h2></div>

<br />

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>Living docs from your repo</h3>
      <p>Generated from your code, kept alive by your commits. Every push detects the diff, regenerates only what's affected, and proposes a PR-style update you can accept, reject, or edit.</p>
    </td>
    <td width="50%" valign="top">
      <h3>MCP integration</h3>
      <p>Every docs site is exposed as a Model Context Protocol server, so Claude, Cursor, ChatGPT and VS Code can read, search and edit your docs through structured tools.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>OpenAPI &amp; Swagger auto-docs</h3>
      <p>Drop an OpenAPI / Swagger spec and get fully structured API docs — endpoints, schemas, parameters, request and response examples — without writing a line.</p>
    </td>
    <td width="50%" valign="top">
      <h3>Crawl an existing website</h3>
      <p>Point GitDocAI at any website and we turn it into a structured documentation site. Works on SPAs too. Also bootstraps from file uploads or a plain-English description.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Inline AI-assisted editor</h3>
      <p>Rich MDX editor with autosave, version history, and a floating AI chat that can rewrite sections, fix grammar, or add examples — with full undo/redo.</p>
    </td>
    <td width="50%" valign="top">
      <h3>We host the site for you</h3>
      <p>Not just a generator — GitDocAI ships your docs as a live, production-grade site on the internet. Bring your own domain (<code>docs.yourcompany.com</code>) with auto-SSL via Cloudflare for SaaS. Full theming (fonts, colors, light/dark, logo, navbar) and multi-version support.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Traffic &amp; usage analytics</h3>
      <p>See visitor counts, page views, geo breakdowns, search queries and publish history. Understand what your users actually read and where they come from.</p>
    </td>
    <td width="50%" valign="top">
      <h3>AI Q&amp;A on your docs</h3>
      <p>Semantic vector search with natural-language answers. Your users get the right answer in one prompt instead of digging through pages.</p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Embeddable knowledge base</h3>
      <p>Drop your docs into your own site with a public unauthenticated widget. Customize hero, page selection, and styling.</p>
    </td>
    <td width="50%" valign="top">
      <h3>Team &amp; programmatic access</h3>
      <p>Admin / editor / viewer RBAC, plus API keys (<code>gdk_*</code>) for CI/CD pipelines and headless automation. The same keys plug into MCP.</p>
    </td>
  </tr>
</table>

<br />

---

<br />

<div align="center">

### Built for AI-native development

GitDocAI ships with a **first-class MCP server**: scoped permissions<br />
(`mcp:read` ⊂ `mcp:edit` ⊂ `mcp:publish`), OAuth Protected Resource Metadata (RFC 9728),<br />
35+ structured tools, and headless API keys (`gdk_*`) for CI and IDE plugins.

<br />

> *If you're building with AI agents, your docs should be a tool they can use<br />— not a static site they have to scrape.*

</div>

<br />

---

<br />

<div align="center"><h2>FAQ</h2></div>

<details>
<summary><b>How good is the AI output, really? Will I have to rewrite everything?</b></summary>
<br />
The AI drafts structured pages with correct headings, cross-references, code samples, and navigation — not a blob of text. Most teams keep 70–90% of generated content as-is and polish the rest. It gets you from blank page to near-shippable in minutes, which is the hard part.
<br /><br />
</details>

<details>
<summary><b>How is this different from other docs platforms?</b></summary>
<br />
Most docs platforms give you a great-looking empty shell — you still have to write every page. GitDocAI writes the pages for you from your existing repos, PDFs, videos, or audio, then lets your team edit and publish. Custom domains, AI search, and team roles are included on plans where most tools charge 2–3× more.
<br /><br />
</details>

<details>
<summary><b>How does the auto-sync with my GitHub repo actually work?</b></summary>
<br />
You install our GitHub App on the repo. When code changes, GitDocAI detects the diff, regenerates only the documentation that's affected, and proposes the change as a <b>pending update</b> — a PR-style diff you can review, accept, reject, or edit inline. Nothing is ever published to your live site without your approval, and the original AI-generated content stays editable.
<br /><br />
</details>

<details>
<summary><b>Can I edit the docs by hand, or is everything AI-generated?</b></summary>
<br />
Both. The dashboard ships an inline MDX editor with autosave and version history, plus a floating AI chat that can rewrite sections, fix grammar, or add examples — with full undo/redo. Auto-generated content, AI-assisted edits, and fully manual writing all live in the same flow.
<br /><br />
</details>

<details>
<summary><b>Can my AI agent (Claude, Cursor, ChatGPT, VS Code) read or edit my docs?</b></summary>
<br />
Yes. Every documentation is exposed as a Model Context Protocol (MCP) server with 35+ structured tools. Interactive clients use OAuth (RFC 9728); headless clients use API keys prefixed <code>gdk_*</code>. Scopes are tiered — <code>mcp:read</code> ⊂ <code>mcp:edit</code> ⊂ <code>mcp:publish</code> — so you can hand an agent a read-only key for Q&amp;A and an editor key for write workflows.
<br /><br />
</details>

<details>
<summary><b>Can I migrate from another docs platform?</b></summary>
<br />
Yes. Import Markdown files, export your current site as a URL crawl, or point us at your GitHub repo. Your existing content comes over in one import — no manual copy-paste.
<br /><br />
</details>

<details>
<summary><b>What types of content can I import?</b></summary>
<br />
Files (Markdown, PDF, Word, code, OpenAPI specs), websites (single page or full crawl), GitHub repositories (full repo, folder, or single file), audio recordings, screen recordings, and screenshots.
<br /><br />
</details>

<details>
<summary><b>Can I generate API documentation from OpenAPI specs?</b></summary>
<br />
Yes. Upload a JSON or YAML OpenAPI/Swagger spec (or select it from a GitHub repo), and we auto-generate endpoint pages with method badges, request/response schemas, and parameter tables.
<br /><br />
</details>

<details>
<summary><b>What happens to my docs if I cancel?</b></summary>
<br />
You always own your content. Export everything as Markdown or MDX any time — no lock-in. If you downgrade, your content stays live on the Free plan; if you cancel, you can export first. Your docs are never deleted without warning.
<br /><br />
</details>

<details>
<summary><b>Is my content private and secure?</b></summary>
<br />
Your drafts are always private. Published docs are public by default, but Pro and Business plans support auth-gated private docs. Data is encrypted in transit and at rest, and we're GDPR-ready. See our security page for details.
<br /><br />
</details>

<details>
<summary><b>Can I use my own domain?</b></summary>
<br />
Yes. On Essential plans and above, you can set a custom domain (e.g., <code>docs.yourcompany.com</code>). We handle DNS verification and SSL certificates automatically.
<br /><br />
</details>

<details>
<summary><b>What happens when my trial ends?</b></summary>
<br />
After the 15-day free trial, you can continue on the Free plan or upgrade. Your content is never deleted — you just lose access to premium features until you upgrade.
<br /><br />
</details>

<br />

---

<br />

<div align="center">

**[gitdoc.ai](https://gitdoc.ai)** · **[docs.gitdoc.ai](https://docs.gitdoc.ai)** · **[LinkedIn](https://linkedin.com/company/gitdocai/)**

<sub>Built with ♥ by the GitDocAI team</sub>

</div>
