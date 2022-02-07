<template>
  <form>
    <Label
      :text="label"
      color="#303030"
    />
    <Input
      :placeholder="placeholder"
      :style="{ marginTop: '7px' }"
      @input="(val) => { inputVal = val; }"
    />
    <Button
      text="Comfirm"
      :style="{ marginTop: '4px' }"
      @click="$emit('submit', inputVal)"
    />
  </form>
</template>

<script>
import Label from '@/components/SingleResponsibitliyPrinciple/Label';
import Input from '@/components/SingleResponsibitliyPrinciple/Input';
import Button from '@/components/SingleResponsibitliyPrinciple/Button';

export default {
  components: {
    Label,
    Input,
    Button,
  },
  props: {
    label: String,
    placeholder: String,
  },
  data() {
    return {
      inputVal: '',
    };
  },
}
</script>
