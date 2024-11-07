<script>
  import Child from "./Child.svelte";
  let data = {
    value: 121,
    name: "cde",
    children: [
      {
        value: 122,
        name: "cdeChild",
        children: [{ value: 123, name: "abcd" }],
      },
    ],
  };
</script>

Parent

<Child {data} identifier="value" />
