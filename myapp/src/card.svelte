<script>
  import MyButton from "./button.svelte";
  import MyCheck from "./checkbox.svelte";
  import MyInput from "./input.svelte";
</script>

<div class="bg-gray-600 rounded-lg p-8">
  <form action="/auth" class="flex flex-col space-y-4">
    <MyInput placeholder="Username" />
    <MyInput placeholder="Password" />
    <MyCheck />
    <MyButton name="Login" type="regular" size="sm" />
  </form>
</div>
