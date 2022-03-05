<script lang="ts">
  import FeedbackItem from "./FeedbackItem.svelte"
  export let feedback: any[] = []

  console.log(feedback)
</script>

{#each feedback as fb (fb.id)}
  <FeedbackItem item={fb} on:delete-feedback />
{/each}