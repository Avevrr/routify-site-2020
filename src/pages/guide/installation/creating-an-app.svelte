<script>
  import { url, meta } from "@sveltech/routify";
  import Prism from "svelte-prism";
  import { Tabs, TabsLink, TabsPage } from "@sveltech/bricks";
  meta.title = "Getting started";
  import Note from "@/components/Note.svelte";
</script>

<!-- routify:options index=10 -->

<div class="c-container-vertical--small">
  <div class="c-content">
    <h1 class="c-h1">Creating an app</h1>
    <p>To create your first Routify app, open an empty folder and type</p>

    <Prism>{`npx @sveltech/routify init`}</Prism>

    <p>
      This will install the
      <a href="https://github.com/sveltech/routify-starter">
        Routify starter template
      </a>
      .
    </p>
  </div>

</div>

<div class="c-container-vertical--small">
  <div class="c-content">
    <h3>Bundled examples</h3>
    <p>
      The Routify starter comes with an example folder (
      <code>src/pages/examples</code>
      ).
    </p>
    <p>
      You can experiment with these examples or just keep them as references.
    </p>
    <p>
      When you're ready to get started on your app, simple delete the contents
      of
      <code>src/pages/index.svelte</code>
      and add your own. You will still be able to access the examples on
      <code>http://localhost:5000/examples</code>
      .
    </p>

    <p>
      When you don't need the examples anymore you can simply delete the
      examples folder.
    </p>
  </div>
</div>
<Note>
  We recommend reading the
  <a href={$url('../../introduction')}>Introduction</a>
  before creating your first app.
</Note>
