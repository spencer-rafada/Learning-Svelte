<script>
  import ComponentEvents from "./ComponentEvents.svelte";
  function handleMessage(event) {
    alert(event.detail.text);
  }
</script>

<ComponentEvents on:message={handleMessage} />
