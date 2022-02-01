---
title: Modal
desc: Modal Description
published: true
---

<script>
  import Component from "@components/Component.svelte"
</script>

<Component title="Modal using label + hidden checkbox">
<label for="my-modal" class="btn modal-button">open modal</label>
<pre slot="html">{
`<!-- The button to open modal -->
<label for="my-modal" class="btn modal-button">open modal</label>

<!-- Put this part before </body> tag -->
<input type="checkbox" id="my-modal" class="modal-toggle">
<div class="modal">
  <div class="modal-box">
    <h3 class="font-bold text-lg">Congratulations random Interner user!</h3>
    <p class="py-4">You've been selected for a chance to get one year of subscription to use Wikipedia for free!</p>
    <div class="modal-action">
      <label for="my-modal" class="btn">Yay!</label>
    </div>
  </div>
</div>`
}</pre>
</Component>

<Component title="Modal using anchor link" desc="Anchor links might not work well on some SPA frameworks so if there are problems, use the first example">
<a href="#my-modal-2" class="btn" rel="external">open modal</a>
<pre slot="html">{
`<!-- The button to open modal -->
<a href="#my-modal-2" class="btn">open modal</a>

<!-- Put this part before </body> tag -->
<div class="modal" id="my-modal-2">
  <div class="modal-box">
    <h3 class="font-bold text-lg">Congratulations random Interner user!</h3>
    <p class="py-4">You've been selected for a chance to get one year of subscription to use Wikipedia for free!</p>
    <div class="modal-action">
     <a href="#" class="btn">Yay!</a>
    </div>
  </div>
</div>`
}</pre>
</Component>