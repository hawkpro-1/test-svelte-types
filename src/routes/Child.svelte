<script lang="ts" generics="Identifier extends string">
  type DataType = {
    [K in Identifier]: number;
  } & {
    name: string;
    children?: DataType[];
  };

  type Props = {
    data: DataType;
    identifier: string;
  };

  let { data, identifier }: Props = $props();
  // If I could do this i can set the Dataprop type to
  //  let { data }: DataProp<typeof identifier> = $props();
  // This does not work as i cannot get props seperatly
</script>

from child
